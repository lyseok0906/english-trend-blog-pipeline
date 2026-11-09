# QA record — usps-package-intercept-how-it-works

Article: `content/drafts/usps-package-intercept-how-it-works.md` (draft, 2026-11-09; about 1,750 words including the sources list; one H1, nine H2 sections; one table).
Brief: `research/briefs/usps-package-intercept-how-it-works.md`. Sources: `research/sources/usps-package-intercept-how-it-works.md` (S1 USPS.com "Package Intercept", no update date; S2 USPS FAQ "USPS Package Intercept - The Basics", dated Oct. 27, 2026; S3 USPS terms page, "Updated: 7/15/2016").
Stage: **draft, Gate 1 (Claude) done 2026-11-09.** Gate 2 (ChatGPT by the user), ready, WordPress and publication are not done.

## Scope

Only what the three pages state: who can request, eligible and not eligible items, retail request steps, return to sender and Hold for Pickup, 7 business days, no guarantee, no edit or cancel, when charges apply, relabeling and postage by class, extra services, Registered Mail, and the differences between the pages. **No fee or postage amount** (S1 shows a dollar figure; not used), no commercial intercept steps, no Notice 123, no Form 1509, no international mail, no claims or lost-mail advice.

## Method

After drafting, all three pages were opened again in the built-in browser (2026-11-09) and tested by script after normalization (apostrophes, quotation marks, dashes, trademark signs, whitespace, lower case): S1 27 phrases (all present; one only differed by a space left where a registered-trademark sign was removed), S2 about 45 phrases (all present; the seven-class list matched when read as separate list items), S3 9 phrases (all present). Absence tests: S1 has no update date and no "recipient", "108 inches", "7 business" or "1509"; S2 has no dollar amount and no wording about a request by the recipient; S3 has no dollar amount.

**One finding at Gate 1:** S2 has a note that only USPS Ground Advantage and Parcel Select oversized-priced items are greater than 108 inches, but not more than 130 inches. The draft first said only the terms page gives 108 inches. Fixed: the eligibility section, the differences table and the closing sentence now carry the note; the diagram line "The 2016 terms page says 108 inches, not 130" is still accurate. **Second fix:** the FAQ relabel table says Bound Printed Matter, Media Mail and Library Mail items are relabeled as Priority Mail and charged Priority Mail commercial postage, also when redirected to the sender; the draft now says so.

## Gate 1 — Factual QA (claim by claim)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | Fee-based; the sender or authorized representative asks USPS to stop or redirect an item not out for delivery or already delivered | S1; S2 | pass |
| C2 | Not guaranteed; request active 7 business days; cannot be edited or cancelled; fees charged when the item is intercepted, none if it is not (USPS.com); the FAQ's "only if an intercept was possible" is kept as FAQ wording in the fees section | S1; S2 | pass (reworded at Gate 2 round 1) |
| C3 | The pages describe requests by the sender or representative or agent, not by the recipient (absence tested) | S1; S2 | pass |
| C4 | Retail senders: return to own address or Hold For Pickup; online only with a USPS.com account | S1 | pass |
| C5 | Commercial senders: own address, new delivery address or Hold For Pickup via Business Customer Gateway; new address only commercial per the FAQ | S1; S2 | pass |
| C6 | Most domestic mailings with a tracking or extra services barcode are eligible; length plus girth not larger than 130 inches | S1; S2 | pass |
| C7 | FAQ note: only Ground Advantage and Parcel Select oversized-priced items measure more than 108 and up to 130 inches | S2 | pass (added at Gate 1) |
| C8 | Recipient and sender both domestic; APO, FPO, DPO excluded | S2 | pass |
| C9 | Tracking numbers beginning 92 or 93: commercial mailer only, Business Customer Gateway; USPS.com retail intercept cannot be used | S2 | pass |
| C10 | FAQ: verify eligibility with USPS Tracking or the eligibility checker on USPS.com | S2 | pass |
| C11 | USPS.com not-eligible list (Marketing Mail and periodicals; Commercial Mailing Receiving Agency; PO Box; nonmailable, surface-only such as Label 127 or Surface Mail Only, hazardous materials such as Consumer Commodity ORM-D) | S1 | pass |
| C12 | FAQ ineligible list (international, APO/FPO/DPO, customs declaration label, surface-only with Limited Quantity, Consumer Commodity or ORM-D markings, no tracking barcode) | S2 | pass |
| C13 | Four retail steps; estimated total is intercept fee plus estimated postage if applicable; USPS then attempts to intercept and redirect | S1 | pass |
| C14 | Intercepted at the delivery Post Office; returned to sender or Hold for Pickup, not to a PO Box; tracking continues under the original number | S2 | pass |
| C15 | Every attempt to locate during the 7 days; no guarantee before delivery; can prevent delivery only while not out for delivery or delivered | S2 | pass |
| C16 | No amounts; both USPS.com and the FAQ point to a price page (USPS.com links Notice 123; the FAQ has a "price information" item) | S1; S2 | pass |
| C17 | Charges: S1 not charged if not intercepted, fee non-refundable if successful; S2 pay all fees only if an intercept was possible, no charge if delivered first, fee per mailpiece; S3 fees and postage only upon a successful intercept | S1; S2; S3 | pass |
| C18 | FAQ sentences on charges "or otherwise" collected from the recipient or by a USPS carrier at delivery, not explained; article does not reconcile | S2 | pass (unreconciled, stated) |
| C19 | USPS.com: redirected as the original service (Priority Mail Express, Priority Mail, USPS Ground Advantage, First-Class Mail); pay applicable postage | S1 | pass |
| C20 | FAQ: Priority Mail Express, Priority Mail, USPS Ground Advantage to sender not relabeled, no additional postage; to Hold for Pickup relabeled as a new item of the same class at the commercial price | S2 | pass |
| C21 | FAQ: Bound Printed Matter, Media Mail, Library Mail relabeled as new Priority Mail items at Priority Mail commercial postage; separate lines for Parcel Select | S2 | pass (fixed at Gate 1) |
| C22 | USPS.com extra services: Adult Signature Required, Adult Signature Restricted Delivery, Signature Confirmation, insurance | S1 | pass |
| C23 | FAQ: those three when redirected to a new address or Hold for Pickup; insurance only if the original shipment had it, original value | S2 | pass |
| C24 | Registered Mail: only when redirected to sender; original number; not relabeled or repackaged; "Withdrawn" on the receipt, sign, surrender; terms page also says return to sender only | S2; S3 | pass |
| C25 | Differences table: mail classes (S1 names four services and excludes Marketing Mail and periodicals; S2 lists seven classes without First-Class Mail, absence tested; S3 all except Standard Mail and Periodicals) | S1; S2; S3 | pass |
| C26 | Differences table: size 130 / 130 with the 108 note / 108; postage as original service / by class / Priority Mail rate | S1; S2; S3 | pass |
| C27 | Dates: S1 no date, S2 Oct. 27, 2026, S3 "Updated: 7/15/2016"; all read 2026-11-09; no price | S1; S2; S3 | pass (absence tested) |

