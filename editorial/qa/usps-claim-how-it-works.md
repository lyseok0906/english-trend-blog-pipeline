# QA record — usps-claim-how-it-works

Article: `content/drafts/usps-claim-how-it-works.md` (draft, 2026-11-17; about 1,930 body words without the alt text; one H1, nine H2 sections; one table of 3 columns and 10 rows).
Brief: `research/briefs/usps-claim-how-it-works.md`. Sources: `research/sources/usps-claim-how-it-works.md` (S1 USPS.com "File a Claim", no update date; S2 USPS FAQ 000006089, Nov 6, 2026; S3 DMM 609, no date; S4 USPS.com insurance page, two lines).
Stage: **draft, Gate 1 done by Claude; waiting for Gate 2.** Rule-type post: re-read the claims page, the FAQ and DMM 609 right before any publishing.

## Scope

How USPS sources say a domestic insurance claim works: who can file, damaged or missing contents against lost, the per-service filing chart, whether insurance is needed, documents and case exceptions, how to file, decision and payment time, appeals, postage and insurance fee, nonpayable and special cases. No amounts, payment caps or fees; no international or bulk claims; the Missing Mail search is left to the published Missing Mail article.

## Method

After drafting, the pages were opened again in the built-in browser (2026-11-17) and tested by script after normalization (apostrophes and quotes removed, dashes unified, ® and ™ and asterisks removed, lowercase): S1 52 of 52 phrases, S2 44 of 44, S3 26 of 27 (the miss, "no insurance coverage is provided", is the DMM 503 rule that the article attributes to our published Certified Mail article, which read it on 2026-11-04; it is not in section 609), S4 11 of 11 (shared with the Ground Advantage QA). Absence tests: S1 has no "deleted after", "10 items", "Consumer Advocate", "photocopy" or 2026 date; S3 has no "usps ground advantage 15 days 60 days" and no "priority mail 15 days 60 days" (domestic Ground Advantage has no row; "USPS Ground Advantage — Retail" appears only in the APO/FPO/DPO row); no page shows "last updated", "updated on", "last modified" or "revised" (the DMM text contains "issued", from unrelated sentences). The article text has no `$`, no fee or cap amount. Internal links 200: Missing Mail, Certified Mail, tracking status (live check, logged out). The new slug returns 404 now (not live); `post-sitemap.xml` lists 31 posts and not the new one.

