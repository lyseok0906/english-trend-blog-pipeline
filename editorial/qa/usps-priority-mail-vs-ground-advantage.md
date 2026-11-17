# QA record — usps-priority-mail-vs-ground-advantage

Article: `content/drafts/usps-priority-mail-vs-ground-advantage.md` (draft, 2026-11-17; about 1,320 body words (after Gate 2 FIX) without the alt text; one H1, six H2 sections; no table).
Brief: `research/briefs/usps-priority-mail-vs-ground-advantage.md`. Sources: `research/sources/usps-priority-mail-vs-ground-advantage.md` (S1 USPS.com Priority Mail, S2 USPS.com Ground Advantage, S3 USPS.com Shipping Insurance and Delivery Services; none shows an update date).
Stage: **published 2026-11-17 (post 135).** Rule-type post: re-read the three pages right before any publishing.

## Scope

What the three USPS.com pages say about Priority Mail and USPS Ground Advantage: delivery-time wording and footnotes, size and weight, packaging, included insurance and conditions, tracking, pickup, one-page-only lines, what the pages do not say. No prices, Priority Mail Express, business options, international mail or recommendation.

## Method

After drafting, the three pages were opened again in the built-in browser (2026-11-17) and tested by script after normalization (apostrophes and quotes removed, dashes unified, ® and ™ removed, footnote digits after words removed, asterisks removed, lowercase): S1 30 of 30 phrases, S2 25 of 25, S3 11 of 11. Absence tests: S2 text (footnotes included) has no "money-back", no "guarantee", no "drop-off"; none of the three pages shows "last updated", "updated on", "last modified" or "revised". The article text has no `$` except $100 (included insurance, as a coverage amount) and $5,000 (additional coverage, as a coverage amount); no postage or fee amount. Internal links 200: pickup, holiday deadlines, tracking status, Certified Mail, Missing Mail (live check, logged out). The new slug returns 404 now (not live); `post-sitemap.xml` lists 31 posts and not the new one.

