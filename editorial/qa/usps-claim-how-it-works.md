# QA record — usps-claim-how-it-works

Article: `content/drafts/usps-claim-how-it-works.md` (draft, 2026-11-17; about 2,090 body words (after Gate 2 FIX) without the alt text; one H1, nine H2 sections; one table of 3 columns and 10 rows).
Brief: `research/briefs/usps-claim-how-it-works.md`. Sources: `research/sources/usps-claim-how-it-works.md` (S1 USPS.com "File a Claim", no update date; S2 USPS FAQ 000006089, Nov 6, 2026; S3 DMM 609, no date; S4 USPS.com insurance page, two lines).
Stage: **published 2026-11-17 (post 138, media 137); Gate 2 PASS on `b2340b5`.** Rule-type post: re-read the claims page, the FAQ and DMM 609 right before any publishing.

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

## Link back from the Missing Mail article (applied after publication, see the Publication record)

The user asked that the two posts be linked to each other. This post links to the published Missing Mail article. The published Missing Mail article does not link here. Proposed after Gate 2 PASS and after this post is published: a link-only edit to the "Claims and refunds" section and Sources note of `content/ready/usps-missing-mail-search-how-it-works.md` and the WordPress post 123 (no change of facts), reported before applying. Not done now because it changes a published post.

## Open points for Gate 2

- Confirm the receipt and online-label differences read as source differences, not advice on what to do without a receipt.
- Confirm that omitting every dollar limit (insured amounts, caps without a receipt or with outer packaging only, cash) is the right reading of "no prices".
- Confirm the appeal paragraph shows the two 30-day wordings without choosing one.
- Decide whether to trim the nonpayable and special-cases section, and approve the proposed link-only edit to the Missing Mail article.
- Dated rule post: re-read the claims page, the FAQ and DMM 609 right before publishing; report before publishing if the chart, the who-can-file wording, the evidence rules or the appeal wording changed.

## Gate 2 FIX on `745ec39` (applied 2026-11-17)

1. **"Uninsured items: no claim" card.** The reviewer read it as too broad, because Priority Mail and Ground Advantage can include insurance and need not have it bought separately. The diagram now has an Insurance card ("A claim needs insurance, which some services include; it need not be bought separately. A Missing Mail Search looks for the item; it is not a claim."), and the alt matches. The body (Does the item need insurance?) now separates insurance bought separately from having no insurance at all, quotes USPS.com ("may have been included with the USPS service or purchased separately") and the FAQ ("if insurance is not purchased at the time of mailing" ... "unable to honor any requests to be compensated"), notes that the FAQ also lists Priority Mail and USPS Ground Advantage as including insurance in the price of postage and that the two wordings are not reconciled, says the receipt or label record shows whether the package was insured, and says a Missing Mail Search is a search for the item and not a claim for payment.
2. **Appeal clock.** The After you file card and the alt now say the 30 days are counted from the decision date or from receiving it, that the sources differ, and to check the USPS claims page. The body adds DMM 609.6, read directly by Claude on 2026-11-17: a customer may appeal "within 30 days from the date of the original decision" (6.2) and for the final review "within 30 days" with no start stated (6.3), and links the USPS claims page. The article still does not say which wording applies; it says anyone close to a limit may want to count from the decision date and check the current wording.
3. **Boundary day.** The meta description said "after day 15". It now says "no sooner than day 15 and no later than day 60" (143 characters), the same wording as the FAQ chart, and the lost-item diagram card and alt now say "no sooner than 15 days, no later than 60" for each group and "from 21, 45 or 75 days, up to 180 days or 1 year" for APO/FPO/DPO. The table headers and the lead already used "no sooner than" and "no later than". Checked: no "after day 15" remains anywhere in the article, diagram or alt.
4. **DMM 503 and who checked what.** The Certified Mail sentence was checked on the official DMM text twice on 2026-11-17: by the reviewer through a search tool, and by Claude in the built-in browser (pe.usps.com/text/dmm300/503.htm: "Except for Priority Mail pieces with included insurance, no insurance coverage is provided when purchasing Certified Mail."). The article now quotes DMM 503 directly and lists it in Sources; Claim C13 is verified, not carried over. Only that sentence of section 503 was read.
5. **Length.** The reviewer said the length need not be cut; the section order (When to file, What to have ready) is unchanged and the nonpayable section keeps each source's conditions. The article is now about 2,090 body words after the fixes.

Changed parts only: the meta description, the Does the item need insurance section, the appeals paragraph, the What the sources do not say scope sentence, Sources, the three diagram cards (lost item, insurance, after you file) and the alt. Image after the change: PNG 546,819 bytes `588a59fc84484885`, SVG 4,442 bytes `07c9dfeb39040dd9` (C2PA stripped; render check `[]`, crops viewed). Link-back to the Missing Mail article: approved by the reviewer after both posts are published; to be recorded (location and result) when applied. Not published.

## Gate 2 re-check on `754b40d`: B FIX applied (2026-11-17)

