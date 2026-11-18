# QA record — usps-refund-how-it-works

Article: `content/drafts/usps-refund-how-it-works.md` (draft, 2026-11-18; about 2,240 words in the body, one H1, nine H2 sections including Sources; two tables; seven internal links).
Brief: `research/briefs/usps-refund-how-it-works.md`. Sources: `research/sources/usps-refund-how-it-works.md` (S1 USPS.com refund page, S2 DMM 604.9, S3 FAQ 000005310, S4 FAQ PO Box 000005315, S5 FAQ claims 000006089).
Stage: **draft, Gate 1 done by Claude 2026-11-18; waiting for Gate 2.** Rule-type post: re-read S1, S2 and S4 right before any publishing.

## Scope as set by the user (2026-11-18)

- Separate the two Click-N-Ship numbers (30 days, 60 days) by application route and condition, checked against the USPS.com page and DMM 604.9.
- Keep refund (money back for postage or fees) and claim (compensation for loss or damage of insured mail) apart.
- Report conflicts with the refund explanations in published posts (section "Comparison with published posts" below).
- No prices, fees or refund percentages; no search volume or Trends figure in the article.

## Method

The USPS.com page and DMM 604 were opened in the built-in browser on 2026-11-18 and every statement the article makes was tested by script after normalization (S1: 50 of 50 phrase checks; S2: 34 of 34, two of them after correcting my phrase to the source's wording). Absence claims were tested by listing occurrences: "10 days" and "10 to 60" on S1 (none), "Click-N-Ship" on S2 (one, in 9.2.5), "update" and date tokens on S1 and S2 (none), "pro-rated" on S4 (none), "change of address" on S1 (none). The three FAQ articles were opened and their dates read (S3 Sep 26, 2024; S4 Nov 13, 2026; S5 Nov 6, 2026). The diagram was rendered (1200 x 2751 PNG) and read on screen. The seven internal links were opened logged out (200). The 2025 notices and all prices are not used.

## Gate 1 — Factual QA (claim by claim)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | A refund is money back for postage or fees paid when no service was rendered, or when more than the lawful price was collected | S2 9.2.1 | pass |
| C2 | DMM windows run from 2 to 60 days after the mailing date | S2 Exhibit 9.2.1 | pass |
| C3 | Three sources: USPS.com page "Request a USPS Refund: Domestic" (no update date), DMM 604.9 (no date), FAQ 000005310 dated Sep 26, 2024, which only points to the USPS.com page | S1 heading; S2; S3 | pass (the browser title of S1 is "Request a Domestic Refund | USPS"; the article uses the on-page heading) |
| C4 | USPS.com sends insured-mail loss, damage and missing-contents claims to the File a Claim page | S1 intro | pass |
| C5 | DMM 604.9.2 points to section 609 for an indemnity claim for loss or damage | S2 9.2 | pass |
| C6 | Claims FAQ: postage reimbursement included with the claim payment if lost or not delivered; insurance fees "are not reimbursed" (reported from our claims article) | S5 ("Postage reimbursements will be included with the claim payment if the item was lost or not delivered. Insurance fees cover the cost of the insurance and are not reimbursed.") | pass |
| C7 | DMM no-refund list includes insured mail, COD, Priority Mail Express insurance and Registered Mail fees after USPS accepts the article | S2 9.2.4 | pass |
| C8 | Priority Mail Express, no extra service: 2 to 30 days after mailing (DMM chart and USPS.com) | S2 chart; S1 | pass |
| C9 | Priority Mail Express with an extra service: 30 to 60 days; one combined request | S2 chart; S1 | pass |
| C10 | Extra services: 30 to 60 days after mailing (chart and USPS.com) | S2 chart; S1 | pass |
| C11 | Postage on other mail: 10 to 60 days, DMM chart only; the USPS.com page does not list this row | S2 chart; S1 has no "10 days" | pass |
| C12 | Priority Mail Express applies online with a free USPS.com account or at a Post Office with PS Form 3533; Part I in duplicate and the original customer copy of Label 11 | S1; S2 9.5.6 | pass |
| C13 | Extra services: online for Certified Mail, Return Receipt, Signature Confirmation (and USPS Tracking for USPS Marketing Mail); otherwise where you paid | S1; S2 9.2.5 | pass |
| C14 | Ordinary postage: PS Form 3533 at a Post Office (DMM 9.2.5; online is limited to Priority Mail Express and the listed extra services) | S2 9.2.5 | pass |
| C15 | PO Box on USPS.com: new unused box online within 30 days of payment; box in use pro-rated at the Post Office where the box is | S1 | pass |
| C16 | Package Intercept and Pickup On Demand: online request; no window on the page | S1 | pass |
| C17 | Pickup On Demand: only if the carrier fails to show up during the specified day; not if the carrier shows up or the request is cancelled after 5 a.m. local time on the pickup day | S1 | pass |
| C18 | Priority Mail Express: guaranteed arrival time on the receipt; one request per tracking number; combine with related extra services | S1 | pass |
| C19 | Click-N-Ship: up to 60 days after the print date; account route (Shipping History, Refund Labels); conditions (not scanned, created within the past 30 days of the print date, no existing request); older label more than 30 and less than 60 days: email the Help Desk with the listed details | S1 | pass |
| C20 | The 30 days belong to the online account route and the 60 days to the older-label email route, both counted from the print date | S1 (reading of C19; the page does not say it in one sentence) | pass, stated as "on the USPS.com page" |
| C21 | "up to 60 days" against "less than 60 days": a small gap in the page's wording | S1 | pass |
| C22 | DMM names Click-N-Ship only once, for the USPS Connect Local Sunday-fee refund applied automatically; no label-refund rule names it | S2 occurrence list (1) | pass |
| C23 | DMM 9.3.10 and 9.3.11: PC Postage indicia, 30 days (with a package identification code, electronically to the provider) and 60 days (without, physically to the provider, from the date in the indicia) | S2 | pass |
| C24 | DMM does not say Click-N-Ship is a PC Postage product; the article does not apply those rules to it | S2 (no such statement) | pass |
| C25 | Meter indicia: 60 days of the date in the indicia (9.3.2), a third separate rule | S2 | pass |
| C26 | What to bring: proof of purchase; tracking number, purchase receipt, photo ID in person; extra services and Priority Mail Express: tracking number and mailing receipt | S1 | pass |
| C27 | DMM evidence rules: keep evidence until resolved; may upload .jpeg, .pdf or .png and give the mailing date; Form 3533 with envelope or wrapper and markings or other evidence | S2 9.2.5 | pass |
| C28 | No refund for postage or extra-service fees when no postmarked or retail receipt or valid acceptance or processing scan exists | S2 9.2.4 | pass |
| C29 | Not refundable: COD etc. after acceptance; unused adhesive stamps (exchange); undeliverable Certified Mail and Signature Confirmation fees with an attempted-delivery scan; Package Intercept per-piece fee once intercepted | S2 9.2.4 | pass |
| C30 | Priority Mail Express exceptions: strike or work stoppage; undeliverable as addressed; held at the addressee's written request; 1-Day shipment mailed Dec 22 to 25 delivered or attempted within 2 business days; non-loss refunds to or from Alaska, Hawaii and some territories | S2 9.5.5 | pass (the DMM text says "delivered or delivery was attempted"; the article says "delivered or attempted") |
| C31 | Payment: online refunds by check by mail; Post Office refunds in cash, check or money order; Click-N-Ship credited to the original payment account; online business refunds by check | S1 | pass |
| C32 | DMM payment: Form 3533 immediate refund in cash or no-fee money order when entitlement is clear and postage is affixed (limit not repeated); otherwise researched, check or credit | S2 9.2.6 | pass |
| C33 | Dispute within 30 days of receiving the decision (USPS.com); online appeals within 30 days of receipt of the denial (DMM); Form 3533 appeals through the postmaster to a manager, no number of days; so for refunds both count from receipt | S1; S2 9.2.5 | pass |
| C34 | Extra-service fees: chart counts from the mailing date; 9.2.4 says less than 30 or more than 60 days from the date the service was purchased | S2 chart and 9.2.4 | pass |
| C35 | PO Box: USPS.com "pro-rated" and 30 days from payment against FAQ table by term, 3-month box not eligible once activated, automatic full refund after 30 days of inactivity; DMM sends PO Box fee refunds to 508.4.6 (not read) | S1; S4; S2 9.6 | pass |
| C36 | Package Intercept fee "may be refundable if the shipment was not intercepted" (USPS.com); not refunded once intercepted (DMM) | S1; S2 9.2.4 | pass |
| C37 | The refund FAQ is a pointer page dated Sep 26, 2024 with no rule of its own | S3 | pass |
| C38 | Processing time given only for Package Intercept and Pickup On Demand among the services covered: normally 2 to 3 business days, longer if more information is needed; credit up to 2 billing cycles; none for Click-N-Ship, extra-service or Priority Mail Express refunds | S1 | pass |
| C39 | No dollar amount or percentage in the article | Body has 0 "$" and no percentage | pass |
| C40 | Internal links return 200: claims, Missing Mail, Certified Mail, PO Box, Package Intercept, Package Pickup, holiday shipping deadlines | Opened logged out | pass |
| C41 | "As of November 18, 2026" and "checked on November 18, 2026" | Read dates | pass |

## Image check

| # | Item | Result |
|---|---|---|
| I1 | Card "Refund: money back" matches C1 | pass |
| I2 | Card "Claim: a different request" matches C4, C5 | pass |
| I3 | Card "When to apply (from mailing date)": Priority Mail Express 2 to 30, with an extra service 30 to 60, extra services 30 to 60, postage on other mail 10 to 60 (DMM chart only) match C8 to C11 | pass |
| I4 | Card "Click-N-Ship label (from print date)": online within 30 days; older label email the Help Desk; page says up to 60 days match C19, C20 | pass |
| I5 | Card "Not refundable (DMM 604.9.2.4)" matches C7, C29 (the card says "DMM 604.9.2.4", the section USPS numbers 9.2.4 under 604) | pass |
| I6 | Footer "Sources: USPS.com refund page, DMM 604.9; read Nov. 18, 2026" | pass |
| I7 | No logos, photos or USPS marks; text 28 to 46 px on an 800 px canvas; no text past the right margin (script check `[]`); footer spacing widened after the first render | pass |
| I8 | Alt text (958 characters) says the same as the diagram and the body (alt equals the body image text) | pass |
| I9 | Files: `assets/optimized/usps-refund-how-it-works.png` (1200 x 2751, 484,090 bytes, sha256 `c5e1bd547cbb5d83...`), `assets/raw/usps-refund-how-it-works.svg` (4,852 bytes, `620417dd6ed41947...`); the C2PA chunk the transfer added was removed on the device and the hashes read back equal the originals | pass |

## Front matter and format

Title 65 characters; slug `usps-refund-how-it-works`; meta description 144 characters; focus keyword `usps refund` appears in the title ("USPS Refunds") and the meta description; category Postal service and stamps; no price. The body is long (about 2,240 words) because the user asked for the Click-N-Ship and refund-against-claim distinctions; if the reviewer wants it shorter, the "Where the sources differ" list and the Priority Mail Express exceptions paragraph are the first to cut.

## Comparison with published posts (the user asked for conflicts to be reported)

No direct contradiction was found. Differences and open points:

1. **PO Box post.** It says USPS.com says you may be eligible for a refund depending on how long you have had the box, and sends readers to the FAQ and DMM. The refund page adds "pro-rated refund for unused time" for boxes in use and "within 30 days of payment" for new boxes; the FAQ (now dated Nov 13, 2026) gives a table by term and an automatic full refund after 30 days of inactivity. The PO Box post does not contradict either, but it does not mention the refund page's wording. The new article shows the difference and does not reconcile it.
2. **Package Intercept post.** It reports that USPS.com says customers are not charged if the shipment was not intercepted and that the fee is non-refundable if the intercept succeeds. The refund page says the fee plus any applicable postage "may be refundable if the shipment was not intercepted." Not a contradiction with the DMM (not refunded once intercepted) but it leaves open what is charged and then refunded when the item is not intercepted; the new article says it does not reconcile.
3. **Certified Mail post.** It says a request can be made 30 to 60 days after the mailing date (FAQ). The DMM chart agrees, but DMM 9.2.4 counts the 30 to 60 days for extra-service fees from the date the service was purchased. Shown in the new article; the Certified Mail post is not wrong.
4. **Package Pickup post.** It says Pickup on Demand refunds can be requested online if the service was not performed according to its service features. The refund page adds the eligibility (carrier does not show up on the specified day; no refund after a cancellation after 5 a.m. local time). Consistent; the new article adds the detail.
5. **Missing Mail post.** It says a service with a money-back guarantee may be refundable and that the claim page covers claims. Consistent.
6. **Claims post.** It says "USPS.com sends postage and fee refunds to a separate page, which this article did not read." Still true as written. It reports the FAQ sentence on postage reimbursement and insurance fees, which matches S5. The claims post gives appeal-clock wording that differs by source; for refunds both USPS.com and the DMM say "receiving" or "receipt".
7. **Holiday shipping deadlines post.** It shows the Priority Mail Express guarantee footnotes (USPS.com lists Puerto Rico among the places where guaranteed-service refunds are no longer processed; the FAQ says "excluding Puerto Rico"; the FAQ note on 1-Day shipments mailed December 22 to 25). DMM 9.5.5 supports the FAQ side: it lists the December 22 to 25 rule and Alaska, Hawaii and some Pacific territories, and does not list Puerto Rico. The post's statement that the pages are not reconciled is still correct; the new article adds the DMM list without taking a side.
8. **Follow-up edits (not applied, need approval after publication):** link-only edit to the claims post at the sentence about the refund page, and to the Missing Mail post and the Certified Mail post if the user wants the new article linked back.

## Open points for Gate 2

- **P1 (Click-N-Ship):** the article reads the 30 days as the online account route and the 60 days as the older-label email route, both from the print date, and says the DMM's own 30 and 60 days are PC Postage rules that do not name Click-N-Ship. Reviewer to confirm the wording is cautious enough.
- **P2 (length):** about 2,240 words; see above.
- **P3 (DMM section names):** USPS cites these as "DMM 604.9.2", "604.9.5" and so on; the article follows that numbering even though the page lists them as 9.2, 9.5 under 604.
- **P4 (before publishing, mandatory):** re-read S1, S2 and S4; if a window, a route or the payment wording changed, report before publishing.

## Result and next step

Gate 1: **PASS** (41 of 41 claims, 9 of 9 image checks). Next: user push, Gate 2 by commit SHA, then approval to move to `ready`; WordPress only after the Gate 2 PASS.
