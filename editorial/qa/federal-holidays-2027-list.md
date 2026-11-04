# QA record — federal-holidays-2027-list

Article: `content/ready/federal-holidays-2027-list.md` (ready since 2026-11-04; written as a draft, 2026-11-04, about 916 words in the body, one H1, six H2 sections including Sources).
Brief: `research/briefs/federal-holidays-2027-list.md`. Sources: `research/sources/federal-holidays-2027-list.md` (S1 OPM 2027 tab, S2 OPM 2028 tab, S3 5 U.S.C. 6103 2024 edition, S4 date computation).
Stage: **ready** (moved from `content/drafts/` on 2026-11-04 with the user's approval; status in the front matter set to `ready`). The earlier stage notes below are kept as history. Gate 1 (Claude) run on 2026-11-04. Gate 2 round 1 (ChatGPT, base `a6de32c`, user-reported 2026-11-04): FIX, applied 2026-11-04 (section "Gate 2 FIX round 1"); **Gate 2 round 2 (ChatGPT, base `0336d6b`, user-reported 2026-11-04): PASS** (section "Gate 2 round 2 result"). Still not in ready; the mandatory OPM re-read before approval and before publishing remains. Not in `content/ready/`, not uploaded to WordPress. Mandatory OPM re-read applies again at approval and before publishing.

## Scope as approved by the user (2026-11-04)

- Based on OPM's full 2027 list (11 rows). Linked to the published weekend-holiday post for the rule; the rule is stated in two sentences and the examples table is not repeated.
- Friday, Dec. 31, 2027 (observed New Year's Day 2028) is kept apart from the 2027 list: its own section, its own card in the diagram, and the sentence "this article does not count it among the 11 holidays above".
- No USPS, bank, stock-market, school, state or private-employer schedule; no pay or leave advice.
- No search volume or Trends figure in the article.

## Method

After drafting, on 2026-11-04 (built-in browser, real page loads): OPM page tested by script (2027 table rows, both footnotes, the "In Lieu Of" fact-sheet title, the 2028 first row and the 2028 weekend footnote, absence of any update text); the statute page tested by script (all 11 holiday strings in (a), (b)(1), (c)); the two live posts opened (weekend post title and its four 2027 dates; Thanksgiving post title, HTTP 200). Weekdays recomputed in Python and asserted (all 16 dates, including June 19, July 4, Dec. 25, Dec. 31, 2027 and Jan. 1, 2028).

## Gate 1 — Factual QA (claim by claim)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | OPM lists 11 federal holidays for 2027, from Friday, January 1 to Friday, December 24 | S1 | pass |
| C2 | Three are printed on a different day from the calendar date: Juneteenth Fri June 18, Independence Day Mon July 5, Christmas Fri Dec. 24 | S1 (rows marked **) | pass |
| C3 | Table dates and holiday names, 11 of 11 rows, in OPM's order (Washington's Birthday name as OPM prints it) | S1 | pass |
| C4 | The last column is the rule in 5 U.S.C. 6103(a): January 1; third Monday in January; third Monday in February; last Monday in May; June 19; July 4; first Monday in September; second Monday in October; November 11; fourth Thursday in November; December 25 | S3 (a) | pass (11 of 11 strings) |
| C5 | OPM names section 6103(a) as the law that specifies holidays for federal employees | S1 footnote * | pass |
| C6 | The weekdays of June 19 (Saturday), July 4 (Sunday) and December 25 (Saturday), 2027 are computed, not OPM's | S4 | pass (computed; disclosed in the article and the diagram footer) |
| C7 | OPM footnote on Washington's Birthday: the name is the one in 6103(a); OPM's policy is to always use the names in the law; other institutions may use other names | S1 footnote * | pass |
| C8 | Link to the Thanksgiving date post with its exact title; for how the fourth Thursday is set | Live post (title and HTTP 200 checked) | pass |
| C9 | Six holidays are set by a weekday rule (MLK, Washington's Birthday, Memorial, Labor, Columbus, Thanksgiving); five by a calendar date (New Year's, Juneteenth, Independence, Veterans, Christmas) | S3 (a) (count of the 11 strings) | pass |
| C10 | The three moved days are all among the five calendar-date holidays, because June 19, July 4 and December 25 fall on a weekend in 2027 | S1; S4 | pass |
| C11 | OPM footnote: Saturday holiday: for most federal employees the preceding Friday will be treated as a holiday for pay and leave purposes; Sunday: the following Monday | S1 footnote ** | pass |
| C12 | OPM cites 5 U.S.C. 6103(b) for the Saturday rule and Section 3(a) of Executive Order 11582 for the Sunday rule | S1 footnote ** | pass |
| C13 | Link to the weekend post with its exact title; the explanation and 2026 to 2028 examples are there and not repeated | Live post | pass |
| C14 | For 2027: Friday June 18 (Juneteenth), Monday July 5 (Independence Day), Friday Dec. 24 (Christmas) | S1 | pass |
| C15 | OPM's 2028 table starts with Friday, December 31, New Year's Day, with the same weekend footnote | S2 (first row; footnote text identical to the 2027 footnote) | pass |
| C16 | January 1, 2028 is a Saturday, so the Friday before is December 31, 2027 | S4 | pass (computed) |
| C17 | The date falls in 2027 but is not on OPM's 2027 tab; not counted among the 11; the 2028 row prints no year, the year is worked out from the weekday | S1; S2 | pass |
| C18 | Exclusions: state and local governments, banks, stock market, schools, Postal Service, private employers; pay and leave details; other work schedules; the "In Lieu Of" fact sheet | Scope statement; fact-sheet title on the OPM page | pass |
| C19 | The statute names Inauguration Day, January 20 of each fourth year after 1965, as a legal public holiday for certain employees; not a 2027 date | S3 (c): "...for the purpose of statutes relating to pay and leave of employees as defined by section 2105... and individuals employed by the government of the District of Columbia employed in the District of Columbia, [and listed Maryland and Virginia counties and cities]" | pass (2025 and 2029 are such years; 2027 is not) |
| C20 | Facts as of November 4, 2026; the OPM page shows no update date; statute from the 2024 edition | Reads | pass |
| C21 | Sources: OPM page (2027 and 2028 tabs) and govinfo statute URL, both opened on 2026-11-04 | Reads | pass |

Result: 21 of 21 claims pass as attributed statements, computed values (disclosed) or stated limits.

## Open points reported

- **P1 — Overlap with the weekend post.** The four 2027 weekend rows appear in both posts. The scope split (full list here; rule and examples there; links both ways proposed, one link from the weekend post to this article would need the user's approval because it changes a published post) is the mitigation. The risk of cannibalization is Claude's judgment, not measured.
- **P2 — Weekday of Jan. 1, 2028 and Dec. 31, 2027.** Computed, not printed by OPM; disclosed.
- **P3 — OPM shows no update date.** The article says so; the re-read before approval and publication is mandatory.
- **P4 — Publication timing.** Plan: publish in early December (estimate from last year's relative Trends curve, source notes); not measured; not in the article.
- **P5 — Competition.** OPM itself and calendar sites were not re-checked; the added value is the attribution, the one-phrase rules and the separate Dec. 31 section (brief).

## Image and alt text

| # | Check | Result |
|---|---|---|
| I1 | Diagram compared with the body and S1/S2: eleven rows with weekday and date as OPM prints them and the holiday name; three rows highlighted with "Falls on Sat, Jun 19", "Falls on Sun, Jul 4", "Falls on Sat, Dec 25"; legend "Yellow: OPM shows a moved day (footnote)"; card "Listed apart" for Fri, Dec 31, 2027 (New Year's Day 2028 on OPM's 2028 tab, not on the 2027 list); footer lines (source, weekdays computed, pages read Nov. 4, 2026) | pass |
| I2 | The Dec. 31 item is visibly separated from the 2027 list (its own gray card below the list) | pass |
| I3 | **File checked as committed.** PNG and SVG staged back from the repository working tree after the write: PNG 1200 x 2277, 94,068 bytes at the source (99,838 bytes after transfer, C2PA block added), pixel-identical to the local build; SVG 37 text elements identical to the build; the draft file in the repository equals the local file. The PNG was opened and viewed from the repository copy | pass |
| I4 | Alt text 309 characters, the same string in the front matter and the body image; matches the table and the separate box | pass |
| I5 | Meta description 140 characters | pass |
| I6 | Front matter complete; one H1; two internal links (weekend post, Thanksgiving post) | pass |
| I7 | Diagram history: the first build left spare space at the bottom of the gray card; its height was reduced before the commit | fixed |

## Gate 2 FIX round 1 (base a6de32c, 2026-11-04)

Gate 2 result (ChatGPT, user-reported): FIX. Request: the PNG's Dec. 31, 2027 item and the alt must say that it is the observed date for New Year's Day 2028.

| # | Change | Result |
|---|---|---|
| H1 | Diagram card "Listed apart": "Fri, Dec 31, 2027: the observed date for New Year's Day 2028. It is on OPM's 2028 tab, not on the 2027 list above." | applied |
| H2 | Alt (333 characters, front matter and body identical): "A separate box lists Friday, Dec. 31, 2027 as the observed date for New Year's Day 2028, from OPM's 2028 tab." | applied |
| H3 | Body, December 31 section: "...so the Friday before it, December 31, 2027, is the observed date for New Year's Day 2028." (it only said "the Friday before it is December 31, 2027" before) | applied |

**Official pages.** OPM 2028 tab first row "Friday, December 31 * | New Year's Day" and its weekend footnote, and the OPM 2027 table were re-opened and tested on 2026-11-04 (Gate 1); the Gate 2 change adds no new statement beyond the OPM row and footnote already tested (C15 to C17).

**Image files checked as committed.** PNG 1200 x 2316, pixel-identical to the local build (102,306 bytes in the repository after the transfer added a C2PA block); SVG 37 text elements identical to the build; the PNG was opened and viewed from the repository copy; the card, the body and the alt agree.

Next: Gate 2 round 2 on the new SHA. Not in ready, not on WordPress; the mandatory OPM re-read at approval and before publishing remains.

## Gate 2 round 2 result (base 0336d6b, reported by the user 2026-11-04)

**PASS.** ChatGPT checked the PNG, the body and the alt for the Dec. 31, 2027 item shown as the observed date for New Year's Day 2028. No change requested or made. Standing conditions: OPM 2027 and 2028 tabs and 5 U.S.C. 6103 are re-read and recorded before approval and before publishing (OPM shows no update date); moving to `ready` and every WordPress step need the user's approval.

## OPM and statute re-read (2026-11-04, second read of the day, built-in browser; user request)

**Result: no change.** OPM "Federal Holidays", 2027 table: the 11 rows (dates, weekdays, names and the footnote marks *, **, **, **) compared as a whole with the rows recorded in the source notes: identical. Both 2027 footnotes (Washington's Birthday naming; the Saturday and Sunday rule with 5 U.S.C. 6103(b) and Section 3(a) of Executive Order 11582) and the "In Lieu Of" fact-sheet title present. 2028 tab: first row "Friday, December 31 * | New Year's Day" present; its footnote is the same weekend sentence. The page still shows no update text. 5 U.S.C. 6103 (2024 edition, govinfo.gov): all 11 strings of (a), the Saturday rule of (b)(1) and the Inauguration Day text of (c) present. The weekdays were computed earlier the same day (S4) and need no repeat. No article change.

The post stays in draft; the re-read is repeated before approval and right before publishing (OPM shows no update date). Moving to `ready` and every WordPress step need the user's approval.

## Move to `ready` (user approval 2026-11-04)

The user approved moving this article to `ready` on 2026-11-04 after the official-source re-check of the same day (section above: no source changed). The file was moved from `content/drafts/` to `content/ready/` and the front matter set to `status: ready`; the article text, diagram and alt were not changed by the move. The OPM 2027 and 2028 tabs and 5 U.S.C. 6103 were read twice on 2026-11-04; no change.

**Before publishing (the user's condition):** the official sources are re-read right before publication and the result is recorded here; if anything changed, the change is reported first and the text fixed before any upload. The as-of date in the article is refreshed at that re-check, which needs the user's approval because it changes the text. WordPress upload and publication have not been done and need the user's separate approval.
