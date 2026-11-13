# QA record — how-to-address-an-envelope-usps

Article: `content/drafts/how-to-address-an-envelope-usps.md` (draft, 2026-11-13; about 1,400 body words without the alt texts; one H1, nine H2 sections; one table of 3 columns; two images).
Brief: `research/briefs/how-to-address-an-envelope-usps.md`. Sources: `research/sources/how-to-address-an-envelope-usps.md` (S1 USPS FAQ 000008202; S2 USPS.com letters page; S3 USPS.com popup; S4 USPS video transcript; S5 USPS.com packages page, step 4; none shows an update date).
Stage: **published 2026-11-13** (Gate 1 by Claude; Gate 2 FIX on `a2f1755` applied in `fbdf9b3`, re-check PASS on `fbdf9b3`; see the sections below). **Rule-type post: re-read the five sources before any later republish.**

## Scope

Where the return address, delivery address and postage go; line by line format; capitals, punctuation and abbreviations; the return address rules; packages and labels; postcards; the letters page's special address notes. No postage prices (the letters page lists some), automation discounts, barcode areas, precanceled stamps, Periodicals, nonprofit mail, international addressing or other carriers.

## Method

After drafting, all five sources were opened again (2026-11-13; the popup and the transcript were fetched as text) and tested by script after normalization: S1 21 of 21 phrases; S2 18 of 18; S3 5 of 5; S4 14 of 14; S5 3 of 3. Absence tests: the transcript has no "capital", "caps", "upper case", "lower case", "comma" or "period" and no date; the popup has no "capital" and no date; S1 has no update date and no inch or distance-from-the-edge measure; S2 and S5 show no "last updated"; S2 lists postage prices on the page and the draft has no `$` (none used). Internal link checked: the Forever stamp post returns 200 (title matches); the new slug returns 404. 27 articles are live.

## Gate 1 — Factual QA (claim by claim)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | Return address: top left corner (letters page); upper-left corner on the front (popup); "above and to the left of" the recipient's address (transcript) | S2; S3; S4 | pass |
| C2 | Delivery address: "center of envelope" (FAQ); "bottom center" (letters page); "in the center" (transcript); parallel to the longest side (popup) | S1; S2; S4; S3 | pass |
| C3 | Postage: upper right corner (FAQ) | S1 | pass |
| C4 | The pages do not give a distance from the edge | S1; S2; S3; S4 | pass (absence tested for inch measures) |
| C5 | Letters page lists four lines for both blocks (name or company, apartment or suite, full street address, city, state and ZIP+4) on separate lines | S2 | pass |
| C6 | FAQ prefers the apartment, suite, room or floor number on the street line after the street address or on the line above, "not below"; transcript: same line | S1; S4 | pass |
| C7 | Two-letter state abbreviations; ZIP+4 "if known" otherwise ZIP; Look Up a ZIP Code tool (transcript); missing ZIP "causes unnecessary delay because it will require manual look-up"; directionals "always use applicable" (FAQ) and "are required" (transcript) | S1; S4 | pass |
| C8 | FAQ: "Use all CAPS, spaces between words, no punctuation, and left justify the margin"; 10, 12 or 14 point for typed or printed addresses | S1 | pass |
| C9 | Letters page: capital letters, pen or permanent marker, no commas or periods, ZIP+4 whenever possible | S2 | pass |
| C10 | Transcript: write legibly, scanners "can decipher most handwriting styles and printed font types," avoid red pen or smearing ink, print labels if you can; no mention of capital letters | S4 (absence tested) | pass |
| C11 | Abbreviations: FAQ "always use applicable abbreviated locators"; transcript: shortened forms can be used, "writing the words is encouraged" | S1; S4 | pass |
| C12 | Return address: FAQ "Always use a return address" (first guideline); transcript "a requirement"; FAQ also "required on certain types of mail" and the DMM list | S1; S4 | pass |
| C13 | Dec. 14, 2023 rule: no longer accepting domestic items with a foreign return address; a foreign address only for international shipping with a customs form | S1 | pass |
| C14 | Popup: address, return address and postage on the same side; improperly addressed package "might get returned to you"; USPS.com package page: parallel to the longest side, same side, a printed label can replace a separate address label, same side, do not bend, fold or overlap | S3; S5 | pass |
| C15 | Postcards: delivery address in the space provided, on the same side as the message and the stamp | S2 | pass |
| C16 | Puerto Rico URB on four lines; Virgin Islands "VI"; APO/FPO/DPO in another country: no city or country name, include unit and box numbers if assigned; links to more details not read | S2 | pass |
| C17 | None of the five pages shows an update date; the FAQ gives none at all | S1 to S5 (absence tested) | pass |
| C18 | FAQ mixes in mailer rules (automation discounts, barcode areas, precanceled stamps, Periodicals, nonprofit mail), left out | S1 | pass |
| C19 | No page says what happens with lowercase or punctuation; the popup says only that an improperly addressed package might be returned | S1 to S5 | pass |

