# QA record — first-day-of-winter-2026

Article: `content/ready/first-day-of-winter-2026.md` (moved from `content/drafts/` on 2026-10-07)
Brief: `research/briefs/first-day-of-winter-2026.md`. Sources: `research/sources/first-day-of-winter-2026.md` (S1 USNO, S2 NOAA NCEI).
Stage: draft written 2026-10-07; Gate 1 done by Claude on 2026-10-07. Gate 2 (English + SEO, ChatGPT): PASS on commit `2edbc32`, 2026-10-07, no changes. Not approved, not on WordPress, not published.

Method: both sources were opened in the built-in browser on 2026-10-07. The draft's NOAA phrases were tested again by script against the page text after the draft was written (all 12 checks true, including the visible "Updated date March 10, 2023"). The USNO times were produced by the page's own data service for each US standard time zone offset. The calendar facts were computed. Lane 1 rule: re-check is recommended, not mandatory.

## Gate 1 — Factual QA (claim by claim)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | Winter 2026 has two start dates: Tuesday, December 1, and Monday, December 21 | S2-3 (meteorological winter includes December), S1-2 (solstice December 21); weekdays computed | pass |
| C2 | December 1 is the first day of meteorological winter | S2-3: winter includes December, January, February; the first day follows from the month. Marked as following from NOAA's list in the body ("That makes December 1 its first day") | pass (inference stated as such) |
| C3 | December 21 is the winter solstice, "the start of astronomical winter" | S1-1: "The times of the solstices mark the beginning of summer and winter." S2: astronomical seasons are defined by the solstices and equinoxes | pass |
| C4 | Facts are as of October 7, 2026; two US government sources | Reads on 2026-10-07 | pass |
| C5 | Table: meteorological calendar used by meteorologists and climatologists (NOAA), starts Tuesday, December 1; astronomical calendar tied to the solstice (USNO), starts Monday, December 21 | S2-3, S1-1, S1-2 | pass |
| C6 | USNO says "the times of the solstices mark the beginning of summer and winter." (quote, 12 words; capital T lowered because the quote starts mid-sentence) | S1 page text: "The times of the solstices mark the beginning of summer and winter." | pass (attributed) |
| C7 | USNO's data service gives the December 2026 solstice at 20:50 UTC on December 21 | S1-2 (API, year 2026, tz 0) | pass |
| C8 | In US standard time zones the moment is still December 21: Eastern 3:50 p.m.; Central 2:50 p.m.; Mountain 1:50 p.m.; Pacific 12:50 p.m.; Alaska 11:50 a.m.; Hawaii-Aleutian 10:50 a.m. | S1-3: API calls with tz -5, -6, -7, -8, -9, -10, zone names from the USNO page's own selector; all return day 21 month 12 | pass |
| C9 | NOAA describes the astronomical seasons as based on the position of Earth in relation to the sun | S2-1 | pass (attributed) |
| C10 | NOAA says the winter solstice in the Northern Hemisphere falls "on or around December 22" (quote, 5 words) | S2-2, checked by script | pass (attributed) |
| C11 | "That is a general statement. The USNO figure above is the specific one for 2026." | Editorial reading of "on or around" next to a computed 2026 value; no new fact | pass (framing) |
| C12 | USNO says seasons depend on the hemisphere and the solstice and equinox names follow the Northern Hemisphere; the article covers the Northern Hemisphere only | S1-4 | pass (attributed; scope statement) |
| C13 | NOAA says meteorologists and climatologists divide the year into groups of three months based on the annual temperature cycle and the calendar | S2-3, checked by script | pass (attributed) |
| C14 | For the Northern Hemisphere NOAA lists meteorological winter as December, January and February | S2-3 (the page says the description is for the Northern Hemisphere, per its March 10, 2023 update note) | pass |
| C15 | NOAA's reason: the meteorological seasons follow the civil calendar, are more consistent in length, so seasonal statistics are easier to calculate from monthly ones | S2-4, checked by script | pass (attributed) |
| C16 | NOAA gives the length of meteorological winter as 90 days in a non-leap year | S2-4: "ranging from 90 days for winter of a non-leap year to 92 days for spring and summer" | pass (attributed) |
| C17 | NOAA's short answer: astronomical seasons are based on Earth's position relative to the sun, meteorological seasons on the annual temperature cycle | S2-1 | pass (paraphrase, attributed) |
| C18 | NOAA adds that astronomical season lengths vary between 89 and 93 days, which would make year-to-year comparison of seasonal statistics hard | S2-5; the page says the variation in length and start date "would make it very difficult to consistently compare climatological statistics" year to year | pass (paraphrase, attributed) |
| C19 | Scope paragraph (no forecast, no statement of how cold or snowy, no statement of which definition is right, no Southern Hemisphere) | Scope statement | pass (scope) |
| C20 | Sources: both checked October 7, 2026; USNO page shows no update date; NOAA page shows "Updated date March 10, 2023" | USNO page: none seen; NOAA visible text "UPDATED DATE MARCH 10, 2023". The page's metadata gives other dates (modified 2024-11-15); the visible date is used | pass |
| C21 | Source titles and URLs | S1 page title "Earth's Seasons - Equinoxes, Solstices, Perihelion, and Aphelion"; S2 page title "Meteorological Versus Astronomical Seasons" | pass |

