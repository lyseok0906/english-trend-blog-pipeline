# QA — USPS Money Orders

Article: `content/ready/usps-money-order-how-it-works.md` (ready, 2026-11-26, about 1,510 words including sources, one H1, Sources included; meta description 137 characters; alt text 1,209 characters).

Stage: scheduled (WP post 187, 2026-11-27 15:00 KST). Gate 1 (Claude) run on 2026-11-26. Gate 2 round 1 = FIX (two points, fixed 2026-11-26, see below); Gate 2 round 1 changed parts = PASS (commit `91d5b5f`). Pre-publication source re-read (2026-11-26) found one small wording difference, fixed (see below); Gate 2 on that change (commit `0bdda77`) = PASS. Backlog row 48.

## Gate 1 — claim groups
- FAQ 000006987 (Jun 10, 2026): 46 of 48 phrases found (2 phrase typos of mine, verified on the page).
- USPS.com Sending Money Orders page: 31 of 31.
- DMM 509.3 (3.1 to 3.3.6): 24 of 24.
- The article gives no amount: no single-order limit (user instruction), no fee, no inquiry or replacement fee, no daily-total thresholds, no international maximum. The DMM's traveler's-check share is written as "at least half of their value" (no percent sign). No dollar sign or percent sign in the article.
- Live link text matches the published title of `usps-claim-how-it-works` ("USPS Claims: Filing Periods, Who Can File and What You Need"); link status to be confirmed in the WordPress build.

## Where the pages differ (shown in the article, not resolved)
- Traveler's checks: not accepted (FAQ), listed with a condition (DMM), not listed (USPS.com: cash or debit card).
- Refund or replacement timing: refund if not cashed in the first 30 days after sale; refund if not cashed within 10 business days after the inquiry; receipt wording says no replacement until 60 days after purchase.
- Where to buy: Post Offices (USPS.com), rural carriers and some contract stations (FAQ), a longer list in the DMM.

## Gate 2 round 1 — FIX and what changed
Gate 2 compared the article with the DMM: (1) Payees: the buying section cites DMM 3.2.4 (a money order must be made payable to a single identifiable party) while the cashing section explains "and"/"or" rules for several payees (DMM 3.3.5); the DMM words these for different steps, so the article must not present one fixed rule. (2) Lost-receipt wording: the diagram and alt text read as if the receipt were required for an inquiry, while the body said an inquiry form can be filled in without it.
Fix: (1) Buying: now says 3.2.4, on how the purchaser completes the order, requires a single identifiable payee, and that 3.3.5, on cashing, separately covers more than one payee. Cashing: the "or" / "and" / no-conjunction rule is attributed to 3.3.5 and the article says the DMM does not say how it fits with 3.2.4. New bullet "One payee or several" in "Where the USPS pages differ" (DMM 3.2.4 against 3.3.5; different steps, not reconciled). (2) Re-read the FAQ: the no-receipt sentence ("you may still complete inquiry form with all of the required information and return it to the window clerk") sits in the FAQ's steps for spoiled or damaged money orders, not in its lost or stolen steps, which say to take the receipt. The body now says exactly that (damaged or spoiled only; not repeated for lost or stolen). Diagram card 4 now separates the two: lost or stolen, take the receipt; damaged or spoiled, replaced with the money order and receipt, and without the receipt the FAQ says the inquiry form can still be filled in. Alt text rewritten to match; front matter and Markdown alt text identical. Diagram card "Where the pages differ" has a payees line.
Re-checked on the pages 2026-11-26: DMM 509 5 of 5 new phrases (3.2.4 heading and sentence, 3.3.5 heading, the "or" and "and"/no-conjunction sentences); FAQ no-receipt sentence and the lost or stolen steps read directly.

## Pre-publication re-read — ID wording and form name (post-PASS correction)
FAQ 000006987 says an "acceptable primary form of identification" is required to cash; the USPS.com page says to take a primary photo ID. The article had merged both into "acceptable primary photo ID" and said the FAQ and USPS.com "give the same steps". Fix: the body now says "bring identification" in the shared steps, then "The FAQ says an acceptable primary form of identification is required; USPS.com says to take a primary photo ID." Diagram card 2 reads "bring an acceptable primary ID (USPS.com: primary photo ID)"; alt text matches (front matter and Markdown alt text identical). "PS Form 6387" in the body is now "Form 6387", the DMM 509.3 wording. Nothing else changed; the DMM payee and no-receipt wording that passed Gate 2 is untouched. Re-read in full: FAQ phrases (6 apparent misses verified as wording differences), USPS.com page (payment, status, 30 and 60 days, designs), DMM 509.3 (3.2.1, 3.2.3, 3.2.4, 3.3.1, 3.3.3, 3.3.5). Not re-read after the fix: the four spot-a-fake checks on USPS.com, which the article states unchanged from Gate 1.

## WordPress build and schedule (2026-11-26)
Built from the pushed files at commit `0bdda77` (the browser fetched the Markdown and PNG from the repository at that commit: md `30e4460968e1a9fa`, PNG `d747d458a2e76edd`). The JavaScript converter output equals the Python converter (12,821 characters, SHA-256 `ba461895...e573`). Media 186 (uploaded PNG 1200 x 3441, alt text 1,209 characters equal to the front matter; WordPress also made a `-scaled` copy, the post uses the original URL, hash `d747d458a2e76edd` read back). Draft post 187: category 6, comments and pingbacks closed, Rank Math description (137 characters) and focus keyword `usps money order` set. Editor: 25 blocks, 0 invalid. Preview at 375 px and 320 px: no horizontal overflow, one H1, image 315 and 260 px wide. The internal link `/usps-claim-how-it-works/` returned 200. Scheduled `future` with `date_gmt` 2026-11-27T06:00:00 = 2026-11-27 01:00 site time (New York) = 15:00 KST; status, date and date_gmt re-read from WordPress. Pre-publication re-read: FAQ, USPS.com page (including the four spot-a-fake checks and verification options, re-read after the fix) and DMM 509.3 done; no other change.

## Image checks
PNG 1200 x 3441 px, 643454 bytes, SHA-256 prefix `d747d458a2e76edd`; SVG 6373 bytes; md 12541 bytes, `30e4460968e1a9fa` (after the ID-wording fix; after the Gate 2 fix: PNG 3372 px `73d8785813052cbd`, md `1a8d811591096d1e`; first draft: before: PNG 3027 px `3c4a2e6a0efcd892`, md `f60ca658e975a336`); C2PA chunk and metadata stripped on the device. The rendering script printed no text past the right margin; the PNG was viewed. Diagram text only repeats facts from the article; alt text matches the front matter and the Markdown alt text.

## Not checked
Search volume; fees and notices (Notice 123); DMM 509 beyond 3.0; ; live-site QA (due about 15:20 KST on 2026-11-27).