The reviewer passed the appeal-clock and lost-claim wording and asked for the Insurance card and alt sentence "A claim needs insurance" to be limited to the claims it applies to, so that COD and the other listed claim types are not lost, while keeping the "some services include insurance" and Missing Mail Search lines.
- Diagram card "Insurance": "Claims cover insured mail, COD, Registered Mail with insurance and Priority Mail Express. Some services include insurance; it need not be bought separately. A Missing Mail Search looks for the item; it is not a claim." (listed claim types from USPS.com's eligible items and DMM 609.1.1: "insured mail, COD items, Registered Mail with postal insurance, or Priority Mail Express"). The sentence "A claim needs insurance" no longer appears in the diagram, alt or body.
- Alt: same sentence structure. Body (Does the item need insurance?): one sentence added saying the claims described are for those four types and that COD and Registered Mail rules are only touched on; the rest of the section is unchanged.
Image: PNG 574,068 bytes `51da1b630f07cb4e`, SVG 4,570 bytes `e53b69e1ce069eeb` (C2PA stripped; render check `[]`, crop viewed). Changed parts only: the Insurance card, the alt and one sentence of the body. Not published.

## Publication record (2026-11-17)

Gate 2 PASS on `b2340b5`. Moved to `content/ready/` (status ready). Right before publishing, the four USPS sources were re-read in the built-in browser and found unchanged from the Gate 1 text: USPS.com "File a Claim" 7,329 characters (52 of 52 phrases), FAQ 000006089 23,922 characters (44 of 44), DMM 609 22,726 characters (29 of 29; still no domestic Ground Advantage row in the chart) and the insurance page 15,569 characters. No important change, so it was published as agreed.

WordPress: body generated by script from the reviewed draft on `main` (SHA-256 of the output equals the Python converter's); md and PNG hashes equal the repository (PNG `51da1b63...`); media 137 (alt equals the front-matter alt; image block uses the original file URL); category Postal service and stamps; comments and pings closed; Rank Math description (143 characters) and focus keyword `usps claim`. Editor check: 28 blocks, 0 invalid, 0 invalid tables. Mobile preview: 375 px table 315 px and image 314 px; 320 px table 260 px and image 259 px; no sideways scroll. Published 2026-11-17 (post 138).

Live QA (logged out): 200; canonical equals the URL; title and meta description (143 characters) equal the draft; Open Graph title, description and image present; robots index, follow; one JSON-LD block with a BlogPosting; one H1; no comment form or pingback; image src, alt and hash (`51da1b63...`) correct; one table of 10 rows plus a header; key sentences present (no sooner than 15 days, 60 days, both appeal-clock wordings, the DMM 503 Certified Mail sentence, the insurance-limited-to-claim-types sentence, saved claims 3 days); no dollar amounts; internal links return 200; present in `/post-sitemap.xml`, the feed, the home page and the category page; 33 posts live.

## Cross-links applied after publication (link-only edits, no change of facts)

The user asked, after the PASS, to link A and B to each other and to add a B link to the Missing Mail post. Applied to the repository files and to WordPress posts 138, 135 and 123 (content edited by replacing one paragraph string each, asserted to occur once; no `target`, internal links):

| Post | Location | Added text |
|---|---|---|
| B, USPS claims (138) | "Does the item need insurance?", after the sentence on included insurance and tracking statuses | "and our Priority Mail vs. Ground Advantage article compares the two services." |
| A, Priority Mail vs Ground Advantage (135) | "Insurance and tracking", last sentence | "and our USPS claims article compares what USPS pages say about filing a claim." |
| Missing Mail (123) | "Claims and refunds", end of the last paragraph | "Our USPS claims article compares that FAQ with the File a Claim page and section 609 of the Domestic Mail Manual." |

The Missing Mail sentence "which this article did not read" is unchanged and still true for that article. Result, checked logged out: each of the three pages has exactly one link to its partner in the article body (200), page title and meta description unchanged, one H1; editor check of 138, 135 and 123: 28, 24 and 27 blocks, 0 invalid; Rank Math keywords unchanged. The Sources lists were not changed.

## Link to the USPS refunds article (link-only edit, 2026-11-18)

Approved by the user after the refunds post was published (post 147). Place: section "Refunds" paragraph beginning "On refunds" (end of the paragraph). Added sentence: "USPS.com sends postage and fee refunds to a separate page, which this article did not read; our USPS refunds article covers that page and the refund rules in the Domestic Mail Manual." Link target: https://statesideexplained.com/usps-refund-how-it-works/ (anchor "USPS refunds article").

The earlier sentence "which this article did not read" is kept on purpose: it states what this article's own sources covered and stays true. The link sentence only says where the separate page is covered. No claim is made that this article was checked against the refund page.

Checked after the edit: repository file and WordPress raw content carry the same sentence; the link goes to the USPS refunds article (post 147) without a new-window attribute, like the other internal links, and returns 200 logged out; the public page has the paragraph text exactly as in the repository, one refund-article link, one H1, canonical unchanged and no comment form; block editor: 28 blocks, 0 invalid. No other text, source statement, date or checked-state line was changed. Repository: `content/ready/usps-claim-how-it-works.md`; WordPress post 138 edited by REST (one asserted-unique paragraph end replaced).