## Image check

| # | Item | Result |
|---|---|---|
| I1 | Card 1 "Who and what": fee-based, sender or representative, not out for delivery or delivered, tracking or extra services barcode, 130 inches matches C1, C6 | pass |
| I2 | Card 2 "Request": retail online with USPS.com account, check eligibility, return to sender or Hold for Pickup, not a PO Box, estimated total matches C4, C13, C14 | pass |
| I3 | Card 3 "Wait": 7 business days, not guaranteed, cannot be edited or cancelled matches C2 | pass |
| I4 | Card 4 "Charges": USPS.com: if the item is intercepted, the fee plus any applicable postage is charged; if not intercepted, no charge; fee nonrefundable; no amounts matches C16, C17 | pass (redrawn at Gate 2 round 1) |
| I5 | Not-eligible card matches C11, C12 (labelled "as USPS lists"); "The pages differ" card matches C26 | pass |
| I6 | Alt text (1,213 characters after Gate 2 round 1) in front matter and body is identical and says the same as the diagram | pass |
| I7 | Files `assets/raw/usps-package-intercept-how-it-works.svg` and `assets/optimized/usps-package-intercept-how-it-works.png` (1200 x 3234, sha256 eadc3ce5...3fd4; Gate 1 version was 1200 x 3096, a607d5ed...de6c) in the repository; no logos or photos; text 25 to 46 px on an 800 px canvas; no text past the right margin | pass |

## Format

Title 60 characters; slug `usps-package-intercept-how-it-works`; meta description 155 characters; the focus keyword `how does usps package intercept work` appears word for word in the title only; one H1; plain markdown table (4 columns, check on a phone at the WordPress preview); no prices.

## Open points

- **P1 (differences):** mail classes, 108 vs 130 inches, postage by class and the FAQ's carrier-collection sentences are shown as differences, not resolved.
- **P2 (old page):** the terms page is dated 2016; the article calls it the oldest and does not say which page controls.
- **P3 (demand):** the phrase is probably urgent how-do-I-stop-my-package searching; the article promises nothing and gives no fee. Relative Trends index only.
- **P4 (length):** about 1,750 words; the long sentences on relabeling by class could be shortened at Gate 2 if wanted.
- **P5 (table on phones):** the four-column table with long cells needs the 375 and 320 px check.

## Result and next step

