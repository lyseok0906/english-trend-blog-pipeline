# QA record — usps-package-pickup-how-it-works

Article: `content/drafts/usps-package-pickup-how-it-works.md` (draft, 2026-11-09; about 1,670 body words; one H1, eight H2 sections; one table).
Brief: `research/briefs/usps-package-pickup-how-it-works.md`. Sources: `research/sources/usps-package-pickup-how-it-works.md` (S1 USPS FAQ "Package Pickup & Pickup on Demand", no update date; S2 USPS.com "How to Prepare & Send a Package", no update date; S3 USPS.com "Schedule a Pickup" form page, no update date; S4 Notice 123, linked only).
Stage: **draft, Gate 1 (Claude) done 2026-11-09.** Gate 2 (ChatGPT by the user), ready, WordPress and publication are not done.

## Scope

What the three USPS pages say about Package Pickup and Pickup on Demand: what is eligible, postage and the 10-ounce rule, size and hazards, addresses, scheduling, changing, leaving the package, and what to do if the pickup fails. No prices or fee amounts (Notice 123 is linked, no amount read or used), no international detail beyond the FAQ notes, no business mailers or USPS Connect, no statement about whether Media Mail can be picked up.

## Method

After drafting, the pages were opened again in the built-in browser (2026-11-09; FAQ accordions read after about 4.5 seconds) and tested by script after normalization (apostrophes, quotation marks, dashes, trademark signs, whitespace, lower case): the FAQ 71 of 71 phrases (one fixed at this step: the draft had left out "properly prepared for pickup"; restored); the USPS.com packages page 10 of 10; the Schedule a Pickup page 1 of 1. Absence tests: the FAQ has no "media mail" and no "library mail"; none of the three pages shows an update date (the "Last Updated" words on the scheduling page belong to a form field about a dog). Notice 123 loads; no amount used. Internal link checked: the Media Mail post returns 200; the new slug returns 404 (unpublished, no clash). 23 articles are live.

