# QA — USPS Money Orders

Article: `content/drafts/usps-money-order-how-it-works.md` (draft, 2026-11-26, about 1,510 words including sources, one H1, Sources included; meta description 137 characters; alt text 1,166 characters).

Stage: draft. Gate 1 (Claude) run on 2026-11-26. Gate 2 round 1 = FIX (two points, fixed 2026-11-26, see below); waiting for Gate 2 on the changed parts. Backlog row 48.

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

## Image checks
PNG 1200 x 3372 px, 626839 bytes, SHA-256 prefix `73d8785813052cbd`; SVG 6213 bytes; md 12361 bytes, `1a8d811591096d1e` (after the Gate 2 fix; before: PNG 3027 px `3c4a2e6a0efcd892`, md `f60ca658e975a336`); C2PA chunk and metadata stripped on the device. The rendering script printed no text past the right margin; the PNG was viewed. Diagram text only repeats facts from the article; alt text matches the front matter and the Markdown alt text.

## Not checked
Search volume; fees and notices (Notice 123); DMM 509 beyond 3.0; WordPress (no draft or schedule exists); mobile and editor checks (after Gate 2 PASS); the pre-publication source re-read.