Gate 1: **PASS** (27 of 27 claims, 7 of 7 image checks; two fixes made during Gate 1). Next: push, Gate 2 by commit SHA. After a Gate 2 PASS: ready, WordPress draft, phone preview, re-read of all three USPS pages right before publishing, publish if unchanged, live QA and records.

## Gate 2 round 1 (base `1dd0826`): FIX applied 2026-11-09

**Finding (ChatGPT):** the lead, diagram and alt summarized the charges as "fees apply only if an intercept was possible", which is the FAQ's wording and is less clear than USPS's main guidance. **Fix:** say that if the shipment is intercepted, the fee plus any applicable postage is charged, and that customers are not charged if it is not intercepted.

**Source re-read (USPS.com page, 2026-11-09, after the finding):** "If the shipment is intercepted, your credit card will be charged the [amount] Package Intercept fee plus any applicable postage. If the actual postage is greater than estimated, any additional postage will be charged accordingly." and "Customers will not be charged if the shipment was not intercepted. If successfully intercepted, the non-refundable Package Intercept fee is applied to each intercept request." The amount on the page is not used. The terms page says fees and postage are charged only upon a successful intercept (read at Gate 1).

**Changed parts and comparison:**

| Place | New wording | Matches source | Result |
|---|---|---|---|
| Lead paragraph | USPS.com says that if the shipment is intercepted, the Package Intercept fee plus any applicable postage is charged, while customers are not charged if the shipment was not intercepted | USPS.com page | pass |
| Section "Fees and postage", charges paragraph | Card is charged the fee plus any applicable postage if intercepted; additional postage if actual postage is greater than the estimate; not charged if not intercepted; fee non-refundable if the intercept succeeds; FAQ and terms-page sentences unchanged and still attributed | USPS.com page; FAQ; terms page | pass |
| Alt text (front matter and body identical) | Step 4: USPS.com says that if the item is intercepted, the fee plus any applicable postage is charged, that customers are not charged if it is not intercepted, and that the fee is nonrefundable | USPS.com page | pass |
| Diagram card 4 | "USPS.com: if the item is intercepted, the fee plus any applicable postage is charged. If not intercepted, no charge. The fee is nonrefundable. No amounts here; USPS has a price page." | USPS.com page | pass |
| Diagram versus body versus alt | Same meaning; no text past the right margin; PNG and SVG read back from the repository | | pass |

Nothing else was changed. The unreconciled FAQ sentences about collection at delivery are still stated as a limit.

## Gate 2 re-check, WordPress, publication and live QA (2026-11-09)

**Gate 2 re-check (ChatGPT, base `f09fe67`): PASS**, no further changes requested on charges. Moved to `content/ready/` (`status: ready`).

**WordPress draft:** post 95, media 94. The PNG was fetched from GitHub main and verified (sha256 eadc3ce5...3fd4, 536,179 bytes) before upload; WordPress made a `-scaled` copy (950 x 2560) because the image is tall, so the post uses the original file URL and the served original was verified with the same hash. Content hash verified in the browser before posting (5b30d4cb...). Category 6 (Postal service and stamps); comments and pings closed; Rank Math focus keyword `how does usps package intercept work` and the 155-character description set and read back in the editor; 32 blocks, none invalid.

**Phone check of the four-column table** (table font `clamp(11px, 3.2vw, 18px)`, as set for the razor post): at 375 px the table fits its box (315 px, 12 px text, smallest cell 72 px), no sideways scroll, page scrollWidth 375. At 320 px the table is 278 px in a 260 px box, so the last column ("Terms page") is cut off and the box scrolls sideways; the page itself does not overflow (scrollWidth 320) and the diagram fits (260 px). Accepted as before (the table scrolls inside its own box).

**Sources re-read right before publishing (2026-11-09):** USPS.com page: all 28 tested phrases present, including the charge sentences used in the fix; price link to Notice 123 present; no update date; no 108 or 7 business days wording. FAQ: dated Oct 27, 2026; all tested phrases present (the seven-class list matched when read as list items; First-Class Mail not in the list; the 108-inch note present; no dollar amount). Terms page: 9 of 9 phrases present, "Updated: 7/15/2016", no dollar amount. No change and no new conflict beyond the differences the article already shows.

**Published:** 2026-11-09 01:15:16 UTC, https://statesideexplained.com/usps-package-intercept-how-it-works/ .

**Live QA (logged out, no cache):** 200; canonical correct; title; meta description (155 characters) and og tags (og description identical); robots index, follow; JSON-LD includes BlogPosting and WebPage; one H1; no comment form, no pingback; image served from the original upload with sha256 identical to the repository PNG, alt 1,213 characters; the three USPS source links present; no dollar amount in the article text; table style `clamp(11px, 3.2vw, 18px)`; in `/post-sitemap.xml`, `/feed/`, the home page and the Postal service and stamps category page.

