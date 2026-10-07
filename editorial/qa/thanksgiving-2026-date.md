# QA record — thanksgiving-2026-date

Article: `content/drafts/thanksgiving-2026-date.md`
Brief: `research/briefs/thanksgiving-2026-date.md`. Sources: `research/sources/thanksgiving-2026-date.md` (S1 OPM "Federal Holidays", S2 5 U.S.C. 6103, 2023 edition on govinfo.gov).
Stage: draft written 2026-10-07; Gate 1 done by Claude on 2026-10-07. Not sent to Gate 2, not approved, not on WordPress, not published.

Method: both official pages were opened again in the built-in browser on 2026-10-07 (the OPM Overview and the 2024 to 2030 tabs, and the statute text). Every date in the table was read from OPM's tabs; the computed claims were checked by script (see the source notes). Lane 1 rule: a re-check before the user approves the move to `ready` is recommended, not mandatory.

## Gate 1 — Factual QA (claim by claim)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | Thanksgiving 2026 in the U.S. is Thursday, November 26 | S1-1 | pass |
| C2 | Federal law sets Thanksgiving Day as "the fourth Thursday in November" | S2-1 | pass (quote, 8 words) |
| C3 | The facts are as of October 7, 2026; two U.S. government sources; the article is about the U.S., not Canada | Browser reads 2026-10-07; scope | pass |
| C4 | Table: 2024 Nov 28; 2025 Nov 27; 2026 Nov 26; 2027 Nov 25; 2028 Nov 23; 2029 Nov 22; 2030 Nov 28, from OPM's tables | S1-2 | pass |
| C5 | Each of these dates is the fourth Thursday of its November | Computation (script; matches OPM) | pass (computed) |
| C6 | The law's list of legal public holidays reads "Thanksgiving Day, the fourth Thursday in November" | S2-1, S2-2 | pass |
| C7 | November 1, 2026 is a Sunday, so the Thursdays are the 5th, 12th, 19th and 26th; the fourth is the 26th | Calendar computation | pass (computed) |
| C8 | The first Thursday of any November is the 1st to the 7th, so the fourth Thursday is always the 22nd to the 28th; stated to be arithmetic, not an OPM statement | Computation (script over 1900 to 2199: dates 22 to 28 only) | pass (computed, labeled) |
| C9 | The table shows both ends of the range: Nov 22 in 2029; Nov 28 in 2024 and 2030 | S1-2 | pass |
| C10 | OPM says federal law (5 U.S.C. 6103) establishes the public holidays on its pages "for Federal employees"; the statute calls them "legal public holidays" | S1-3, S2-2 | pass (attributed; quote 3 words) |
| C11 | The article does not say what private employers, schools, states, banks or stores do | Scope statement | pass (scope) |
| C12 | The day after Thanksgiving is not on OPM's list of federal holidays | S1-4 | pass |
| C13 | Sources: both checked October 7, 2026; the OPM page shows no update date; statute text is from the 2023 edition of the U.S. Code on govinfo.gov; OPM's current tables cite the same section | Browser reads; S1-3 | pass |
| C14 | Source titles and URLs | OPM page title "Federal Holidays"; govinfo page "Sec. 6103 - Holidays", 2023 Edition | pass |

### Image (`assets/optimized/thanksgiving-2026-date.png`, original SVG in `assets/raw/`)

- Own calendar diagram, no photos, no logos. 1200x1668. Every sentence traces to the claims above: "Thursdays: 5, 12, 19 and 26. The 4th Thursday is November 26" (C7); "Federal law: Thanksgiving Day is the fourth Thursday in November. So it falls between the 22nd and 28th" (C2, C8); "Source: OPM and 5 U.S.C. 6103, read Oct. 7, 2026" (C13).
- The calendar grid is November 2026 (Sunday the 1st, 30 days; computed); the highlighted cell is the 26th.
- Alt text in the front matter and the body is identical (290 characters).
- File check on the device: pixel hash of the PNG matches the cloud render (md5 of RGB bytes 9bc95820...). Visual check of the render: no text overflow.

### Handled by wording

- The rule explanation is labeled as arithmetic; OPM's statements are attributed to OPM.
- The statute edition (2023) is named in the Sources section; the page's own amendment notes were not used as a claim.
- "Federal employees" scope is quoted, so the article does not claim a nationwide rule.

### Not verified

- A later edition of the U.S. Code than the 2023 edition (the uscode.house.gov page was under maintenance); OPM's 2026 table agrees with the statute's rule.
- The OPM page's update date (none shown).
- Whether the title and first paragraph match what searchers want (search volume and competition not measured; Canadian-intent overlap not measured).
- The exact diagram text size on a real phone (to be checked in the WordPress preview).

### Re-check obligations

Recommended (lane 1): re-read S1 and S2 before the user approves moving the article to `ready`. If OPM's 2026 date or the statute's wording differs, return to draft.
