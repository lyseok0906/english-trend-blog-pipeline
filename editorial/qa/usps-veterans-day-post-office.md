# QA record — usps-veterans-day-post-office

Article: `content/drafts/usps-veterans-day-post-office.md` (draft, 2026-11-06; about 370 words in the body, one H1, three H2 sections including Sources; one table).
Brief: `research/briefs/usps-veterans-day-post-office.md`. Sources: `research/sources/usps-veterans-day-post-office.md` (S1 USPS national release of Nov. 4, 2026).
Stage: **published 2026-11-06** (ready 2026-11-06 with the user's approval; file in `content/ready/`). Gate 1 (Claude) done 2026-11-06; Gate 2 (ChatGPT, base commit `61113c6`) = PASS, reported by the user 2026-11-06.

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
| I7 | Files: `assets/raw/usps-veterans-day-post-office.svg`, `assets/optimized/usps-veterans-day-post-office.png` (1200 x 1500, 221,867 bytes, sha256 17c8537b...c418; corrected 2026-11-06: the 217,379 first written was the size of an earlier render) read back from the repository | pass |

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


## Move to `ready` (user approval 2026-11-06)

The user approved the move to `ready` and the WordPress draft on 2026-11-06. The file was moved from `content/drafts/` to `content/ready/` and the front matter set to `status: ready`; the article text, diagram and alt were not changed by the move.

## WordPress draft (2026-11-06)

Post 82 (draft) and diagram media 81 were created through the logged-in browser session. Checks before publishing: posted body equals the repository text after block conversion (sha256 of the typed source matched before posting; the saved raw content equals the source apart from the image block); 13 blocks, none invalid; image file read back from the site has the repository hash 17c8537b...c418 (221,867 bytes), alt text equals the front matter alt; category Postal service and stamps; comments and pings closed; Rank Math focus keyword `is the post office open on veterans day` and the 145-character description read back in the editor; logged-out request returned 404 and the draft was not in the sitemap. The table block has the same mobile setting as the other tables (automatic column widths, font size `clamp(12px, 3.6vw, 18px)`).

**Mobile preview:** at 375 px and 320 px no horizontal overflow, no word broken inside a table cell, the diagram loaded (WordPress served a 768 px copy through srcset) and its text was readable on screen.

## Pre-publication check of the USPS notice (2026-11-06, about 04:43 UTC)

Only whether the source changed (the user's rule; Gate 1 and Gate 2 not repeated). The Nov. 4, 2026 release was fetched again: page title and "Nov. 4, 2026" unchanged; the three relied-on sentences present word for word ("will observe Veterans Day on Wednesday, November 11", "All Post Office locations will be closed", "Regular mail delivery and retail services will resume on Thursday, November 12"); "Priority Mail Express" appears once (kiosk postage-printing list) and there is still no statement on its delivery; no hours. USPS newsroom feed: 702 items, newest Nov. 4, 2026; the only Veterans Day items are the Nov. 4, 2026 release and the Oct. 29, 2025 one. **No change.**

## Publication and live QA (2026-11-06)

Published by Claude at the user's explicit request of 2026-11-06 (the user had earlier said they would publish themselves and changed this in the same message that approved ready): REST status change on post 82, published 2026-11-06 04:43:44 UTC (site local time 2026-11-05 23:43). Logged-out checks right after:

| Check | Result |
|---|---|
| URL https://statesideexplained.com/usps-veterans-day-post-office/ | 200 |
| Title, H1 | "Is the Post Office Open on Veterans Day? What USPS Says for 2026" (title tag adds " - Stateside Explained") |
| Canonical, og:url | the post URL |
| Meta description, og:description | the 145-character description |
| Robots | index, follow, max-snippet:-1, max-video-preview:-1, max-image-preview:large |
| og:image | the diagram file |
| JSON-LD | Person, Organization, WebSite, ImageObject, WebPage, BlogPosting |
| Comment form, pingback link | none |
| Diagram | loaded; file read back with the repository hash; alt text correct |
| Links in the body | one, the USPS release (opens in a new tab, rel noopener) |
| Headings and table | three H2 (what the notice says, what it does not say, Sources), one table, the key sentences present in the page text |
| Phone width (375 px) | no overflow, no broken words in the table, diagram readable |
| Post sitemap | listed, lastmod 2026-11-06T04:43:44+00:00 (16 URLs in the post sitemap) |
| RSS feed and home page | the post is listed in both |
| Public REST | status publish, category 6 |

No indexing request was made (user rule). Result: **live QA passed.**
