# QA record — usps-return-receipt-how-it-works

Article: `content/drafts/usps-return-receipt-how-it-works.md` (draft, 2026-11-24, about 2,000 words in the body, one H1, nine H2 sections including Sources, one table; meta description 149 characters; alt text 784 characters).
Brief: `research/briefs/usps-return-receipt-how-it-works.md`. Sources: `research/sources/usps-return-receipt-how-it-works.md` (R1 to R3, read 2026-11-24).
Stage: ready; scheduled (WordPress post 174). Gate 1 (Claude) run on 2026-11-24. **Gate 2 round 1 (ChatGPT, base `f839045`, user-reported 2026-11-24): FIX, four items, applied 2026-11-24** (section "Gate 2 FIX round 1"); **Gate 2 round 2 (base `ee58248`) = PASS for the changed parts (user-reported 2026-11-24); the reviewer could not screen-check the PNG, the repository PNG was viewed by Claude**; scheduled 2026-11-24 (section "Scheduling record"). Backlog row 44.

## Scope
- No fees, prices or percentages; dollar thresholds in the class lists are written as "a value the FAQ states"; trends are not in the article; search volume not checked.
- Three internal links, each once: Certified Mail, redelivery, refund (the Priority Mail Express post is not linked).

## Method
All three sources were opened on 2026-11-24 and each statement was tested by script.

| Source | Phrase checks | Matched at once | Notes |
|---|---|---|---|
| R1 FAQ Basics (000006076) | 45 | 44 | the page runs "certain" and "destinations" together; sentence read |
| R2 FAQ Electronic (000007257) | 29 | 29 | |
| R3 DMM 503 section 6.0 | 13 | 13 | tested within section 6.0 only |
| Total | 87 | 86 | |

## Gate 1 — claim groups

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | Lead: proof of delivery (signature, date, actual delivery address if different); bought at the time of mailing; green card PS Form 3811 or email; cannot be bought after mailing; 90-day request if paid and not received | R1, R3 | pass |
| C2 | What it shows: signature of the recipient or authorized agent, date and time, address; DMM wording "to whom the mail was delivered and date of delivery" | R1, R3 | pass |
| C3 | Table: card mailed after delivery; email with a link and a letter attached; requested at mailing; email requested afterward on USPS Tracking; not purchasable on USPS.com; Post Office; cannot be viewed online; electronic not for APO, FPO, DPO, territories | R1, R2, R3 | pass |
| C4 | Table: green card "where to buy": not stated; mail from home, office or collection box if fees, postage and form are affixed | R1 | pass |
| C5 | DMM purchase rules: complete return address; PME label meets it; PS Form 3811 entries and attached; return name and address the mailer's except the ENDS, cigarette and smokeless tobacco cases; endorsement; no endorsement for electronic; weight excluded | R3 | pass |
| C6 | Classes: PME "Form 3811 only", Priority Mail, First-Class Mail, Ground Advantage - Commercial, Parcel Select with the parenthetical condition (the article says the FAQ does not say whether it covers earlier classes); further classes with COD or insurance condition; international Registered Mail to certain destinations and PS Form 2865 pink card | R1 | pass |
| C7 | Extra services list; some "Form 3811 only"; the electronic FAQ marks PME "Form 3811 only"; the DMM PME sentence carries "Form 3811 option only" | R1, R2, R3 | pass |
| C8 | Electronic: request at mailing; wait for delivery and signature record; USPS Tracking, article number, email address; Basics FAQ steps for requesting again; no barcode number, no electronic version | R2, R1 | pass |
| C9 | Timing: immediate if delivered, within hours depending on the email server; otherwise usually within 48 hours of delivery; link and attached letter | R2 | pass |
| C10 | "designed to be equivalent to"; "is not determined by the Postal Service"; courts; two years; slower after 60 days; Bulk Proof of Delivery at 25 items per day, signature extract file | R2 | pass |
| C11 | Related Tracking Number tracks the card, not the mailpiece; tracking status of the delivery record after delivery | R1 | pass |
| C12 | 90 days; PS Form 3811-A at any Post Office, station or branch with the receipt | R1, R3 | pass |
| C13 | Refund: only if USPS fails to provide the signature (unless refused, unclaimed or returned); usps.com/help or origin Post Office; "not less than 30 days, or more than 60 days from the date of mailing"; retail purchase: after 30 calendar days from mailing or any time after known delivery; electronic: 3 to 5 days, check status, junk folder, request again | R1 | pass |
| C14 | Differences: email timing; how the email address is given (Basics FAQ, DMM, Electronic FAQ); refund timing sentences; PME electronic | R1, R2, R3 | pass |
| C15 | Not said: green card transit time; court acceptance; fees point to Notice 123 and "Insurance & Extra Services" | R1, R2 | pass (absence checks) |

