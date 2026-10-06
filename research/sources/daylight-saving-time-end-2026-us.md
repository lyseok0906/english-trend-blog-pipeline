# Source notes — daylight-saving-time-end-2026-us

Retrieved: **2026-10-06** (all items below), by Cowork (Claude). Revised the same day after the DOT and statute pages were read (revision note at the end).
**Reading limit:** every page was read through a page-summarizing tool, not opened in a browser. Quotes below are what the tool returned. Claude re-reads these pages at drafting, at factual QA and before publish approval. The user's own look happens at final publish approval (user instruction, 2026-10-06).

## S1 — NIST: Daylight Saving Time (primary, official)

- URL: https://www.nist.gov/pml/time-and-frequency-division/popular-links/daylight-saving-time-dst
- Page date shown: "Updated February 9, 2026".

| # | Claim supported | Support |
|---|---|---|
| S1-1 | In 2026, daylight saving time begins March 8 at 2:00 a.m. local time and ends November 1 at 2:00 a.m. local time | Stated on page |
| S1-2 | Rule: begins "at 2:00 a.m. on the second Sunday of March" and ends "at 2:00 a.m. on the first Sunday of November" | Quoted on page |
| S1-3 | At the November change, clocks go from 2 a.m. back to 1 a.m. (one hour repeated); in March they go from 2 a.m. to 3 a.m. | Stated on page |
| S1-4 | Places that do not observe daylight saving time: Hawaii, American Samoa, Guam, Puerto Rico, U.S. Virgin Islands, and Arizona (except the Navajo Indian Reservation) | Stated on page |
| S1-5 | Daylight saving time and time zones are regulated by the U.S. Department of Transportation, not by NIST; the Energy Policy Act of 2005 is the law cited | Stated on page (paraphrased) |

## S2 — U.S. DOT: Daylight Saving Time page (primary, official; the regulating agency)

- URL: https://www.transportation.gov/regulations/daylight-saving-time
- Page date shown: "Last updated September 3, 2025".

| # | Claim supported | Support |
|---|---|---|
| S2-1 | Places that do not observe daylight saving time: Hawaii, American Samoa, Guam, Northern Mariana Islands, Puerto Rico, the Virgin Islands, and most of Arizona | Quoted by tool from the page |
| S2-2 | DOT oversees regulations under the Uniform Time Act | Stated on page (paraphrased) |

Not on the page (per the tool): the start and end Sundays, whether states may adopt year-round daylight time.

**Difference between S1 and S2 (must be settled at factual QA):** S2 lists the Northern Mariana Islands and S1 does not; S1 says Arizona "except the Navajo Indian Reservation" while S2 says "most of Arizona". The two sources are not contradictory about Arizona, but the lists differ on one territory. The draft attributes the list to DOT (the regulating agency) and does not present the NIST list as complete.

## S3 — U.S. DOT: Uniform Time (primary, official)

- URL: https://www.transportation.gov/regulations/time-act
- Page date shown: "Last updated July 15, 2026".

| # | Claim supported | Support |
|---|---|---|
| S3-1 | The Uniform Time Act establishes a system of uniform daylight saving time across the nation; states that observe it must begin and end on federally mandated dates | Stated on page (paraphrased) |
| S3-2 | "States may choose to exempt themselves from observing Daylight Saving Time by State law." | Quoted on page |
| S3-3 | States cannot choose permanent daylight saving time | Reported by tool as the page's statement; **confirm the exact wording at factual QA** |
| S3-4 | "DOT does not have the power to repeal or change Daylight Saving Time" and has no role in individual state decisions | Quoted on page |
| S3-5 | DOT oversees the nation's time zones; Congress or the Secretary of Transportation can change time-zone boundaries | Stated on page (paraphrased) |

Not on the page (per the tool): the start and end dates.

## S4 — 15 U.S.C. § 260a, govinfo.gov (primary, official statute text)

- URL: https://www.govinfo.gov/link/uscode/15/260a
- Page date: no edition date labeled (per tool); amendment notes show changes in 1972, 1983, 1986 and 2005, and the text reflects amendments through Pub. L. 109-58 (Aug. 8, 2005).

| # | Claim supported | Support |
|---|---|---|
| S4-1 | Daylight saving time runs from 2 a.m. on the second Sunday of March to 2 a.m. on the first Sunday of November | Stated in statute text |
| S4-2 | A state entirely within one time zone may exempt itself by law; a state in more than one time zone may exempt the whole state or the part within a given zone | Stated in statute text (paraphrased) |
| S4-3 | The 2005 amendment moved the period from April-October to March-November | Reported by tool from the page's amendment notes |

The uscode.house.gov copy returned only a maintenance notice on 2026-10-06 and was not used.

## S5 — 15 U.S.C. § 260a, Cornell Legal Information Institute copy (corroboration only)

- URL: https://www.law.cornell.edu/uscode/text/15/260a
- Read the same day; it agrees with S4 on the dates (S4-1) and state exemptions (S4-2). It is a university-hosted copy, so S4 is the citation if the draft cites the statute.

## S6 — Calendar computation (Python, 2026-10-06)

- March 2026 Sundays: 1, 8, 15 → second Sunday is March 8. November 2026 Sundays: 1, 8 → first Sunday is November 1.
- Days from 2026-10-06 to 2026-11-01: 26.
- This checks S1-1 against the rule in S1-2 and S4-1; it does not replace them.

## S7 — Google autocomplete, US setting (demand signal, qualitative only)

Endpoint: suggestqueries.google.com, `hl=en&gl=us`. Fetched 2026-10-06 through the summarizing tool. Autocomplete changes between fetches and shows that a query shape is suggested; it gives no search volume and no competition.

**`when does daylight saving time end 2026`:** 1 when does daylight saving time end 2026 / 2 …2026 usa / 3 when does daylight savings time end 2026 canada / 4 …australia / 5 …uk / 6 …in ontario / 7 …california / 8 …alberta / 9 …vancouver / 10 when do daylight saving time end 2026.

**`when does daylight saving time end in the us`:** 1 …in the us / 2 …in the us in 2026 / 3 …in the usa / 4 …in the us 2025 / 5 …in the us this year / 6 when did daylight savings time end in the us / 7 when does daylight savings time stop in the us / 8 when does daylight savings time start and end in the us / 9 is daylight saving time still in effect / 10 are we ending daylight savings time this year.

**`when do clocks go back 2026`:** suggestions included uk, usa, scotland, canada, ireland, england, ontario, australia, gov uk (US is one of nine).

**`which states do not observe daylight saving time`:** 10 suggestions, all US-state intent (includes "which two states do not observe daylight saving time").

## Not verified

- Search volume and competition.
- The exact wording of S3-3 (permanent daylight saving time).
- Whether the Northern Mariana Islands belong in the list the article gives (S2 includes them, S1 does not).
- Anything about pending legislation (out of scope). S3-4 is the only sentence the article uses for readers who ask whether daylight saving time is ending, and it says only what DOT can and cannot do.
- Other countries' dates (out of scope).

## To re-check at drafting, at factual QA and before publish approval

Re-read S1 to S4 (page dates, the 2026 dates, the non-observing list, S3-3 wording). If a page date or a fact changed, record it here and return to draft.

## Revision note

First version (commit e346543) listed the DOT page as unread and the statute as read only through the Cornell copy. This revision adds S2, S3 and S4, and records the difference between the NIST and DOT lists.
