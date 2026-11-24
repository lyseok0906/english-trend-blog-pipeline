# QA record — usps-priority-mail-express-how-it-works

Article: `content/drafts/usps-priority-mail-express-how-it-works.md` (draft, 2026-11-24, about 1,900 words in the body, one H1, nine H2 sections including Sources; meta description 146 characters; alt text 1,128 characters after Gate 2 round 2).
Brief: `research/briefs/usps-priority-mail-express-how-it-works.md`. Sources: `research/sources/usps-priority-mail-express-how-it-works.md` (S1 to S4, read 2026-11-24).
Stage: draft. Gate 1 (Claude) run on 2026-11-24. **Gate 2 round 1 (ChatGPT, base `f839045`, user-reported 2026-11-24): FIX, two items, applied 2026-11-24** (section "Gate 2 FIX round 1"); **Gate 2 round 2 (ChatGPT, base `ee58248`, user-reported 2026-11-24): FIX, one item (Service Commitments tool and receipt roles), applied 2026-11-24** (section "Gate 2 FIX round 2"); Gate 2 round 3 (changed part only) not yet run. Backlog row 43.

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
After round 1: PNG 1200 x 3648 px, 696,273 bytes, SHA-256 prefix `2c00d8340b38aa9b`; SVG 6,607 bytes, `4d81bdbb66b80f0f`; md 14,575 bytes, `77c8384bf0e42e97`; alt text 1,100 characters (first version: PNG 3372 px, `40c306f03a8354f4`; SVG `3dffbcc000ba3564`; md `1030473f21a0f457`; alt 891); C2PA chunk and metadata stripped on the device (hashes equal the originals). The rendering script printed no text past the right margin; the PNG was viewed. Diagram text only repeats facts from the article; alt text (891 characters) matches the front matter and the Markdown alt text.

## Open points for Gate 2
1. Is the refund section (about 330 words) too close to post 147? It is limited to what the FAQ states.
2. The Hold for Pickup difference ("five postal business days" against "5 days"): fair, or too strong?
3. The sixth exception bullet is a compressed paraphrase of a long FAQ item.
4. Five internal links: acceptable?

## Not checked
WordPress draft, editor, mobile, live page, publication slot. Search volume: not checked (Trends relative only). Two older quick drafts in WordPress (post 153 and 168) are not used.

## Gate 2 FIX round 1 (2026-11-24, base `f839045`): applied

Reviewer result: two items. (1) The diagram's Waiver of Signature card put "the carrier leaves the item" and "returned if not claimed in 5 days" in one line, so an item already left in a secure place could look as if it is returned after 5 days; delivered-by-leaving and not-claimed-and-held had to be separated. (2) The lead and the diagram's opening card should not let the money-back guarantee read as automatic for every shipment: the conditions and exceptions should sit close to it.

Applied: (1) body: with a waiver the carrier signs and leaves the item in a secure location where the area is secured and protected from weather, and an item left that way has been delivered; separately, in the same paragraph, the FAQ says an item not claimed within five days by the recipient is returned to the sender; the article says the FAQ does not say whether that return applies to an item left in a secure location or only to one that could not be left. Diagram card 2 and the alt text say the same (carrier signs and leaves the item where the area is secured and weather-protected; "separately, the FAQ says an item not claimed within 5 days is returned"). (2) the lead now says whether a given shipment has the guarantee is shown when it is mailed (the FAQ says the Service Commitments tool shows whether USPS can offer one) and that exceptions apply; diagram card 1 and the alt text carry the same condition. The rest of the article is unchanged, including the refund exceptions list, the Hold for Pickup section and the Where the pages differ section.

The Waiver of Signature FAQ wording was re-checked against the earlier read of the page (same paragraph: carrier signs and leaves; "If the item is not claimed within five days by the Recipient, it will be returned to the Sender"). Nothing is published; Gate 2 round 2 is needed.

## Gate 2 FIX round 2 (2026-11-24, base `ee58248`): applied

Finding: the diagram and alt text said the Service Commitments tool and the receipt show whether the guarantee can be offered. The FAQ supports two separate things: the Service Commitments tool shows whether USPS can offer the money-back guarantee for a shipment, and the receipt carries the delivery commitment; the FAQ does not say the receipt shows guarantee availability. The lead sentence "whether a given shipment has the guarantee is shown when it is mailed" had the same scope problem.

Applied: (1) lead: "The FAQ says the Service Commitments tool shows whether USPS can offer the money-back guarantee for a shipment, that the delivery commitment is found on the receipt, and that exceptions apply." (2) diagram card 1: "The Service Commitments tool shows whether USPS can offer the guarantee; the receipt shows the commitment. Exceptions apply." (3) alt text (front matter and body): "the Service Commitments tool shows whether USPS can offer the guarantee for a shipment, the receipt shows the delivery commitment, and exceptions apply". The rest of the article is unchanged.

Image checks after round 2: PNG 1200 x 3717 px, 706,385 bytes, SHA-256 prefix `ed83c481c8b1b4e4`; SVG 6,733 bytes, `2a43479b0829a8d2`; md 14,654 bytes, `0568d850c7efcdf7`; alt text 1,128 characters; meta description 146 characters; no dollar sign or percent sign; C2PA chunk and metadata stripped on the device (hashes equal the originals); the rendering script printed no text past the right margin; the PNG was viewed. Nothing is published; Gate 2 round 3 (changed part only) is needed.
