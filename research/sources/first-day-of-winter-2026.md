# Source notes — first-day-of-winter-2026

Retrieved: **2026-10-07**, by Cowork (Claude), both pages opened in the built-in browser (a real browser). Brief: `research/briefs/first-day-of-winter-2026.md`.
Reading limit: the NOAA page was read in full from the page text. The USNO data service was queried through the page's own API with the page's own time-zone list.

## S1 — USNO, Earth's Seasons data service (primary, official)

- URL: https://aa.usno.navy.mil/data/Earth_Seasons (page title "Earth's Seasons - Equinoxes, Solstices, Perihelion, and Aphelion"). Data call used: `/api/seasons?year=2026&tz=<offset>&dst=false`.
- Page date shown: none.
- Read: yes (2026-10-07).
- Page text, verbatim: "The times of the equinoxes mark the beginning of spring and fall. The times of the solstices mark the beginning of summer and winter." and "The seasons are hemisphere dependent. While the northern hemisphere experiences summer, the southern hemisphere is experiencing winter. That said, the conventional method for naming the solstices and equinoxes is by the seasons of the northern hemisphere."
- The page's time-zone selector ("Need USA Time Zone?") lists: -4 Atlantic Standard Time; -5 Eastern Standard Time; -6 Central Standard Time; -7 Mountain Standard Time; -8 Pacific Standard Time; -9 Alaska Standard Time; -10 Hawaii-Aleutian Standard Time; -11 Samoa Standard Time; +10 Chamorro Standard Time. The page also says "5 hours West of Greenwich (UTC-5) is Eastern Standard Time".
- API result for the year 2026 (tz 0): December solstice, day 21, month 12, time "20:50". Further calls (dst false): tz -5 gives 15:50; tz -6 gives 14:50; tz -7 gives 13:50; tz -8 gives 12:50; tz -9 gives 11:50; tz -10 gives 10:50. All are December 21, 2026. (The same call returned the other 2026 events: perihelion Jan 3 17:15, March equinox Mar 20 14:46, June solstice Jun 21 08:24, aphelion Jul 6 17:30, September equinox Sep 23 00:05, all UTC; not used.)

| # | Claim supported | Support |
|---|---|---|
| S1-1 | USNO says the solstices mark the beginning of summer and winter | Quoted on page |
| S1-2 | The December 2026 solstice is on December 21 at 20:50 UTC | API tz 0 |
| S1-3 | On the same date, the time is 3:50 p.m. Eastern, 2:50 p.m. Central, 1:50 p.m. Mountain, 12:50 p.m. Pacific, 11:50 a.m. Alaska and 10:50 a.m. Hawaii-Aleutian Standard Time | API with tz -5 to -10, using the page's own zone list |
| S1-4 | Seasons are hemisphere dependent; solstice and equinox names follow the Northern Hemisphere | Quoted on page |

## S2 — NOAA NCEI, "Meteorological Versus Astronomical Seasons" (primary, official)

- URL: https://www.ncei.noaa.gov/news/meteorological-versus-astronomical-seasons
- Page dates shown on the page: "PUBLISHED SEPTEMBER 22, 2016"; "UPDATED DATE MARCH 10, 2023" with the note "BROKEN LINKS UPDATED. THE DESCRIPTION OF THE MONTHS FOR EACH METEOROLOGICAL SEASON WAS CLARIFIED AS APPLYING TO THE NORTHERN HEMISPHERE." (The page metadata gives different dates, published 2016-03-10 and modified 2024-11-15; the visible dates are the ones used.)
- Read: yes, in full (2026-10-07).
- Verbatim lines used:
  - "In short, it's because the astronomical seasons are based on the position of Earth in relation to the sun, whereas the meteorological seasons are based on the annual temperature cycle."
  - "In the Northern Hemisphere, the summer solstice falls on or around June 21, the winter solstice on or around December 22, the vernal or spring equinox on or around March 21, and the autumnal equinox on or around September 22."
  - "the elliptical shape of Earth's orbit around the sun causes the lengths of the astronomical seasons to vary between 89 and 93 days."
  - "Meteorologists and climatologists break the seasons down into groupings of three months based on the annual temperature cycle as well as our calendar."
  - "meteorological winter includes December, January, and February." (preceded by "Meteorological spring in the Northern Hemisphere includes March, April, and May; ...")
  - "they are more closely tied to our monthly civil calendar than the astronomical seasons are. The length of the meteorological seasons is also more consistent, ranging from 90 days for winter of a non-leap year to 92 days for spring and summer."
  - "it becomes much easier to calculate seasonal statistics from the monthly statistics"

| # | Claim supported | Support |
|---|---|---|
| S2-1 | Astronomical seasons are based on Earth's position relative to the sun; meteorological seasons on the annual temperature cycle | Stated on page |
| S2-2 | In the Northern Hemisphere the winter solstice falls on or around December 22 | Stated on page (general statement) |
| S2-3 | Meteorological seasons are three-month groups; meteorological winter is December, January and February (Northern Hemisphere) | Stated on page |
| S2-4 | Meteorological seasons are tied to the civil calendar and are more consistent in length (winter 90 days in a non-leap year); this makes seasonal statistics easier to calculate | Stated on page |
| S2-5 | Astronomical season lengths vary between 89 and 93 days | Stated on page |

## Calendar facts (computed, not from a source page)

- December 1, 2026 is a Tuesday; December 21, 2026 is a Monday; the two dates are 20 days apart. Checked with a calendar computation on 2026-10-07.
- December, January and February of winter 2026–27 contain 31 + 31 + 28 = 90 days (2027 is not a leap year); this matches NOAA's "90 days for winter of a non-leap year". The article does not state it as a fact about 2026–27 unless attributed to NOAA.

## Not sourced and not used

- Any statement that the solstice is the "shortest day" (not in either page).
- Any weather or snow statement.
- Search demand (not measured; see the brief).
