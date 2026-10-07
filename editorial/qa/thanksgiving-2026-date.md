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

## Gate 2 (ChatGPT, 2026-10-07, result reported by the user)

**PASS.** No changes requested. A recommended (not mandatory) re-check of the official pages before the user approves the move to `ready` still applies, because the dates are fixed by statute and OPM tables that rarely change.

## Gate 2 final (ChatGPT, 2026-10-07)

**Gate 2 final PASS** (the original review result stands; no changes were requested).

## Pre-approval re-check (recommended, lane 1) — 2026-10-07

Method: the OPM "Federal Holidays" page was opened in the built-in browser and its full text tested by script (strings normalized for case, quotes, asterisks and spacing): 19 of 19 strings present (the Overview sentences, the Thanksgiving Day rows for 2024 to 2029, the Saturday and Sunday footnotes, the "In Lieu Of" fact sheet title, the marked rows Jul 3 2026, Jun 18 2027, Jul 5 2027, Dec 24 2027, Dec 31, the 2026 rows Nov 11 and Dec 25; no "day after Thanksgiving" entry). The govinfo 5 U.S.C. 6103 page (2023 Edition) was opened and tested: 14 of 14 items present, three of them with only a formatting difference (footnote marker in "section 6309 [1] of this title"; the executive order is printed as "Ex. Ord. No. 11582, Feb. 11, 1971"). Dates were recomputed by script: fourth Thursdays 2024 to 2030 are Nov 28, 27, 26, 25, 23, 22, 28; July 4 2026, June 19 2027, Dec 25 2027 and Jan 1 2028 are Saturdays and July 4 2027 is a Sunday; Nov 11, Nov 26 and Dec 25, 2026 are a Wednesday, Thursday and Friday. **Result: no difference from the source notes; no change to the article.**

Applies to the Thanksgiving claims (OPM rows, statute wording, computed dates). The article is as of October 7, 2026, the same day, so the as-of date in the text is still correct. Ready-move approval has not been given yet.

## Ready-move approval (2026-10-07)

The user approved moving this article to `content/ready/` after Gate 2 final PASS and the recommended source re-check, for this article only. Front matter set to `status: ready`; backlog stage `ready`. Not on WordPress and not published. Next: Claude creates the WordPress draft when the user asks; the user previews on a phone and publishes. If more than a day passes before publishing, tell Claude so the sources are re-read.

## WordPress draft (2026-10-07)

Claude created the draft through the logged-in browser: post id 34, status draft, slug `thanksgiving-2026-date`, category "US dates, seasons and holidays" (id 4), diagram uploaded as media id 33 (1200x1668, not scaled; file hash matches the repository PNG, sha-256 71baaa3b...) with the `image_alt` text (media alt text and body alt identical), no featured image, comments and pings closed. Rank Math meta description (141 characters, equals the front matter) and focus keyword set and confirmed in the edit screen. Body checked against `content/ready/thanksgiving-2026-date.md`: letters and digits only, lowercase, the same 1967 characters as the repository text (image alt and title excluded), one table, six H2 headings, two official source links (OPM and govinfo). The draft returns 404 to logged-out visitors, as it should.

Remaining: the user previews on a phone width (preview link https://statesideexplained.com/?p=34) and publishes (Publish is the user's step). If more than a day passes before publishing, tell Claude so the sources are re-read. After publishing, send the live URL for live QA, then Claude moves the article to `content/published/`.

