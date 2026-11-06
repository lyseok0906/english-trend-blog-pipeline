# QA record — usps-veterans-day-post-office

Article: `content/drafts/usps-veterans-day-post-office.md` (draft, 2026-11-06; about 370 words in the body, one H1, three H2 sections including Sources; one table).
Brief: `research/briefs/usps-veterans-day-post-office.md`. Sources: `research/sources/usps-veterans-day-post-office.md` (S1 USPS national release of Nov. 4, 2026).
Stage: **draft; Gate 1 (Claude) done 2026-11-06; Gate 2 (ChatGPT, base commit `61113c6`) = PASS, reported by the user 2026-11-06.** The move to `ready`, WordPress and publication are not done and need the user's approvals.

## Scope as set by the user (2026-11-06)

- Only the closure on Wednesday, November 11 and the resumption on Thursday, November 12 from the Nov. 4, 2026 release; **Priority Mail Express delivery on the day is not in the notice and is not inferred** (the article says the notice does not say, either way).
- The notice's usps.com and self-service kiosk paragraph, the 2025 notice, the Holidays & events page and other holidays are **not used** in the article.
- No search volume, Trends figure or advice.

## Method

After drafting, the notice page was fetched again in the built-in browser (2026-11-06) and every statement the article makes was tested by script after normalization (6 of 6 phrase checks). The Priority Mail Express and hours statements were tested by listing every occurrence of "Priority Mail Express" and of "deliver" and by searching for times or "hours". The diagram was rendered and read on screen (1200 x 1500 PNG) and its text compared with the notice. The 2025 notice and the other USPS pages were not re-read (already recorded).

## Gate 1 — Factual QA (claim by claim)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | USPS will observe Veterans Day on Wednesday, November 11, 2026 | S1 "will observe Veterans Day on Wednesday, November 11" (year from the release date and the page's "Nov. 4, 2026") | pass |
| C2 | All Post Office locations will be closed | S1 | pass |
| C3 | Regular mail delivery and retail services will resume on Thursday, November 12 | S1 | pass |
| C4 | The statements come from a USPS national release dated November 4, 2026 | S1 page date "Nov. 4, 2026", label "National news", RSS 04 Nov 2026 | pass |
| C5 | Release title "U.S. Postal Service To Observe Veterans Day Holiday, Nov. 11", published in the USPS Newsroom | S1 page title | pass |
| C6 | The notice does not say whether Priority Mail Express will be delivered on November 11, either way | S1: no such sentence; the only "Priority Mail Express" is in the kiosk postage-printing list, which the article does not use and which is not a delivery statement | pass |
| C7 | The notice does not list hours for any individual Post Office | S1: no times or "hours" | pass |
| C8 | Apart from the resumption date, the notice does not describe delivery on November 11 | S1: "deliver" appears only in the resumption sentence and the boilerplate | pass |
| C9 | Weekdays: November 11, 2026 is a Wednesday and November 12 a Thursday | Calendar (also stated by S1) | pass |
| C10 | "As of November 6, 2026" and "checked on November 6, 2026" | Read dates | pass |
| C11 | Source URL | S1 URL opened | pass |

## Image check

| # | Item | Result |
|---|---|---|
| I1 | Card 1: "Wednesday, November 11 / USPS will observe Veterans Day. All Post Office locations will be closed." matches C1, C2 | pass |
| I2 | Card 2: "Thursday, November 12 / Regular mail delivery and retail services will resume." matches C3 | pass |
| I3 | Card 3: "Not in the notice / Whether Priority Mail Express is delivered on November 11: the notice does not say, either way." matches C6 (first version said "does not mention it", which is not exact because the notice mentions Priority Mail Express in the kiosk list; reworded before commit) | pass |
| I4 | Footer "Source: USPS national release, Nov. 4, 2026" matches C4 | pass |
| I5 | No logos, photos or USPS marks; the Closed card uses red and the resume card green, each also labeled in words; text at 28 to 46 px on an 800 px canvas, readable at phone width | pass |
| I6 | Alt text (425 characters) says the same as the diagram and the body; SVG `<title>` the same | pass |
| I7 | Files: `assets/raw/usps-veterans-day-post-office.svg`, `assets/optimized/usps-veterans-day-post-office.png` (1200 x 1500, 217,379 bytes, sha256 17c8537b...c418) read back from the repository | pass |

## Front matter and format

Title 64 characters; slug `usps-veterans-day-post-office`; meta description 145 characters; focus keyword `is the post office open on veterans day` appears word for word in the title only (the first paragraph and the meta description answer the question without repeating the phrase; noted for Gate 2, no change made); one H1; table in plain markdown; no internal link (none natural; decide at Gate 2); no statements about 2025 or other holidays.

## Open points

- **P1 (timing, estimate):** Veterans Day is November 11. Gate 2 and the user's approval are still needed; the site's crawl pace (three newest posts uncrawled about 13 days after publishing, Search Console 2026-10-20) means indexing before the holiday is unlikely. After the holiday the article records what USPS said for 2026 only.
- **P2 (scope):** the article is short because the user limited it to closure and resumption. The usps.com and kiosk paragraph of the notice, the Holidays & events page and the 2025 comparison are available if the user widens the scope.

## Result and next step

Gate 1: **PASS** (11 of 11 claims, 7 of 7 image checks). Next: user push, Gate 2 by commit SHA, then approval to move to `ready`; before publishing, re-read the notice and record the result (mandatory); WordPress only with the user's approval.


## Gate 2 (ChatGPT) — PASS (user-reported 2026-11-06, base commit `61113c6`)

The user reported Gate 2 round 1 as PASS for the article and the diagram at `61113c6`; no FIX items were reported. ChatGPT had said in advance that it would look at the reader's need for the closure and resumption information, the wording that Priority Mail Express delivery is not confirmed in the notice, the title and keyword, and the diagram on a phone, and that it would not force the keyword into the first paragraph. Nothing in the article, diagram or alt text was changed after Gate 1.

## Move to `ready` — approval requested

The article stays in `content/drafts/` with `status: draft` until the user approves the move. After approval: move the file to `content/ready/`, set `status: ready`, then prepare the WordPress draft and the mobile preview (the user publishes). **Before publishing (the user's condition):** only check whether USPS's national release of Nov. 4, 2026 changed (page text of the three relied-on sentences and the date; the RSS for a newer Veterans Day item); if nothing changed, Gate 1 and Gate 2 are not repeated; if anything changed, report it first and fix only that part. The mandatory re-read is recorded here.