## Gate 1 — Factual QA (claim by claim)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | Damaged or missing contents: file immediately, no later than 60 days from (after) the mailing date | S1; S2; S3 | pass |
| C2 | Lost item: file within the time period for the service; chart gives a "File After" or "No Sooner Than" day and a "File Before" or "No Later Than" day, counted from the mailing date; filing period is based on the mailing date on the receipt | S1; S2 | pass |
| C3 | Chart rows: Priority Mail Express 7 and 60; Priority Mail Express COD, Priority Mail, USPS Ground Advantage, Insured Mail, COD, Registered Mail and Registered COD 15 and 60; APO/FPO Priority Mail Express Military 21 days and 180 days; APO/FPO/DPO Insured and Registered 45 days and 1 year; surface only 75 days and 1 year (days after mailing, years as written) | S1; S2 | pass (rows compared line by line; S3 chart agrees where it has a row) |
| C4 | The DMM chart lumps "Insured Mail (including Priority Mail under 503.4.2)" and has no separate domestic Ground Advantage row; USPS.com and the FAQ list Priority Mail and Ground Advantage separately with the same numbers | S3 (absence tested); S1; S2 | pass |
| C5 | FAQ asterisk: bulk claims through the Business Customer Gateway no sooner than 15 days (three rows marked) | S2 | pass |
| C6 | Insurance page: for Priority Mail and Ground Advantage a lost item "no later than 60 days from the date of mailing", no opening day | S4 | pass |
| C7 | The pages do not say why a lost-item claim cannot be filed sooner or when an item counts as lost | S1; S2; S3 (absence reasoned) | pass |
| C8 | Who can file: USPS.com quote (sender or recipient; must have the original mailing receipt); FAQ (mailer or addressee; recipient keeps article and container; first approved claimant is paid) | S1; S2 | pass |
| C9 | DMM 1.3: damaged or missing: either; lost: either with the original retail mailing receipt or the online label record or printout; only the account holder for insured USPS Returns packages; only the mailer when the mailer added and paid for insurance on USPS Returns packages; only the mailer for insured or COD parcels paid using USPS Ship | S3 | pass |
| C10 | FAQ: claims without a mailing receipt can be filed but payment may be limited; DMM: if only the outer packaging is submitted, indemnity can be limited; both give dollar limits, not repeated | S2; S3 | pass |
| C11 | Eligible items (Priority Mail Express and other insured mail, COD, Registered Mail with insurance); insurance may be included or bought | S1 | pass |
| C12 | Priority Mail and Ground Advantage include insurance when the domestic shipment has an applicable USPS Tracking barcode (amount not given in the article) | S4 | pass |
| C13 | The DMM Certified Mail rule is reported from our published Certified Mail article | published article | pass (carried over; attributed) |
| C14 | Uninsured items: USPS "may not legally pay compensation for uninsured lost or damaged articles"; Missing Mail Search for missing or delayed uninsured mail; FAQ: unable to honor requests to be compensated | S1; S2 | pass |
| C15 | What to have ready: tracking or label number (13 to 34 characters; where found), evidence of insurance (three kinds), proof of value (list), proof of damage (photos, repair estimate) | S1 | pass |
| C16 | Save packaging and contents; do not throw out damaged items after photographing them; do not reship undamaged items; may be asked to take the package to a Post Office | S1 | pass |
| C17 | Receipt difference: USPS.com "the original mailing receipt"; DMM photocopy acceptable for insured and COD mail | S1; S3 | pass |
| C18 | Online label record: USPS.com lists it as evidence of insurance; the DMM requires tracking number, postage, insurance fee, declared value, mailing date, origin and delivery ZIP Codes, plus a postmarked receipt or an electronic acceptance scan followed by an acceptance or physical scan as evidence of mailing | S1; S3 | pass |
| C19 | Mailed claim with several extra services: original receipts for all (DMM 1.5.2) | S3 | pass |
| C20 | Addressee must keep container, damaged articles, packaging and contents; on written request make them available; failure results in denial (FAQ and DMM) | S2; S3 | pass |
| C21 | How to file: online fastest and easiest, free account, save to finish later; paper form by phone; FAQ: up to 10 items under one tracking number, proof of value and insurance required, saved claims deleted after 3 days; USPS.com gives no deletion period | S1; S2 | pass (absence tested) |
| C22 | Decision usually within 5-10 days (USPS.com); FAQ same plus up to 30 days for in-depth claims such as high claim amounts; payment in 7-10 business days; USPS does not pay more than actual value; letter lists the reasons; partial approval or denial | S1; S2 | pass |
| C23 | Appeals: USPS.com 30 days "of receiving the decision" and second appeal 30 days "of the date you received the appeal denial"; FAQ 30 days "of the date of the original decision" and final appeal to the Consumer Advocate 30 days "of the date of the second denial"; whether "receiving" and "date of" mean the same day is not stated | S1; S2 | pass |
| C24 | FAQ: postage reimbursement included with payment if the item was lost or not delivered; insurance fees not reimbursed; USPS.com sends postage and fee refunds to a separate page not read | S2; S1 | pass |
| C25 | DMM nonpayable examples (six) and FAQ special cases (airline tickets, gift cards and similar, cash lower limit with Registered Mail excepted, checks not cash, collectibles by receipt) | S3; S2 | pass |
| C26 | USPS.com instructions "do not include all the details and exceptions"; no update date on USPS.com or DMM; no approval rate; section 609 only was read in the DMM | S1; S3 | pass |

## Image checks

800 px wide SVG, 1200 px wide PNG (scale 1.5), render check printed `[]` (no text beyond 745 px), viewed in crops. Five cards (who can file; damaged or missing contents; lost item by days after mailing; have ready; after you file) and a three-line footer ("No amounts or fees are shown"). Alt text equals the front-matter alt and describes every card. C2PA metadata stripped on the device; SHA-256 prefix and sizes equal the originals (PNG 431,387 bytes `e38696403ba4f078`; SVG 3,569 bytes `0c6527ae9a3e09a9`).

## Format

One H1 in the body, H2 sections only, a single 3-column table (mobile-safe, post-only table font at publishing), prose with a bulleted list only for Sources, meta description 155 characters. Focus keyword `usps claim`. The article is long (about 1,930 words) because it compares three sources; Gate 2 may ask to trim the "Cases that are limited or not paid" section.

## Link back from the Missing Mail article (decision needed at Gate 2)

The user asked that the two posts be linked to each other. This post links to the published Missing Mail article. The published Missing Mail article does not link here. Proposed after Gate 2 PASS and after this post is published: a link-only edit to the "Claims and refunds" section and Sources note of `content/ready/usps-missing-mail-search-how-it-works.md` and the WordPress post 123 (no change of facts), reported before applying. Not done now because it changes a published post.

## Open points for Gate 2

- Confirm the receipt and online-label differences read as source differences, not advice on what to do without a receipt.
- Confirm that omitting every dollar limit (insured amounts, caps without a receipt or with outer packaging only, cash) is the right reading of "no prices".
- Confirm the appeal paragraph shows the two 30-day wordings without choosing one.
- Decide whether to trim the nonpayable and special-cases section, and approve the proposed link-only edit to the Missing Mail article.
- Dated rule post: re-read the claims page, the FAQ and DMM 609 right before publishing; report before publishing if the chart, the who-can-file wording, the evidence rules or the appeal wording changed.