## Gate 1 — Factual QA (claim by claim)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | Priority Mail page: "2-3 Days"; service includes tracking and delivery in 2-3 days | S1 | pass |
| C2 | Footnote: the expected delivery date on the receipt or at checkout "in most cases" reflects 2-3 days and is based on origin, destination and drop-off time; it "does not come with a money-back guarantee" | S1 | pass |
| C3 | The page points to the USPS Service Standards Map for estimates | S1 | pass |
| C4 | Ground Advantage page: "Packages in 2–5 Days"; footnote "Expected delivery in 2–5 days"; slower service possible to certain places (including Alaska, Hawaii and offshore destinations) or with hazardous materials | S2 | pass |
| C5 | The Ground Advantage page does not say how much slower, does not mention a guarantee either way, does not say where the date is shown or that it depends on drop-off time | S2 (absence tested: no "money-back", "guarantee", "drop-off") | pass |
| C6 | Maximum weight 70 lbs on both; combined length and girth 108 inches (Priority Mail) and 130 inches (Ground Advantage) | S1; S2 | pass |
| C7 | Priority Mail Flat Rate products "let you ship packages up to 70 lbs to any state at the same price"; Flat Rate envelopes or boxes in standard sizes; own box priced by weight and zone | S1 | pass |
| C8 | Ground Advantage: own packaging, measure it; price tiers up to 4, 8, 12 and 15.999 oz then by the pound rounded up; a large First-Class Mail envelope over 15" long, 12" high or 3/4" thick, rigid, or not uniformly thick pays the Ground Advantage price | S2 | pass |
| C9 | Both pages give the same dimensional-weight rule (over 1 cubic foot, divide by 139); both list handling fees for live animals or perishable items such as food or plants; the nonstandard-fee lists are not the same (amounts differ, not given); Flat Rate packaging is exempt from nonstandard fees (Priority Mail page) | S1; S2 | pass |
| C10 | Priority Mail page: "Includes USPS Tracking and up to $100 of insurance with most shipments (restrictions apply)"; Ground Advantage page: "$100 insurance is included (for both outbound and return shipments)" and up to $5,000 additional coverage for merchandise | S1; S2 | pass |
| C11 | Priority Mail footnotes: insurance available only for certain products and destinations; does not cover certain items; DMM 609.4.3, 609 and 503.4; domestic shipments need the applicable USPS Tracking barcode; not included for Open & Distribute, Premium Forwarding Service-Residential or -Commercial; additional insurance replaces the included insurance | S1 | pass |
| C12 | Insurance page: both services' domestic shipments must have an applicable USPS Tracking barcode to qualify; Priority Mail insurance not included with certain extra services (not named); chart footnote: maximum liability of $100 with an IMpb or USPS retail tracking barcode "and the mailer pays retail or commercial prices" | S3 | pass |
| C13 | The DMM rule "no insurance coverage is provided when purchasing Certified Mail, except for Priority Mail pieces with included insurance" is reported from our published Certified Mail article, not re-read in the DMM today | published article (DMM and FAQ read 2026-11-04) | pass (carried over; attributed to our article) |
| C14 | Tracking included in both; Priority Mail page excludes Prepaid Forever Priority Mail Flat Rate from tracking; no page says whether those packages get included insurance | S1; S2; S3 | pass (absence reasoned from the three pages; not searched for an explicit statement elsewhere) |
| C15 | Keep the postmarked mailing receipt and proof of value in case you need to file a claim | S3 | pass |
| C16 | Both pages list free Package Pickup at home or office; our Package Pickup article says the FAQ lists Priority Mail and USPS Ground Advantage as eligible | S1; S2; published pickup article | pass |
| C17 | Priority Mail "no surcharges for fuel; residential or rural delivery; or Saturday delivery"; the footnote on the Saturday part concerns Priority Mail Express (no conclusion drawn) | S1 | pass |
| C18 | Ground Advantage "includes forwarding, undeliverable as addressed (UAA), and return to sender (RTS) at no additional cost"; the Priority Mail page has no such line | S2; S1 (absence reasoned) | pass |
| C19 | Ground Advantage is the "primary option" for HAZMAT only mailable by ground, with a zero handling fee; the Priority Mail page lists a HAZMAT handling fee | S2; S1 | pass |
| C20 | Ground Advantage page calls itself "our best-priced service for items up to 15.999 oz"; no cost comparison made | S2 | pass |
| C21 | No update date on any of the three pages; no Ground Advantage FAQ article found (404 and empty FAQ search); DMM 503.4 not read | S1; S2; S3; research notes | pass |

## Image checks

800 px wide SVG, 1200 px wide PNG (scale 1.5), render check printed `[]` (no text beyond 745 px), viewed in crops. Six cards (delivery time; size and weight; insurance and tracking; both pages; hazardous materials; not stated) and a two-line footer ("Prices are not shown"). The insurance card was reworded after the first render so that "both need a USPS Tracking barcode" is attributed to the insurance page, not to both product pages. Alt text equals the front-matter alt and describes every card. C2PA metadata stripped on the device; SHA-256 prefix and sizes equal the originals (PNG 566,849 bytes `bc4a20b27732e420`; SVG 4,344 bytes `21e6959c3afab0c4`).

## Format

One H1 in the body, H2 sections only, prose with a bulleted list only for Sources, no table, meta description 151 characters (target 150 to 156). Focus keyword `priority mail vs ground advantage`.

## Open points for Gate 2

- Confirm the Delivery time section reads as "page is silent", not "no guarantee", for Ground Advantage.
- Confirm the insurance section attributes each condition to the right page (Priority Mail footnotes against the insurance page) and does not state anything about Prepaid Forever insurance.
- Confirm that $100 and $5,000 are acceptable as coverage amounts under "no prices".
- Link plan: the article does not link to the claims article because that article is not published; after both are published, a link between them can be added in a small edit (see the claims QA record).
- Dated rule post: re-read the three pages right before publishing; report before publishing if the delivery-time wording, size limits, insurance wording or pickup and tracking lines changed.

## Gate 2 FIX on `745ec39` (applied 2026-11-17)

