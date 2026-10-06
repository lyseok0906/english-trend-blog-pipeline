# QA record — daylight-saving-time-end-2026-us

Draft: `content/drafts/daylight-saving-time-end-2026-us.md`
Sources: `research/sources/daylight-saving-time-end-2026-us.md` (S1–S7)
Stage: factual QA done by Claude on 2026-10-06 (Gate 1 pass); English + SEO QA reviewed by ChatGPT, revisions applied 2026-10-07 (Gate 2: Pass after revision). Publish approval pending.

Limit of this check: all pages were read through a summarizing reader, not a browser.
Two statements were checked a second time on the live DOT pages at QA (C13, C15), and
their wording is quoted below.

## Gate 1 — Factual QA (claim by claim)

Result values: `pass` = matches the recorded source; `pass (attributed)` = true only
as attributed to the named source in the text; `computed` = checked by calculation.

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | DST in the U.S. ends Sunday, November 1, 2026, at 2:00 a.m. local time | S1-1, S4-1, S6 (Nov 1, 2026 is the first Sunday of November) | pass, computed |
| C2 | At that moment clocks go back to 1:00 a.m. | S1-3 | pass |
| C3 | The hour from 1:00 to 2:00 a.m. happens twice that night | S1-3 ("one hour repeated"), follows from C2 | pass |
| C4 | DST began March 8, 2026, clocks moved from 2:00 a.m. to 3:00 a.m. | S1-1, S1-3, S6 (Mar 8, 2026 is the second Sunday of March) | pass, computed |
| C5 | Federal law runs DST from 2:00 a.m. on the second Sunday of March to 2:00 a.m. on the first Sunday of November (15 U.S.C. § 260a) | S4-1 | pass |
| C6 | In 2026 those Sundays are March 8 and November 1 | S6 | computed |
| C7 | NIST cites the Energy Policy Act of 2005 for the current rule | S1-5 | pass (attributed) |
| C8 | DOT says Hawaii, American Samoa, Guam, Northern Mariana Islands, Puerto Rico, the Virgin Islands and most of Arizona do not observe DST | S2-1 (re-read 2026-10-06; page updated Sept 3, 2025) | pass (attributed) |
| C9 | Table: Arizona "No, for most of the state" | S2-1 | pass |
| C10 | NIST's list is almost the same and does not mention the Northern Mariana Islands | S1-4 compared with S2-1 | pass (attributed) |
| C11 | NIST says the Navajo Indian Reservation is the exception in Arizona and does observe DST | S1-4 | pass (attributed) |
| C12 | DOT oversees the nation's time zones and the uniform observance of DST | S2-2, S3-1, S3-5 | pass |
| C13 | Federal law allows a state to exempt itself from observing daylight saving time by state law (revised after Gate 2; the earlier wording "and stay on standard time" was removed from the sentence; the heading "Can a state stay on standard time?" is a question, answered by the sentence below it) | S3-2 (verbatim: "States may choose to exempt themselves from observing Daylight Saving Time by State law."), S4-2. The revised sentence follows the source wording | pass |
| C14 | States do not have the authority to choose permanent DST (as DOT says) | S3-3, now confirmed verbatim on the live page (Uniform Time, updated July 15, 2026): "States do not have the authority to choose to be on permanent Daylight Saving Time." | pass (attributed) |
| C15 | DOT says it does not have the power to repeal or change DST | S3-4, verbatim on the live page: "DOT does not have the power to repeal or change Daylight Saving Time." | pass (attributed) |
| C16 | Source titles, page dates and URLs in the Sources section | S1–S4 headers (NIST updated Feb 9, 2026; DOT DST Sept 3, 2025; DOT Uniform Time July 15, 2026; govinfo statute text) | pass |

Image (`assets/optimized/daylight-saving-time-end-2026-us.png`, original SVG in
`assets/raw/`): own diagram, no photos, logos or third-party artwork. Dates (March 8,
November 1), the 2:00 a.m. times, the 1:00–2:00 a.m. hour repeating, the statute
citation and the "Hawaii, most of Arizona and several U.S. territories" line all match
C1–C8. Rendered and checked visually; no overlapping text.

### Points handled by wording, not by choosing a side

- NIST and DOT lists differ (Northern Mariana Islands; Arizona/Navajo wording). The
  draft attributes each list and states the difference. It does not merge them into one
  unattributed list.
- The article does not say whether any law to end DST is pending. It says what DOT
  states today and that the article does not track proposals (now in "Who decides").

### Not verified (and kept out of the article)

- Whether any federal or state bill to change DST is pending or likely.
- Time zones outside the U.S.; other countries' change dates.
- Individual state exemption laws beyond what DOT and the statute say in general.
- Health, safety or energy effects of the clock change.
- uscode.house.gov (under maintenance during research); govinfo text was used.

### Re-check before publish approval

Re-open S1, S2, S3 and S4 and confirm: page dates unchanged, 2026 dates unchanged, the
non-observing lists unchanged, the two DOT sentences unchanged. If anything changed,
record it here and return the draft for revision. The article must publish before
2026-11-01.

### Gate 1 verdict

Pass. No claim in the draft is unsupported by a recorded source. Draft may go to
English + SEO QA.

## Gate 2 — English + SEO QA

Reviewer: ChatGPT, on the draft text of commit `ae6c3de` (the diagram image was not
provided to the reviewer, so the text inside the diagram and its rendering were checked
by Claude only). Applied by Claude on 2026-10-07.

Result: **Pass after revision.**

Passed as written:

- The first sentence answers the search question directly.
- The whole page keeps one search intent.
- Meta description is 149 characters (limit 160); unchanged.
- US-English wording and a general-reader tone.
- Image alt text describes the diagram appropriately.

Revisions requested and applied:

| # | Finding | Change made |
|---|---|---|
| 1 | Title was 83 characters and could be cut off in search results | Title and H1 changed to "When Does Daylight Saving Time End in the U.S. in 2026?" (55 characters). Slug and focus keyword unchanged |
| 2 | "The statute lets a state exempt itself by state law and stay on standard time" was farther from the source wording than needed | Replaced with "Federal law allows a state to exempt itself from observing daylight saving time by state law." This also updates C13 above |
| 3 | The heading "Is daylight saving time ending?" could read as a claim or forecast about the rule ending, which the article does not cover | Heading removed. The DOT "no power to repeal or change" sentence and the "does not track proposals" sentence now sit in "Who decides". A new section "Can a state stay on standard time?" follows it and opens with the sentence from #2, then the DOT sentence on permanent daylight saving time |

Claude's note on #3: the reviewer's text suggested the new heading in place of the old
one, but the old section's content was about DOT's lack of power to repeal or change the
rule, which does not answer "Can a state stay on standard time?". To keep every claim
under a heading that fits it, the repeal/proposals sentences were moved into "Who
decides" and the new heading was given the state-exemption content. No claim was added
or removed, only moved or reworded; C12–C15 still hold against S2–S4.

After the revisions the page has these sections: What happens at 2:00 a.m. on
November 1; The rule behind the date; Where clocks do not change; Who decides; Can a
state stay on standard time?; Sources.

Still to confirm by the reviewer (optional): the final text after revision, and the
diagram image itself.

## Gate 3 — Publish approval

Not requested. The user approves publishing each article explicitly; this record does
not grant it.