## Gate 1 — Factual QA (claim by claim)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | Three options for outgoing mail: Pickup on Demand, Package Pickup, Collection Service (prepaid mail in a collection box or handed to a carrier or postal employee) | S1 | pass |
| C2 | Package Pickup is free regardless of the number of items; next delivery day or a designated day, at the time the carrier delivers mail; can occur at any time on the scheduled date | S1 | pass |
| C3 | Schedule, edit or cancel Package Pickup Monday to Saturday until 2:00 AM Central Time on the day; the modify note says "before 2:00 am" without a zone (difference shown, not resolved) | S1 | pass |
| C4 | Pickup on Demand: fee per trip regardless of items; two-hour window; typically within two hours of the scheduled pickup time; schedule, edit or cancel until 5:00 AM local time; fees in Notice 123 under Domestic - Other Services and Fees | S1; S4 | pass |
| C5 | Each item up to 70 pounds and 130 inches in total length and girth | S1 | pass |
| C6 | The carrier can only pick up packages with prepaid postage, or return merchandise, eligible for the free or the paid service | S1 | pass |
| C7 | Package Pickup list: Priority Mail Express, Priority Mail, USPS Ground Advantage, Returns, International Priority Mail Express, International Priority Mail, First-Class Package International Service; other classes such as First-Class Mail items may be picked up if combined with a listed product | S1 | pass |
| C8 | Pickup on Demand adds USPS Connect Local, Package Service parcels, and Priority Mail Express and Priority Mail Open and Distribute shipments | S1 | pass |
| C9 | Media Mail is not named on the list; the article does not say whether Media Mail can be picked up | S1 | pass (absence tested) |
| C10 | Priority Mail Express guarantee needs presentation to an acceptance employee at a Post Office; contact the local Post Office for guarantee details | S1 | pass |
| C11 | International packages can be picked up only if label, customs forms and postage were completed online; hand-written customs forms mean a Post Office retail location | S1 | pass |
| C12 | Sufficient postage before pickup; online options (Click-N-Ship, PC Postage, postage meters); six valid ways to prepay as listed | S1 | pass |
| C13 | Stamps only on items of 10 oz or less and 1/2 inch or less in thickness; heavier or thicker stamped pieces go to a retail counter | S1 | pass |
| C14 | USPS.com: a stamped package over the limits left in a mailbox is left by the carrier; in a blue collection box it is returned; with Click-N-Ship or kiosk postage any drop-off method works; free pickup request listed | S2 | pass |
| C15 | The carrier is not required to verify postage; offices follow standard revenue protection practices if a package appears underpaid | S1 | pass |
| C16 | Hazardous materials must meet DMM or IMM standards; includes fragile items without proper packaging and liquid items | S1 | pass |
| C17 | Not all addresses are eligible; the scheduling page says it verifies the address; the pages do not list ineligible addresses | S1; S3 | pass (absence tested) |
| C18 | Weekend or holiday request is picked up on the next scheduled delivery day (Saturday afternoon for Monday example); up to 6 months ahead; login for future and repeat requests (daily, weekly, monthly within six months) | S1 | pass |
| C19 | Package locations listed; multi-story buildings: ground level, secured location; carrier discretion; snow, ice, obstructed pathways and dogs may prevent a pickup; no need to be present if postage-paid, properly prepared for pickup and left in a safe location | S1 | pass |
| C20 | Modify or cancel through "Modify an Existing Pickup" with confirmation number and email or phone; modifiable: date, location, number of packages, total weight; same-day volume or weight increase: call the local Post Office | S1 | pass |
| C21 | Confirmation email or carrier notice; if not collected the notice says why; delivery status for Priority Mail Express or packages with USPS Tracking or Signature Confirmation | S1 | pass |
| C22 | If the pickup does not happen: contact the local Post Office, file a service request (Email Us > Where is my Mail?); Pickup on Demand refunds can be requested online if service was not performed per its features | S1 | pass |
| C23 | None of the three pages shows an update date; the pages do not give the carrier arrival time or the Pickup on Demand fee | S1; S2; S3 | pass (absence tested) |
| C24 | Table: Package Pickup and Pickup on Demand columns match C2 to C4, C7, C8 | S1 | pass |

## Image check

| # | Item | Result |
|---|---|---|
| I1 | "Package Pickup (free)" card matches C2, C3 | pass |
| I2 | "Pickup on Demand (fee)" card: fee per trip, Notice 123, two-hour window, until 5:00 AM local time, no amount matches C4 | pass |
| I3 | "Limits" card: 70 lb, 130 in, not all addresses, prepaid postage, stamps 10 oz and 1/2 inch matches C5, C12, C13, C17 | pass |
| I4 | "After you schedule" card: up to six months, leave where you chose, need not be present, snow, ice, paths, dogs matches C18, C19 | pass |
| I5 | Footer "Sources: USPS FAQ, USPS.com, Schedule a Pickup; no update dates; read Nov. 9, 2026" matches C23 | pass |
| I6 | Alt text (1,001 characters) in front matter and body is identical and says the same as the diagram | pass |
| I7 | Files `assets/raw/usps-package-pickup-how-it-works.svg` and `assets/optimized/usps-package-pickup-how-it-works.png` (1200 x 2355, 404,283 bytes, sha256 1bdbb4fc1522cfeb31deadbdde770bc21f8a9886e7623cdcf596b4c2c754f2d8) in the repository; no logos or photos; no text past the right margin (render check printed an empty list) | pass |

## Format

Title 57 characters; slug `usps-package-pickup-how-it-works`; meta description 152 characters; focus keyword `usps package pickup` appears in the title; one H1; plain markdown table with three columns; one internal link (Media Mail post); no prices.

## Open points