1. **Expected, not fixed, delivery times.** The reviewer noted that the diagram and alt showed only "2-3 days" and "2–5 days". The diagram card and the alt now say "expected 2-3 days" and "expected 2-5 days", keep the Priority Mail "no money-back guarantee" line and the Ground Advantage "slower to Alaska, Hawaii, offshore places or with hazardous materials" line, and end with "Both are expected times". The lead sentence and the meta description (now 151 characters, "expected delivery of 2-3 days ... and 2-5 days") say "expected"; the Delivery time section adds that both pages word the time as an expected delivery, so the article reads the numbers as expected times, not fixed delivery times. The Ground Advantage page stays described as silent on a guarantee.
2. **Insurance card.** Retitled "Included insurance, with conditions"; it keeps "up to $100" for Priority Mail ("most shipments"), "$100 is included" for Ground Advantage, the Tracking barcode condition attributed to the insurance page, and "up to $5,000" as the most that can be bought. Alt matches.
3. **DMM 503 sentence.** Read directly by Claude on 2026-11-17 (pe.usps.com/text/dmm300/503.htm): "Except for Priority Mail pieces with included insurance, no insurance coverage is provided when purchasing Certified Mail." The article now quotes it from the DMM and links the Certified Mail article for the service; DMM 503 is added to Sources, and the text says only that sentence of section 503 (not 503.4) was read. The reviewer's own check of the same text is consistent with this. Claim C13 is now verified in the DMM, not carried over.
4. **Prices.** The reviewer confirmed $100 and $5,000 as coverage limits fit "no prices"; they still appear only as limits.

Changed parts only: the lead, meta description, Delivery time paragraph, the Certified Mail sentence in Insurance and tracking, the "What the pages do not say" scope sentence, Sources, the diagram card texts and the alt. Image after the change: PNG 578,060 bytes `6106ebc912e21b9b`, SVG 4,390 bytes `69375b562faffc94` (C2PA stripped; render check `[]`, crops viewed). Not published.

## Gate 2 re-check on `754b40d`: PASS (2026-11-17)

The reviewer passed the changed parts and asked to continue with the usual procedure.

## Publication record (2026-11-17)

Moved to `content/ready/` (status ready) after the Gate 2 PASS. Right before publishing, the three USPS pages (Priority Mail, Ground Advantage, Shipping Insurance and Delivery Services) were re-read in the built-in browser: page text lengths equal the earlier read the same day (11,552, 7,658 and 15,569 characters), the Priority Mail phrase test 30 of 30, the Ground Advantage test 25 of 25 (still no "money-back", "guarantee" or "drop-off"), the insurance page 9 of 9, no update date on any page; no change, so the post was published as agreed.
WordPress: the body was generated by script from the reviewed draft on `main` (SHA-256 of the output equals the Python converter's, `3a0f8ffe...`), the PNG hash was compared with the repository (`6106ebc9...`), media 134 (alt equals the front-matter alt, checked; the image block uses the original file, not the -scaled copy), post 135 created as a draft (category 6, Postal service and stamps; comments and pingbacks closed; Rank Math description and focus keyword `priority mail vs ground advantage` set). Editor check: 24 blocks, none invalid, Rank Math description and keyword read back. Preview at 375 and 320 px: no sideways scroll (scrollWidth equals the window width), image 315 and 260 px wide. Published 2026-11-17 (post 135).
Live QA (logged out): 200; canonical equals the URL; title and meta description (151 characters) equal the draft; Open Graph title, description and image present; robots index, follow; one JSON-LD block with a BlogPosting; one H1; no comment form or pingback link; image SHA-256 equals the repository and the live alt is the front-matter alt; 12 key sentences present (expected 2-3 days, no money-back guarantee, 2–5 days, slower service, 108 and 130 inches, insurance wording, DMM 503 sentence, Prepaid Forever, best-priced line); only $100 and $5,000 as dollar amounts; five internal links 200 (holiday deadlines, Certified Mail, tracking status, Missing Mail, Package Pickup); listed in `/post-sitemap.xml`, `/feed/`, `/` and `/category/postal-service-and-stamps/`; 32 posts live (`x-wp-total` 32).
Link to the USPS claims article: added after that article was published (see below).

## Link to the USPS claims article (2026-11-17, after its publication)

Link-only edit on the user's instruction, applied to the repository file and to WordPress post 135: the last sentence of "Insurance and tracking" now ends "...covers the search for lost mail, and our USPS claims article compares what USPS pages say about filing a claim." Checked logged out: one link to `/usps-claim-how-it-works/` (200), title and meta description unchanged, editor check 24 blocks, 0 invalid. No fact changed.
