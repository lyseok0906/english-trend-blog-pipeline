# QA record — federal-holiday-weekend-observed

Article: `content/drafts/federal-holiday-weekend-observed.md`
Brief: `research/briefs/federal-holiday-weekend-observed.md`. Sources: `research/sources/federal-holiday-weekend-observed.md` (S1 OPM "Federal Holidays", S2 5 U.S.C. 6103, 2023 edition on govinfo.gov, which also prints Executive Order 11582).
Stage: draft written 2026-10-07; Gate 1 done by Claude on 2026-10-07. Not sent to Gate 2, not approved, not on WordPress, not published.

Method: the OPM page was opened again in the built-in browser on 2026-10-07 and 16 phrases and rows were tested against the page text (Overview wording, both footnote sentences, the OPM fact sheet title, the five weekend rows, the 2028 and 2029 veterans rows and the three 2026 holidays still ahead): all present. The statute page and the executive order text (sections 1 to 5) were read in full from the page. Weekdays of the actual holiday dates were computed by script. Lane 1 rule: a re-check before the user approves the move to `ready` is recommended, not mandatory. No USPS source is used (user decision 2026-10-07).

## Gate 1 — Factual QA (claim by claim)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | For most federal employees, a federal holiday on a Saturday is treated as a holiday on the Friday before, and one on a Sunday on the Monday after; OPM publishes this rule for federal employees | S1-1, S1-2 | pass (attributed) |
| C2 | The facts are as of October 7, 2026; two sources; the article is about federal employees only, not banks, schools, post offices or private employers; shows dates for 2026 to 2028 | Browser reads; scope | pass |
| C3 | OPM says most federal employees work Monday through Friday; for them a Saturday or Sunday holiday usually is observed on the Friday before or the Monday after | S1-1 | pass (attributed) |
| C4 | OPM's footnote: for most federal employees the preceding Friday "will be treated as a holiday for pay and leave purposes" (Saturday) and the following Monday (Sunday) | S1-2 | pass (attributed; quote 9 words) |
| C5 | For Saturday OPM cites 5 U.S.C. 6103(b); the section says that instead of a Saturday holiday the Friday immediately before is a legal public holiday for employees whose basic workweek is Monday through Friday; it applies to statutes on pay and leave | S1-3, S2-1, S2-2 | pass |
| C6 | For Sunday OPM cites Section 3(a) of Executive Order 11582 (February 11, 1971); the order is printed in the notes to the statute | S1-3, S2 page | pass |
| C7 | The order says an employee whose basic workweek does not include Sunday, and who would ordinarily be excused on a holiday, is excused on the next workday when a holiday falls on a Sunday | S2-5 | pass (paraphrase of the order's text) |
| C8 | Table: Independence Day 2026 falls on Saturday, July 4; OPM lists Friday, July 3 | S1-4; weekday computed | pass |
| C9 | Table: Juneteenth 2027 falls on Saturday, June 19; OPM lists Friday, June 18 | S1-4; S2-4; weekday computed | pass |
| C10 | Table: Independence Day 2027 falls on Sunday, July 4; OPM lists Monday, July 5 | S1-4; weekday computed | pass |
| C11 | Table: Christmas Day 2027 falls on Saturday, December 25; OPM lists Friday, December 24 | S1-4; weekday computed | pass |
| C12 | Table: New Year's Day 2028 falls on Saturday, January 1, 2028; OPM lists Friday, December 31, 2027 under its 2028 tab, a date that falls in 2027 | S1-4; weekday computed | pass |
| C13 | OPM's tables mark these dates with a footnote | S1-4 (rows carry a * or ** marker with the footnote) | pass |
| C14 | The three holidays still ahead in 2026 are Veterans Day Wednesday Nov 11, Thanksgiving Thursday Nov 26, Christmas Friday Dec 25; all on weekdays; OPM lists them on their own dates | S1-6; weekday computed | pass |
| C15 | The rule applies to most federal employees; the statute has separate rules for employees whose basic workweek is not Monday through Friday | S1-2, S2-3 | pass |
| C16 | OPM has a fact sheet titled "Federal Holidays - 'In Lieu Of' Determination", not summarized | S1-5 | pass |
| C17 | Scope: no state, local, bank, school, Postal Service or private-employer rules, no pay and leave details, other schedules or Inauguration Day; no source used for those | Scope statement | pass (scope) |
| C18 | Sources: both checked October 7, 2026; the OPM page shows no update date; statute text from the 2023 edition on govinfo.gov, which also prints the executive order | Browser reads | pass |
| C19 | Source titles and URLs | OPM page title "Federal Holidays"; govinfo page "Sec. 6103 - Holidays" | pass |

### Image (`assets/optimized/federal-holiday-weekend-observed.png`, original SVG in `assets/raw/`)

- Own card diagram, no photos, no logos. 1200x2109. Every line traces to the claims above: "For most federal employees (OPM)" (C1); "Saturday holiday is treated as the Friday before; Sunday holiday is treated as the Monday after" (C1, C4); the five example cards (C8 to C12); "Source: OPM and 5 U.S.C. 6103, read Oct. 7, 2026" (C18).
- Alt text in the front matter and the body is identical (539 characters; long, because the five examples are spelled out; Gate 2 may want it shorter).
- File check on the device: pixel hash of the PNG matches the cloud render (md5 of RGB bytes 97483572...). Visual check of the render: no text overflow.

### Handled by wording

- OPM's statements are attributed to OPM; the weekday computation is labeled as computed.
- Nothing is said about the Postal Service or any other organization.
- The "treated as" wording follows OPM's footnote ("for pay and leave purposes"), so the article does not say that offices close.

### Not verified

- The text of Executive Order 11582 beyond what the govinfo page prints; OPM's "In Lieu Of" fact sheet (not opened).
- The OPM page's update date (none shown); a later edition of the U.S. Code than 2023.
- Search volume and competition for the focus keyword (not measured; private-employer intent overlaps).
- The exact diagram text size on a real phone (to be checked in the WordPress preview).

### Re-check obligations

Recommended (lane 1): re-read the OPM overview, both footnotes and the 2026 to 2028 tables before the user approves moving the article to `ready`. If a date or the rule wording changed, return to draft.

## Gate 2 (ChatGPT, 2026-10-07, result reported by the user)

**PASS.** No changes requested. A recommended (not mandatory) re-check of the official pages before the user approves the move to `ready` still applies, because the dates are fixed by statute and OPM tables that rarely change.

## Gate 2 final (ChatGPT, 2026-10-07)

**Gate 2 final PASS** (the original review result stands; no changes were requested).
