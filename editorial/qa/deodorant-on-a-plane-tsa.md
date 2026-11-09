# QA record — deodorant-on-a-plane-tsa

Article: `content/drafts/deodorant-on-a-plane-tsa.md` (draft, 2026-11-09; about 950 words including the sources list; one H1, eight H2 sections; one table).
Brief: `research/briefs/deodorant-on-a-plane-tsa.md`. Sources: `research/sources/deodorant-on-a-plane-tsa.md` (S1 TSA Deodorant (aerosol), March 29, 2023; S2 TSA Deodorant (liquid), March 29, 2023; S3 TSA Deodorant (Solid), March 30, 2017; S4 eCFR 49 CFR 175.10, up to date as of 11/05/2026).
Stage: **draft, Gate 1 (Claude) done 2026-11-09.** Gate 2 (ChatGPT by the user), ready, WordPress and publication are not done.

## Scope

Only what the three TSA pages state and what 49 CFR 175.10(a)(1) states about toiletries including aerosols. No other toiletries, gel or roll-on products, brands, prices, airline rules or other countries.

## Method

After drafting, the three TSA pages, TSA's item search for "deodorant" and the eCFR page were opened again in the built-in browser (2026-11-09) and tested by script after normalization (apostrophes, quotation marks, dashes, whitespace, lower case): aerosol and liquid pages 8 of 8 phrases each, solid page 3 of 3; the aerosol and liquid texts between the header and the final-decision line are identical; eCFR 6 of 6 phrases. Absence tests: the solid page has no size wording (no "3.4", "ounce" or "ml") and no "gel" or "roll"; the item search returns exactly the three deodorant pages.

## Gate 1 — Factual QA (claim by claim)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | Solid deodorant: carry-on Yes, checked Yes; no size limit or other instruction on the page; last updated March 30, 2017 | S3 | pass (absence tested) |
| C2 | Aerosol and liquid deodorant: carry-on "Yes (Less than or equal to 3.4oz/100 ml allowed)", checked "Yes"; both last updated March 29, 2023 | S1; S2 | pass |
| C3 | The aerosol and liquid pages carry the same header and the same text | S1; S2 | pass (compared by script) |
| C4 | The pages do not explain the 3.4-ounce figure | S1; S2 | pass (read; no explanation) |
| C5 | Checked bags: the FAA limits the total amount of restricted medicinal and toiletry articles including aerosols; total per person 2 kg (70 oz) or 2 L (68 fl oz); each container 0.5 kg (18 oz) or 500 ml (17 fl oz); "See the FAA regulations for more information" | S1; S2 | pass |
| C6 | 49 CFR 175.10(a)(1): medicinal and toilet articles (including aerosols) in carry-on and checked baggage; same aggregate and container quantities; eCFR up to date as of Nov. 5, 2026 | S4 | pass |
| C7 | The rule also says the release of gas must not cause extreme annoyance or discomfort to crew members so as to prevent the correct performance of assigned duties | S4 | pass |
| C8 | The TSA pages do not cite the paragraph by number (so the article says only that the rule "appears to be" the one they point to) | S1; S2 | pass (absence tested) |
| C9 | Release devices (button or nozzle) must be protected by caps or other suitable means, on both the aerosol and the liquid page; the rule says a cap or other suitable means; the Solid page does not mention release devices | S1; S2; S3; S4 | pass |
| C10 | TSA's item search for "deodorant" returns exactly these three pages; no TSA page for gel or roll-on deodorant | search | pass |
| C11 | No page gives a number of deodorants or mentions a brand or ingredients | S1; S2; S3 | pass (read) |
| C12 | Every page says the final decision rests with the TSA officer | S1; S2; S3 | pass |
| C13 | Table: the three rows match C1, C2, C5 and the page dates | S1; S2; S3 | pass |
| C14 | Internal link to the 3-1-1 post is the only claim about the general liquids rule (no rule restated) | own post | pass (link tested at publication) |

## Image check

| # | Item | Result |
|---|---|---|
| I1 | Solid card: carry-on Yes, checked Yes, no size limit shown matches C1 | pass |
| I2 | Aerosol card: 3.4 oz (100 ml) or less, checked Yes, release device capped or protected matches C2, C9 | pass |
| I3 | Liquid card: same text as the aerosol page matches C3 | pass |
| I4 | Checked-bag totals card: 2 kg (70 oz) or 2 L (68 fl oz) per person; each container 0.5 kg (18 oz) or 500 ml (17 fl oz); TSA points to the FAA regulations matches C5 | pass |
| I5 | Dates card: solid March 30, 2017; aerosol and liquid March 29, 2023; final decision with the TSA officer matches C1, C2, C12; footer sources and read date match the article | pass |
| I6 | Alt text (741 characters) in front matter and body is identical and says the same as the diagram | pass |
| I7 | Files `assets/raw/deodorant-on-a-plane-tsa.svg` and `assets/optimized/deodorant-on-a-plane-tsa.png` (1200 x 2517, 391,865 bytes, sha256 35a6c965...5eca) in the repository; no logos or photos; text 25 to 46 px on an 800 px canvas; no text past the right margin | pass |

## Format

Title 57 characters; slug `deodorant-on-a-plane-tsa`; meta description 147 characters; the focus keyword `can you bring deodorant on a plane` appears word for word in the title only (the title uses "Can You Bring Deodorant on a Plane?"); one H1; plain markdown table with five columns (check on a phone at the WordPress preview, as for the razor post); no prices.

## Open points

- **P1 (old pages):** the solid page dates from 2017 and the others from 2023; the article gives each date.
- **P2 (FAA link):** the TSA pages say "See the FAA regulations" without a citation; the article reads 49 CFR 175.10(a)(1) and says it "appears to be" the rule, without claiming TSA applies exactly this text.
- **P3 (demand):** probably a quick yes/no and size search; relative index only (see brief).
- **P4 (5-column table on phones):** use the razor post's table font `clamp(11px, 3.2vw, 18px)` and check 375 and 320 px.

## Result and next step

Gate 1: **PASS** (14 of 14 claims, 7 of 7 image checks). Next: push, Gate 2 by commit SHA. After a Gate 2 PASS under the standing rule: ready, WordPress draft, phone preview, re-read of the three TSA pages, the item search and the eCFR paragraph right before publishing, publish if unchanged, live QA and records.
