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