## Image checks
After round 1: PNG 1200 x 3372 px, 627,035 bytes, SHA-256 prefix `3497373ec6f530e2`; SVG 6,141 bytes, `4b3886823a585261`; md 14,027 bytes, `1f5a56cb3b399073`; alt text 1,044 characters (first version: PNG 3234 px, `02ad054d8b57c44a`; SVG `19687db61f06f3e8`; md `79f7080f754b822d`; alt 784); C2PA chunk and metadata stripped on the device (hashes equal the originals). The rendering script printed no text past the right margin; the PNG was viewed. Alt text (784 characters) matches the front matter and the Markdown alt text.

## Open points for Gate 2
1. "Not stated" for where to buy the green card, and the sentence about the parenthetical condition after Parcel Select: fair readings of the FAQ?
2. (Round 1 asked for the Priority Mail Express point to be tied to the form a reader can choose and for the DMM note's scope to be marked separately; applied. Re-check the new wording.)
3. The two refund-timing sentences shown as a difference.
4. (Round 1: the electronic timing and the 3 to 5 day advice are no longer shown as a difference; re-check.)

## Not checked
WordPress draft, editor, mobile, live page, publication slot. Search volume: not checked. Return Receipt for Merchandise not read.

## Gate 2 FIX round 1 (2026-11-24, base `f839045`): applied

Reviewer result, four items: (1) the diagram's "usually available within 48 hours of delivery" lacked its condition: USPS gives it for a request made before delivery (USPS waits for delivery and for the signature record to be complete); for an item already delivered with the record complete, the FAQ says it is processed immediately; diagram, alt and the differences text had to be aligned. (2) The diagram's refund line lacked the exceptions (refused, unclaimed, returned to sender) that the body has. (3) "48 hours" and "check after 3 to 5 days" have different starting points and purposes, so calling them a conflict is not safe; they should be explained side by side. (4) On Priority Mail Express, the FAQs mark "Form 3811 only"; the article should tie that to the form a reader can choose and mark the scope of the DMM wording separately, instead of saying the pages do not say whether PME can have the electronic version.

Applied: (1) diagram card 3 and the alt text: "requested before delivery: usually available within 48 hours of delivery; already delivered and recorded: processed right away." (2) diagram card 4 and the alt text: the fee is refunded only if USPS fails to provide the signature, unless the item was refused, unclaimed or returned to the sender. (3) the body's timing bullet was removed from "Where the USPS pages differ" and replaced by two sentences in "Getting the electronic version": the 48-hour sentence applies to a request made before delivery, and the 3 to 5 day advice counts from the request and tells a sender what to check and is not a second delivery time; the diagram's differences card no longer lists email timing. (4) "Which mail it goes with": both FAQs mark Priority Mail Express "Form 3811 only", Form 3811 is the green card (one of the two forms a mailer can choose between), so the FAQs point to the green card rather than the email for PME; the DMM's similar note "Form 3811 option only" is in its sentence about the return address on the PME label, so the article reads it as applying to that sentence, not to the whole service; the PME bullet was removed from the differences list; diagram card 2 adds "Priority Mail Express: marked Form 3811 only." The differences list now has two items (how the email address is given; refund timing); the alt text matches.

Phrases used were already tested against the Basics FAQ, the Electronic FAQ and DMM 6.0 on 2026-11-24 (Form 3811 only on both FAQ lists; "usually available to be sent by email within 48 hours of delivery"; "we will process it immediately"; "Form 3811 option only" in 6.1.1). Nothing is published; Gate 2 round 2 is needed.

## Scheduling record (2026-11-24)
Right before scheduling, the three sources were read again (FAQ 000006076 still dated Sep 18, 2026: 29 of 32 phrase checks at once, the three others are my wording of lines on the page (recipient or authorized agent, 30 calendar days, 3-5 days); FAQ 000007257 still dated May 18, 2026: 24 of 26 at once, the two others are lines that exist (processed immediately, official United States Postal Service document); DMM 503 section 6.1 read: evidence of delivery, return address, Form 3811 option only, endorsement, 90 days, PS Form 3811-A unchanged). No important change, so nothing was reported first. Built from the repository files on `main` (md `1f5a56cb3b399073`, PNG `3497373ec6f530e2`; converted content hash equal to the Python reference), media 172 (image 200, hash equal), post 174 created as a draft in category Postal service and stamps, comments and pings closed, Rank Math keyword and description set (149 characters). Editor: 29 blocks, 0 invalid (one table). Preview at 375 px and 320 px: no page overflow, the table fits its figure (315 and 260 px), one H1. File moved to `content/ready/` with `status: ready`. Scheduled for 2026-11-25 15:00 KST (06:00 UTC; the site shows 2026-11-25 01:00 because its timezone is America/New_York, UTC-5). Re-read after saving: status future, date_gmt 2026-11-25T06:00:00. Not public yet (public posts: 39). Live QA is still to be run after the post appears.