- **P1 (cutoff wording):** the FAQ gives "2:00 AM Central Time" in one place and "before 2:00 am" in the modify note. Shown, not resolved.
- **P2 (no update dates):** none of the pages is dated; the article says so and gives the read date.
- **P3 (demand):** only Google Trends relative indexes were measured; search volume was not checked (`docs/next-candidates-2026-11-09.md`).
- **P4 (re-check):** rule-type post; re-read the FAQ, the USPS.com packages page and the scheduling page right before approval and before publishing, and report first if a limit, cutoff or eligibility list changed.

## Gate 2 FIX round 1 (base `5010b89`, applied 2026-11-09) — changed parts only

**Gate 2 requests:** (1) the 10 oz and 1/2 inch limit must carry the DMM condition that postage is paid only with stamps, in body, diagram and alt; (2) the wording on hazardous materials and on liquid and fragile items must match the official sources.

**What changed:** the scope paragraph now names DMM sections 116, 126, 136 and 601; the section "Postage and the 10-ounce rule" now gives the DMM rule (items bearing only postage stamps, over 10 ounces or over one half-inch thick, may not be picked up in normal delivery and collection or through Pickup on Demand; the sender presents them at a Post Office; improperly presented items are returned; section 126 says precluded from pickup service), names the classes of the three sections read (Priority Mail Express, Priority Mail, retail First-Class Mail and USPS Ground Advantage), says the article does not cover other classes, notes the FAQ's "or" sentence and that the article follows the DMM wording, and keeps the USPS.com note on mailbox and blue box and on Click-N-Ship or kiosk postage; the section "Size, hazards and addresses" no longer says fragile or liquid items are hazardous: it quotes the FAQ's two sentences, says the FAQ does not define hazardous materials or say whether fragile or liquid items count as hazardous, and gives DMM 601 3.1.1, 3.4 and 3.6 as the separate rules, without saying what a carrier refuses at a pickup; "What the pages do not say" and the sources list updated (DMM 116, 126, 136, 601). Diagram rebuilt (Limits card with the stamps-only condition; new card "Hazardous, fragile, liquid"; footer names the DMM sections). Alt rewritten (1,482 characters, identical in front matter and body).

**Method:** DMM 116 3 of 3, DMM 126 3 of 3, DMM 136 3 of 3, DMM 601 5 of 5 phrases tested after normalization on 2026-11-09 (all pass); FAQ phrases re-read (the "or" sentence, the prepay list item, the fragile and liquid sentence). Absence tests: DMM 116, 126 and 136 show no date; DMM 601 shows 7-12-26 in the text and 4-6-26 on section 3.4. Details in `research/sources/usps-package-pickup-how-it-works.md` (P17 to P20).

| # | Changed claim | Source | Result |
|---|---|---|---|
| F1 | DMM 116 1.0, 126 1.2 and 136 1.0: items bearing only postage stamps as postage payment and weighing more than 10 ounces or measuring more than one half-inch in thickness may not be picked up in normal delivery and collection of mail or through Pickup on Demand (126: precluded from pickup service); the sender presents them at a Post Office or retail counter | S5; S6; S7 | pass |
| F2 | DMM 116 and 136: improperly presented items are returned to the sender | S5; S7 | pass |
| F3 | The three sections cover Priority Mail Express, Priority Mail, and retail First-Class Mail and USPS Ground Advantage; the article reads those sections only | S5; S6; S7 | pass |
| F4 | FAQ: one sentence reads "10 oz or less or 1/2-inch or less"; the prepay list reads "10 oz or less and 1/2-inch in thickness or less"; DMM wording is "more than 10 ounces, or more than one half-inch" | S1; S5-S7 | pass |
| F5 | FAQ: hazardous materials must meet DMM or IMM standards; next sentence "This includes items that contain anything fragile without proper packaging or liquid items"; the FAQ does not define hazardous materials or say whether fragile or liquid items count as hazardous | S1 | pass (absence tested) |
| F6 | DMM 601: package to withstand normal transit and handling and cushion fragile items (3.1.1); liquid marked on the outer container with orientation arrows, primary containers closed with screw-on caps of at least one and one-half turns, soldering, clips or similar means (3.4); perishable, hazardous, biological or restricted materials subject to PUB 52 (3.6); presented as mailing standards, not as pickup refusal rules | S8 | pass |
| F7 | USPS.com: stamped package over the limits left in a mailbox is left by the carrier, in a blue collection box is returned; Click-N-Ship or kiosk postage allows any drop-off method (unchanged text, now placed after the DMM rule; the DMM wording covers items bearing only postage stamps) | S2; S5-S7 | pass |

