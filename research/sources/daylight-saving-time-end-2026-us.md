# Source notes — daylight-saving-time-end-2026-us

Retrieved: **2026-10-06** (all items below), by Cowork (Claude).
**Reading limit:** every page was read through a page-summarizing tool, not opened in a browser. Quotes below are what the tool returned. Open the pages yourself before drafting and before publishing.

## S1 — NIST: Daylight Saving Time (primary, official)

- URL: https://www.nist.gov/pml/time-and-frequency-division/popular-links/daylight-saving-time-dst
- Page date shown: "Updated February 9, 2026".
- Read: yes (summary by tool).

| # | Claim supported | Support |
|---|---|---|
| S1-1 | In 2026, daylight saving time begins March 8 at 2:00 a.m. local time and ends November 1 at 2:00 a.m. local time | Stated on page |
| S1-2 | Rule: begins "at 2:00 a.m. on the second Sunday of March" and ends "at 2:00 a.m. on the first Sunday of November" | Quoted on page |
| S1-3 | At the November change, clocks go from 2 a.m. back to 1 a.m. (one hour repeated); in March they go from 2 a.m. to 3 a.m. | Stated on page |
| S1-4 | Places that do not observe daylight saving time: Hawaii, American Samoa, Guam, Puerto Rico, U.S. Virgin Islands, and Arizona (except the Navajo Indian Reservation) | Stated on page |
| S1-5 | Daylight saving time and time zones are regulated by the U.S. Department of Transportation, not by NIST; the Energy Policy Act of 2005 is the law cited | Stated on page (paraphrased) |

Not on the page (per the tool): energy-savings data, legislative history beyond the 2005 Act, practices of non-US territories.

## S2 — 15 U.S.C. § 260a, Cornell Legal Information Institute copy (statute text, not the government's own site)

- URL: https://www.law.cornell.edu/uscode/text/15/260a
- Page date: shows an amendment note; the 2005 amendment took effect March 1, 2007 (per tool).
- Read: yes (summary by tool). **This is a university-hosted copy of the statute, not uscode.house.gov or govinfo.gov.** If the draft cites the statute, open the official copy and use it as the citation.

| # | Claim supported | Support |
|---|---|---|
| S2-1 | Daylight saving time runs from 2 a.m. on the second Sunday of March to 2 a.m. on the first Sunday of November | Stated in statute text |
| S2-2 | A state entirely within one time zone may exempt itself by law if the entire state observes standard time; a state in more than one time zone may exempt the whole state or the part within a given zone | Stated in statute text (paraphrased) |

## S3 — Calendar computation (Python, 2026-10-06)

- March 2026 Sundays: 1, 8, 15 → second Sunday is March 8. November 2026 Sundays: 1, 8 → first Sunday is November 1.
- Days from 2026-10-06 to 2026-11-01: 26.
- This checks S1-1 against the rule in S1-2; it does not replace S1.

## S4 — Google autocomplete, US setting (demand signal, qualitative only)

Endpoint: suggestqueries.google.com, `hl=en&gl=us`. Fetched 2026-10-06 through the summarizing tool. Autocomplete changes between fetches and shows that a query shape is suggested; it gives no search volume and no competition.

**`when does daylight saving time end 2026`:** 1 when does daylight saving time end 2026 / 2 …2026 usa / 3 when does daylight savings time end 2026 canada / 4 …australia / 5 …uk / 6 …in ontario / 7 …california / 8 …alberta / 9 …vancouver / 10 when do daylight saving time end 2026.

**`when does daylight saving time end in the us`:** 1 …in the us / 2 …in the us in 2026 / 3 …in the usa / 4 …in the us 2025 / 5 …in the us this year / 6 when did daylight savings time end in the us / 7 when does daylight savings time stop in the us / 8 when does daylight savings time start and end in the us / 9 is daylight saving time still in effect / 10 are we ending daylight savings time this year.

**`when do clocks go back 2026`:** suggestions included uk, usa, scotland, canada, ireland, england, ontario, australia, gov uk (US is one of nine).

**`which states do not observe daylight saving time`:** 10 suggestions, all US-state intent (includes "which two states do not observe daylight saving time").

## Not verified

- Search volume and competition.
- The Department of Transportation's own page on this topic (not read; a DOT page returned 404 in an earlier session).
- Anything about proposed legislation (out of scope).
- Other countries' dates (out of scope).
- The official statute copy at uscode.house.gov or govinfo.gov.

## To re-check before drafting and before publishing

Re-open S1 (look at the "Updated" date and the 2026 dates and the non-observing list) and the statute (S2) in a browser.
