# QA record — daylight-saving-time-end-2026-us

Article: `content/ready/daylight-saving-time-end-2026-us.md` (moved from `content/drafts/` on 2026-10-07)
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

Approval: given by the user in chat on 2026-10-07 for this article only ("approve moving to
ready"). It is not approval of any other article and not approval to publish
automatically. The user publishes in WordPress.

Final reviewer confirmation: ChatGPT confirmed the three Gate 2 revisions on commit
`910a211` and checked the diagram (dates, times, the repeated 1:00–2:00 a.m. hour, no
clipped or overlapping text) and that the four source links open.

Pre-approval source re-check by Claude, 2026-10-07 (same reading tool as before, so the
same limit applies):

| Source | Re-check result |
|---|---|
| NIST | Updated Feb 9, 2026; 2026 dates, rule wording, non-observing list (no Northern Mariana Islands; Navajo Indian Reservation observes DST) and DOT-regulates statement unchanged |
| DOT, Daylight Saving Time | Updated Sept 3, 2025; list unchanged (includes Northern Mariana Islands, "most of Arizona") |
| DOT, Uniform Time | Updated July 15, 2026; the three quoted sentences unchanged (exemption by state law; no authority for permanent DST; no power to repeal or change DST) |
| 15 U.S.C. § 260a (govinfo) | 2:00 a.m. second Sunday of March to 2:00 a.m. first Sunday of November; state exemption by law; latest amendment Aug 8, 2005 (Pub. L. 109-58); unchanged |

One nuance recorded: the reader's summary of the DOT "Daylight Saving Time" page did not
repeat a sentence about what DOT oversees. The article's statement that DOT oversees the
nation's time zones and uniform observance of daylight saving time rests on NIST
(S1-5: regulated by DOT) and the DOT "Uniform Time" page (S3-1, S3-5), not on that
page, and is not attributed to it in the text. No change needed.

Result: no source changed. Article moved to `content/ready/`, front matter `status: ready`.

### Hand-off for publishing in WordPress (user)

- Title: When Does Daylight Saving Time End in the U.S. in 2026?
- Slug (permalink): `daylight-saving-time-end-2026-us` (stable once published)
- Category: US dates, seasons and holidays
- Meta description (149 characters): "Daylight saving time in the US ends Sunday, November 1, 2026, at 2:00 a.m. local time. See what changes, which places skip it, and who sets the rule."
- Body: start at the bold first sentence. Do not repeat the `#` title line, because WordPress shows the Title field as the page title.
- Image: upload `assets/optimized/daylight-saving-time-end-2026-us.png` and use it in the body where the markdown image line is; use it as the featured image as well. Alt text: the `image_alt` value in the front matter.
- Table under "Where clocks do not change" and the four links under "Sources" should keep their format.
- Before pressing Publish: read the preview once; publish before November 1, 2026.
- After publishing: send Claude the live URL. Claude then moves the article to `content/published/` with that URL and updates the backlog.

### After publishing (checks by Claude on the live site, with the user's browser pane)

1. The live URL opens, the title and headings are as in `content/ready/`, and the table renders.
2. The diagram loads, has the alt text from the front matter, and is not cut off on a phone-width screen.
3. Meta description and title in the page source match this record.
4. `https://statesideexplained.com/sitemap_index.xml` opens and lists the post. On 2026-10-07, before any content was published, it returned 404 while `post-sitemap.xml` and `page-sitemap.xml` returned 200; Rank Math reports that URL as the sitemap index and its sitemap module is on, so the 404 was probably caused by having no published content. This is not proven. If it is still 404 after the first post is published, treat it as a site setup problem (Rank Math sitemap settings, permalinks, cache) and fix it before publishing more posts.
5. Wordfence license registration and turning comments off (Settings → Discussion) are done before or right after this first post.