## Image checks

800 px wide SVG, 1200 px wide PNG (scale 1.5), render check printed `[]`, viewed in crops. Alt text equals the front-matter alt and describes every card. C2PA metadata stripped on the device; SHA-256 and sizes equal the originals (PNG 447,558 bytes; SVG 3,697 bytes). The "Letters and formatting" card says the FAQ and the letters page ask for capital letters and "no commas or periods": the FAQ's own wording is "no punctuation", which includes both.

## Format

One H1, H2 sections only, a single 3-column table (mobile-safe), prose with a bulleted list only for Sources, meta description 145 characters, no prices.

## Open points for Gate 2

- Confirm that the apartment number paragraph reads as a source difference (FAQ: same line preferred, line above allowed; letters page: its own line above) and not as a recommendation.
- Confirm the "always" against "required on certain types of mail" paragraph is shown without resolving.
- Dated rule post: re-read the five pages right before publishing; report before publishing if the placement, apartment, capitals, return address or foreign return address wording changed.

## Gate 2 FIX on `a2f1755` (applied 2026-11-13)

1. **ZIP+4 read as required.** The lead answer and the diagram's "Line by line" card said "ZIP+4". The FAQ says: "Use a ZIP+4 ZIP Code (if known) on last line following city and state. Otherwise, use the ZIP Code." (S1, tested again). Fix: the lead now says "city, state and ZIP Code, using ZIP+4 if you know it"; the diagram card reads "state and ZIP Code (ZIP+4 if you know it)"; the front-matter alt and the body alt were changed together and are equal (checked by script); the line-by-line paragraph quotes the letters page's "whenever possible" and says the FAQ's instruction when ZIP+4 is not known is the five-digit ZIP Code. The letters page's four-line list is still described as the letters page's own wording.
2. **Fictional example added.** New section "A fictional example" and a second image, `assets/optimized/how-to-address-an-envelope-usps-example.png` (800 px SVG, 1200 px PNG, render check `[]`, viewed; C2PA stripped, hashes verified: PNG 174,620 bytes, SVG 2,542 bytes; the main diagram is now PNG 457,398 and SVG 3,782 bytes). It shows made-up names and addresses (Jane Sample, John Example; Anytown NY; Othertown CA): return address top left, stamp upper right, delivery address in the center, capital letters, no punctuation, two-letter states, the apartment number on the street line after the street address. Each element is traced to S1: center, upper right postage, all CAPS and no punctuation, two-letter state, apartment on the same line after the street address, ZIP+4 if known and otherwise the ZIP Code; the return address in the top left is from S2 and S3. The text also says the letters page puts the apartment number on its own line above the street and the delivery address "bottom center". The second ZIP Code in the example is five digits on purpose and the image says so. No real person or address is intended; no price is shown. Front matter now has `image_2` and `image_2_alt` (body alt equals front-matter alt for both images).
Changed parts only: the lead, the line-by-line and ZIP paragraphs, the new example section, the main diagram card, both alt texts, and the example image. Re-read the five pages right before publishing.

## Publication record (2026-11-13)

Moved to `content/ready/` after the Gate 2 PASS on `fbdf9b3`. WordPress: media 121 (main diagram) and 122 (fictional example), both with alt equal to the front-matter alt (`image_alt`, `image_2_alt`, checked); post 124 created as a draft (category 6; comments and pingbacks closed; Rank Math description and focus keyword `how to address an envelope` set). The body was generated by script from the draft on `main` (12,540 characters, 30 block comments) and matched the local Python conversion by SHA-256 (`71f18b24...`); both images were fetched from `main` and matched the repository hashes before upload. Editor check: 27 blocks (2 images), none invalid; Rank Math keyword and description read back. Phone preview at 375 px (table 315 px wide, images 315 px, no page overflow) and 320 px (table 260 px, images 260 px, no overflow, table font 11 px); the fictional example stays legible at 320 px. **Re-read right before publishing:** FAQ 21 of 21 (text length 3,813, no date), letters page 18 of 18, popup 5 of 5, video transcript 14 of 14 (still no mention of capital letters), package page 3 of 3; no update date on any page; no change and no conflict. Published 2026-11-13 03:13 UTC.
Live QA (logged out): 200; canonical equals the URL; title and meta description equal the draft; Open Graph title, description and image present; robots index, follow; one JSON-LD block with a BlogPosting; one H1; no comment form or pingback link; both image SHA-256 values equal the repository (`923e79c4...`, `0c24863d...`) and the live alts are the front-matter alts; key sentences present (the ZIP+4 lead, the "A fictional example" section, the FAQ capital letters quote, the five-digit ZIP sentence; the name Jane Sample appears in the prose and in the image alt, and the all-capitals JANE SAMPLE only in the alt text and the image); the Forever stamp link returns 200; the post is in `/post-sitemap.xml`, `/feed/`, the home page and the category page; 29 posts total. No indexing request. Search volume was never checked; Trends relative indexes only.