### Image (`assets/optimized/first-day-of-winter-2026.png`, original SVG in `assets/raw/`)

- Own diagram, no photos, no weather art, no agency logos. 1200x1509.
- Every sentence traces to the claims above: "Tuesday, December 1" and "Meteorological winter begins; It runs through December, January and February (NOAA)" (C1, C2, C14); "20 days later" (computed: December 21 minus December 1); "Monday, December 21; Winter solstice: astronomical winter begins (USNO)" (C1, C3); "Standard time: 3:50 p.m. Eastern; 12:50 p.m. Pacific; 10:50 a.m. Hawaii-Aleutian" (C8). Source line: "Source: USNO and NOAA, read Oct. 7, 2026".
- Alt text in the front matter and the body is identical and describes the diagram's content without repeating the keyword.
- File check on the device: pixel hash of the PNG matches the cloud render (md5 of RGB bytes 4c73f931...); the SVG on the device contains the diagram title text.
- Visual check: the first render had the last time line crossing the card border; the card was made taller and the render checked again.

### Handled by wording

- Every clock time names its time zone and says standard time.
- The NOAA "on or around December 22" is not presented as a 2026 value; the USNO value is.
- No statement about "shortest day", weather or snow.
- NOAA's visible update date is used instead of the page's metadata dates.

### Not verified

- Search volume and competition for the focus keyword (not measured; see the brief).
- Whether other sites, calendars or schools use either definition (not in the sources; not claimed).
- The exact diagram text size on a real phone (to be checked in the WordPress preview).

### Re-check obligations

Recommended, not mandatory (lane 1): before the user approves publishing, re-read both pages and re-run the USNO query for 2026; compare the three clock times and the NOAA wording. If anything differs, return to draft. Flag for the user: the brief proposed three time zones (Eastern, Pacific, Hawaii); the draft lists six (adding Central, Mountain and Alaska) because all six come from the same USNO call. The diagram keeps three. The focus keyword is the brief's proposal, not separately approved.

## Gate 2 — English + SEO QA

ChatGPT reviewed commit `2edbc32` on 2026-10-07 (this article's draft is in that commit unchanged from the one recorded under Gate 1). Result: **PASS**, no changes requested. The article stays in `content/drafts/` and is not changed by Gate 2.

Next: Recommended (lane 1) source re-check before the user approves the move to `ready`. Moving to `ready` needs the user's approval for this article alone. Not on WordPress, not published.

## Pre-approval source re-check (2026-10-07, recommended for lane 1)

Done by Claude after Gate 2 passed and before asking the user to approve the move to `ready`. Both pages were opened again in the built-in browser.

- USNO: the data service was queried again for year 2026 with tz 0, -5, -6, -7, -8, -9 and -10. December solstice: 20:50 UTC, 15:50, 14:50, 13:50, 12:50, 11:50 and 10:50, all on December 21, the same as in the source notes and the draft. The page text still says "The times of the solstices mark the beginning of summer and winter." and "The seasons are hemisphere dependent." with the Northern Hemisphere naming sentence. The page's own zone selector still lists Eastern, Central, Mountain, Pacific, Alaska and Hawaii-Aleutian Standard Time at -5 to -10.
- NOAA: 13 phrases tested against the page text (all the draft's attributed statements, including "on or around December 22", the three-month groupings, December-January-February, 90 days for winter of a non-leap year, 89 and 93 days, and the visible "Updated date March 10, 2023"): all present, nothing changed.
- Calendar facts (December 1 is a Tuesday, December 21 is a Monday, 20 days apart) are unchanged by definition.

Result: **no difference**; the draft needs no change. The draft text on the device is the text Gate 2 reviewed (commit `2edbc32`). The user's approval to move this article to `ready` is requested separately; until then the article stays in `content/drafts/`.

## Gate 3 — Approval

The user approved moving this article to `content/ready/` on 2026-10-07, after Gate 2 PASS and the source re-check above (no difference). The approval covers this article only. Front matter set to `status: ready`. Publishing is a separate step by the user: next, Claude uploads the article to WordPress as a draft (title, slug, category "US dates, seasons and holidays", diagram with alt text, Rank Math meta description and focus keyword), and the user previews on phone width and presses Publish.

If more than a day passes before publishing, tell Claude so USNO and NOAA are re-read before Publish (recommended for lane 1).