Earlier claim rows C1 to C24 other than C12, C13, C14 and C16 are unchanged; those four are replaced by F1 to F7. Image checks I3 and I5 are superseded by the image check below.

**Image check (round 1):** Limits card matches F1 and C5, C12, C17 (70 pounds, 130 inches, prepaid postage, not all addresses eligible, the stamps-only condition, take it to a Post Office per the DMM); "Hazardous, fragile, liquid" card matches F5 and F6; footer names USPS FAQ and USPS.com (no update dates) and DMM 116, 126, 136, 601. Files in the repository: `assets/optimized/usps-package-pickup-how-it-works.png` 1200 x 3003, 534,992 bytes, sha256 94933849510023818db53b65aadfdb7fae95b6453468ed8fdac2b71f8f561e51 (equal to the render); `assets/raw/usps-package-pickup-how-it-works.svg` 4,189 bytes. Render check printed an empty list. Alt equals body alt (1,482 characters).

**Open points after the FIX:** P1 (cutoff wording), P2 (no update dates on the three USPS pages and DMM 116, 126, 136), P3 (demand) and P4 (re-check) unchanged. New: P5, the FAQ's fragile and liquid sentence is ambiguous; the article shows it and the DMM rules and does not decide what a carrier refuses.

## Publication and live QA (2026-11-09)

Gate 2 re-check on `8fbce79` = PASS (user-reported). Moved to `content/ready/` (front matter `status: ready`; text unchanged). WordPress draft post 109, media 108 (original file URL used in the image block; alt saved on the media item; category Postal service and stamps; comments and pings closed; Rank Math description and focus keyword `usps package pickup` set). Editor check: 29 blocks, none invalid. Phone preview: at 375 px the three-column table fits (315 px, 12 px font); at 320 px it fits (260 px, 11 px font); no page overflow (post-only table font `clamp(11px, 3.2vw, 18px)`).

**Right before publishing**, the USPS FAQ (24 phrases, including the "10 oz or less or 1/2-inch or less" sentence, the prepay list item and the fragile and liquid sentence), the USPS.com packages page (10 phrases), the Schedule a Pickup page, DMM 116, 126 and 136 (3 phrases each), DMM 601 (6 phrases including the 3.4 mark) and Notice 123 (loads) were re-read and tested after normalization: 0 missing. Absence tests held (the FAQ has no "media mail" or "library mail" and no update date; the USPS.com page shows no update date; DMM 116, 126 and 136 show no date; DMM 601 shows 7-12-26 and 4-6-26). No change and no new conflict, so the post was published directly under the standing rule: **2026-11-09 05:30:47 UTC** (post 109).

**Live QA (logged out):** https://statesideexplained.com/usps-package-pickup-how-it-works/ returns 200; canonical correct; title and 152-character meta description and Open Graph description match; robots index, follow; JSON-LD types present; one H1, nine H2, one table; no comment form and no pingback link; image returns 200, 534,992 bytes, sha256 equal to the repository file; alt 1,482 characters (equal to the draft); the internal link (Media Mail post) returns 200; the DMM stamps-only sentence, the section 136 reference, the FAQ-does-not-define sentence and the DMM 601 date mark are present in the live text; the post is in `/post-sitemap.xml`, `/feed/`, the home page and the category page. The article gives no price or fee amount. No indexing request.
