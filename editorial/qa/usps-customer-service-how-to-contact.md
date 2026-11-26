# QA — USPS Customer Service

Article: `content/ready/usps-customer-service-how-to-contact.md` (ready, 2026-11-26, about 1,100 words including sources, one H1, Sources included; meta description 144 characters after the Gate 2 fix; alt text 920 characters).

Stage: scheduled (WP post 190, 2026-11-28 09:00 KST). Gate 1 (Claude) run on 2026-11-26. Gate 2 round 1 = FIX (one point, fixed 2026-11-26, see below); Gate 2 on the changed parts (commit `bdf12d7`) = PASS. Backlog row 49.

## Gate 1 — claim groups
- USPS.com Contact Us: 34 of 34 phrases found.
- USPS Email Us: 18 of 18.
- USAGov complaint page: 22 of 23 (1 phrase typo of mine, verified on the page).
- The article gives no price, fee, insurance amount or percentage (no dollar or percent sign). It gives phone numbers and hours as the pages list them, dated; it does not give the stamps / Postal Store or free-supplies numbers, the OIG number or the Consumer Advocate address.
- Link text matches the live titles of `usps-tracking-status-what-it-means` and `usps-missing-mail-search-how-it-works`; link status to be confirmed in the WordPress build.

## Former "Where the pages differ" (replaced after Gate 2, see below)
- Mail theft: Email Us topic (theft of mail) vs USAGov (outside theft to the Postal Inspection Service).
- Informed Delivery help: USPS.com technical-issue topic vs separate Informed Delivery support email.
- Tracking questions: Email Us "Where is my package?" vs separate tracking phone line.
- TTY: "TTY: 711" vs dialing 7-1-1 to reach a state relay service.

## Gate 2 round 1 — FIX and what changed
Gate 2: the article's "Where the pages differ" section and diagram card presented four items as differences between sources, but most are different routes for the same kind of question, not conflicting rules. Examples: USAGov's "TTY: 711" and the USPS page's 7-1-1 relay description are not separate numbers or conflicting rules; tracking questions have an Email Us topic and a phone line as different intake routes. Theft: USAGov separates USPS employee or facility cases (Office of the Inspector General) from outside mail fraud or theft (Postal Inspection Service).
Fix: the section is now "Which route fits which problem", a grouping by problem (delivery or mail service; tracked package; USPS.com technical problem and Informed Delivery; mail theft or fraud; policy change; hearing or speech needs) that states what each page says without calling anything a conflict. The introduction sentence, meta description ("which route fits which problem"), diagram card 4 ("Which route fits which problem") and the last sentence of the alt text (front matter and Markdown alt text identical) were changed to match. The "What the pages do not say" paragraph gained the gap "which route to start with if you are unsure who took a piece of mail", which none of the pages states. USAGov page re-read on 2026-11-26 (updated September 4, 2026): the three complaint routes, the OIG and USPIS split, the PRC line and "TTY: 711" are as written.

## WordPress build and schedule (2026-11-27 KST)
Pre-publication re-read: Contact Us (phone numbers, hours, TRS text, chat and form lines, supply and stamps lines unchanged), Email Us (six topics and examples unchanged; all 21 checked phrases found) and the USAGov page (re-read 2026-11-26 for the Gate 2 fix, updated September 4, 2026). Gate 1's 8 "misses" on Contact Us were dash and spacing differences ("Monday - Friday 8 AM - 8:30 PM ET"), not wording changes.
Built from the pushed files at commit `bdf12d7` (md `b72f377abe17d700`, PNG `e02240bd3773738b`; converter output equals the Python converter, 11,783 characters, SHA-256 `30575bdb...2f2f`). Media 189 (PNG 1200 x 2538, alt 920 characters equal to the front matter; original URL hash read back equal). Draft post 190: category 6, comments and pingbacks closed, Rank Math description (144 characters) and focus keyword `usps customer service`. Editor: 25 blocks, 0 invalid. Preview 375 and 320 px: no horizontal overflow, one H1, image 315 and 260 px wide. Internal links `/usps-tracking-status-what-it-means/` and `/usps-missing-mail-search-how-it-works/` returned 200. Scheduled `future`, `date_gmt` 2026-11-28T00:00:00 = 2026-11-27 19:00 site time (New York) = 09:00 KST on 2026-11-28; read back from WordPress. The Free Boxes post (3 PM KST) links to this post, so this one must be public first.

## Image checks
PNG 1200 x 2538 px, 514710 bytes, SHA-256 prefix `e02240bd3773738b`; SVG 4814 bytes after the C2PA metadata block was removed on the device; md 10,368 bytes, `b72f377abe17d700` (after the Gate 2 fix; before: PNG 2469 px `48d0a5f99f7d525b`, md 9,260 bytes `13807bc240da83c1`); C2PA `caBX` chunk removed from the PNG (pixel data hash unchanged). The rendering script printed no text past the right margin; the PNG was viewed. Diagram text only repeats facts from the article; alt text matches the front matter and the Markdown alt text.

## Not checked
Search volume; whether the phone numbers and hours change after the 2026-11-27 re-read; the pages for OIG, USPIS and PRC; live-site QA (due about 09:20 KST on 2026-11-28).
