# Brief — first-day-of-winter-2026

**Stage:** topic brief (lifecycle step 1). Source notes not yet created: the verbatim notes below are moved into `research/sources/first-day-of-winter-2026.md` at the sources step. No draft exists.
**Lane:** US dates, seasons and holidays. **Pilot slot:** a week 2–4 post (see "Why now").
**Prepared:** 2026-10-07 by Cowork (Claude). Not yet reviewed by the user or ChatGPT.

## Candidate card

| Check | Result |
|---|---|
| Official sources | U.S. Naval Observatory (USNO) Earth's Seasons data service; NOAA NCEI "Meteorological Versus Astronomical Seasons". Both opened in a real browser on 2026-10-07 |
| Diagram without photos | Yes: one timeline, Dec 1 (meteorological winter starts) and Dec 21 (winter solstice) |
| Search question clear | Yes, one question with two correct answers. Weakness: the date alone is answered directly in results, so the article's value is the two definitions |
| Changing information | No: both dates are astronomy and a calendar convention. The only live element is the USNO data service itself |
| Re-check before approval | Recommended, not mandatory (lane 1): re-run the USNO year query and re-read the NOAA page |

## Topic

Why "the first day of winter" has two answers in 2026, and what each one means.

## Working title (proposal)

When Is the First Day of Winter in 2026? Two Answers

## Search intent and focus keyword

- **Proposed focus keyword:** `when is the first day of winter 2026`
- **Intent:** informational, a date question. Readers also ask which date "counts".
- **Demand signal:** the Google autocomplete check (US setting) in `docs/blog-c-lanes-planning.md` (2026-10-06) listed 10 variants, including "in usa", "in the united states" and state names. It was not repeated on 2026-10-07: the fetch tool returned a result for a different query, which was discarded. A web search for the keyword on 2026-10-07 returned mostly almanac and countdown pages (titles only; not a Google ranking). **Search volume and competition were not checked.**

## Audience

US readers who want the date and want to know why calendars and weather reports disagree.

## Angle

1. **The answer.** Winter 2026 has two start dates: the winter solstice on Monday, December 21, and meteorological winter on Tuesday, December 1 (weekdays computed from the calendar).
2. **Astronomical definition (USNO).** The solstices mark the beginning of summer and winter. For 2026 the USNO data service gives the December solstice at 20:50 UTC on December 21, which is 3:50 p.m. Eastern Standard Time, 12:50 p.m. Pacific Standard Time and 10:50 a.m. in Hawaii. The date is December 21 in all of those zones.
3. **Meteorological definition (NOAA).** Meteorological winter is December, January and February. NOAA says meteorologists and climatologists use three-month groups tied to the calendar because they make seasonal statistics easier to calculate.
4. **Why they differ.** Astronomical seasons follow Earth's position relative to the sun; meteorological seasons follow the annual temperature cycle (NOAA).

## Why now

Winter begins in 55 days (December 1) and 75 days (December 21). No hard deadline; the article is useful any time before December 1. Interest probably rises in late November (Claude's judgment, not measured).

## Scope: in and out

- **In:** the two definitions, the two 2026 dates, the USNO times with time zones, the NOAA reasons.
- **Out:** weather or snow forecasts, "shortest day" statements (not in the pages read), Southern Hemisphere details beyond the one USNO note that seasons depend on the hemisphere, state-by-state variants (the start is not a state rule), advice on anything.

## Image plan (no photos)

Own horizontal timeline: Dec 1 (meteorological winter begins; runs through February) and Dec 21 (solstice, with the three clock times) on one line. No weather or seasonal photos.

## Official source notes (read 2026-10-07 in the built-in browser)

- **USNO Earth's Seasons**, https://aa.usno.navy.mil/data/Earth_Seasons (query `year=2026`). Page note: "The times of the equinoxes mark the beginning of spring and fall. The times of the solstices mark the beginning of summer and winter." and "The seasons are hemisphere dependent." The data service (`/api/seasons?year=2026`) returned the December solstice as day 21, month 12 at 20:50 for tz 0, 15:50 for tz -5, 12:50 for tz -8 and 10:50 for tz -10. The page shows no update date (browser last-modified header is the load time).
- **NOAA NCEI, "Meteorological Versus Astronomical Seasons"**, https://www.ncei.noaa.gov/news/meteorological-versus-astronomical-seasons. Page metadata: published 2016-03-10, modified 2024-11-15. Says the winter solstice falls "on or around December 22" in the Northern Hemisphere (a general statement; the USNO 2026 value is the specific one) and that meteorological winter "includes December, January, and February".

## Re-check rule

Lane 1: re-read both sources at drafting, at factual QA and before publish approval; re-run the USNO query for 2026 and compare the three clock times. If the USNO values or the NOAA wording differ, return to draft.

## Risks

- A date-only query is probably answered in the results themselves (Claude's judgment), so the article has to carry the two-definition explanation.
- NOAA's "on or around December 22" and USNO's December 21 look different; the draft must say the NOAA wording is general and USNO's is the 2026 value.
- Time zones: a solstice time given without a zone would be wrong for some readers. Every time in the article names its zone.

## Open questions for the user

1. Approve the focus keyword.
2. Approve naming Eastern, Pacific and Hawaii times (the other zones are not needed).
