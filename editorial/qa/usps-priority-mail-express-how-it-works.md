# QA record — usps-priority-mail-express-how-it-works

Article: `content/drafts/usps-priority-mail-express-how-it-works.md` (draft, 2026-11-24, about 1,900 words in the body, one H1, nine H2 sections including Sources; meta description 146 characters; alt text 891 characters).
Brief: `research/briefs/usps-priority-mail-express-how-it-works.md`. Sources: `research/sources/usps-priority-mail-express-how-it-works.md` (S1 to S4, read 2026-11-24).
Stage: draft. Gate 1 (Claude) run on 2026-11-24. Gate 2 not yet run. Backlog row 43.

## Scope
- No prices, fees, insurance amounts or percentages anywhere (the article says the Sunday and holiday fee exists and does not give it); trends are not in the article; search volume not checked.
- Refund rules are given briefly as the FAQ states them; the chart from DMM 604.9 stays in post 147.
- Five internal links, each once, link text equal to the live titles: refund, holiday deadlines, tracking status, redelivery, claim.

## Method
All four pages were opened on 2026-11-24 and each statement tested by script (normalization as in the source notes).

| Source | Phrase checks | Matched at once | Notes |
|---|---|---|---|
| S1 FAQ PME (000008250) | 69 | 69 | |
| S2 USPS.com PME | 17 | 17 | page prices not used |
| S3 FAQ Waiver of Signature (000006914) | 19 | 18 | miss: typo in my phrase ("Label Label"); page text read |
| S4 FAQ Hold for Pickup (000008085) | 9 | 9 | |
| Total | 114 | 113 | |

## Gate 1 — claim groups (each tested against the source named)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | Lead: 1-3 days, 6 PM local time, most U.S. addresses and PO Boxes, money-back guarantee; day depends on ZIP Codes, date and time of mailing | S1, S2 | pass |
| C2 | "Attempted delivery" counts; sender chooses waiver or signature; Hold for Pickup returned if not picked up within 5 days with the count worded differently | S1, S3, S4 | pass |
| C3 | Sources and dates (May 22, 2026; no date; Oct 11, 2023; May 19, 2026) | S1 to S4 | pass |
| C4 | "fastest domestic shipping service"; 7 days a week, 365 days a year, "with limited exceptions"; 6 PM time is local at the recipient's address; Sunday and holiday delivery in many major markets for an additional fee | S1, S2 | pass |
| C5 | Mail at Post Office, station or branch, Contract Postal Unit, collection box, hand to carrier, Package Pickup or Pickup on Demand; 70 pounds; 108 inches combined length and girth | S1, S2 | pass |
| C6 | Time of day of acceptance and other factors; Service Commitments tool results; Scheduled Delivery Day basis; footnote 2; "found on your receipt" | S1, S2 | pass |
| C7 | Three scan events and "This is not a complete list"; the refund section repeats that other events also meet the commitment | S1 | pass |
| C8 | Waiver: sender, at mailing, cannot be changed in transit, carrier signs and leaves in a secure location if secured and weather-protected, five days then returned, not with additional insurance, COD or COD Restricted Delivery, voids loss claims, claims remain for damage, missing contents, service failures | S3 | pass |
| C9 | Signature Required: Label 11-F on or after January 2012, "signature required" box, signature image, item can be left if not checked, required for COD, COD Restricted Delivery, additional insurance | S3 | pass |
| C10 | Hold for Pickup (PME FAQ): in place of carrier delivery, five postal business days, retail locations and kiosks, cremated remains excluded, notifications, second notice after 3 days, final after 5 calendar days, no Sunday or holiday fee | S1 | pass |
| C11 | Hold for Pickup FAQ: identification, no fee, another notification at 3 days and return at 5 days for PME, eligible methods, exclusions | S4 | pass |
| C12 | Refund: three cases, postage and Sunday or holiday premium, sender asks, no sooner than 2 days and no later than 30 (60 with an Extra Service), online or PS Form 3533, appeal online within 30 days | S1 | pass |
| C13 | Exceptions list (six bullets, "not complete") | S1 | pass (last bullet: "refund requested other than for loss" for items to or from Alaska, Hawaii, Guam, American Samoa, the Northern Mariana Islands, or to Palau, the Marshall Islands, Micronesia; the FAQ text for this item was read in two pieces) |
| C14 | Insurance: USPS.com says most shipments include insurance, with restrictions and DMM references; waiver FAQ ties loss claims to signature | S2, S3 | pass (no amount given) |
| C15 | Differences: refund window (S2 30 days, S1 adds 2 and 60); Hold for Pickup days; 7 days a week against markets; age of the signature FAQ | S1 to S4 | pass |
| C16 | Not said: markets, complete scan list, receipt format, cutoff handling | S1 to S4 | pass (absence checks) |

## Image checks
PNG 1200 x 3372 px, 626,204 bytes, SHA-256 prefix `40c306f03a8354f4`; SVG 5,919 bytes, `3dffbcc000ba3564`; md 13,726 bytes, `1030473f21a0f457`; C2PA chunk and metadata stripped on the device (hashes equal the originals). The rendering script printed no text past the right margin; the PNG was viewed. Diagram text only repeats facts from the article; alt text (891 characters) matches the front matter and the Markdown alt text.

## Open points for Gate 2
1. Is the refund section (about 330 words) too close to post 147? It is limited to what the FAQ states.
2. The Hold for Pickup difference ("five postal business days" against "5 days"): fair, or too strong?
3. The sixth exception bullet is a compressed paraphrase of a long FAQ item.
4. Five internal links: acceptable?

## Not checked
WordPress draft, editor, mobile, live page, publication slot. Search volume: not checked (Trends relative only). Two older quick drafts in WordPress (post 153 and 168) are not used.
