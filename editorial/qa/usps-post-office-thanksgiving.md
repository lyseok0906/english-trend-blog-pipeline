# QA record — usps-post-office-thanksgiving

Article: `content/drafts/usps-post-office-thanksgiving.md` (draft, 2026-11-18; about 610 words in the body, one H1, four H2 sections including Sources; one table; two internal links).
Brief: `research/briefs/usps-post-office-thanksgiving.md`. Sources: `research/sources/usps-post-office-thanksgiving.md` (S6 USPS national release of Nov. 17, 2026; S2 Holidays and Events page).
Stage: **draft, Gate 1 done by Claude 2026-11-18; waiting for Gate 2.** Rule/schedule-type post: re-read the release and the Holidays and Events page right before any publishing.

## Scope as set by the user (2026-11-18)

- Explain the closure on Thursday, November 26 and the resumption on Friday, November 27 from the **Nov. 17, 2026** release.
- **Priority Mail Express delivery on Thanksgiving Day is not confirmed by the notice**: the article says the notice does not say, either way, and does not fill the gap.
- **The 2025 notice (S4) is not applied to 2026**: it is not quoted, compared or used. The article only says it does not use notices from earlier years.
- No search volume, Trends figure or advice. Search volume was not checked.

## Method

The release page was opened in the built-in browser on 2026-11-18 and every statement the article makes was tested by script after normalization (20 of 20 phrase checks, page text 2,998 characters after whitespace normalization). "Priority Mail Express", "deliver", "hours" and times, "deadline" and similar words, and "lobb" were listed occurrence by occurrence. The Holidays and Events page was read the same way. The diagram was rendered (1200 x 1980 PNG) and read on screen. The two internal links were opened logged out (200). The 2025 notice was not used.

## Gate 1 — Factual QA (claim by claim)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | USPS will observe the Thanksgiving federal holiday on Thursday, November 26, 2026 | S6 "will observe the Thanksgiving federal holiday on Thursday, November 26" (year from the release date) | pass |
| C2 | All Post Office locations will be closed | S6 | pass |
| C3 | Regular mail delivery and retail services will resume on Friday, November 27 | S6 | pass |
| C4 | The statements come from a USPS national release dated November 17, 2026 | S6 page date "Nov. 17, 2026", label "National news"; RSS item dated Tue, 17 Nov 2026 13:36 -0500 | pass |
| C5 | Release title "U.S. Postal Service To Observe Thanksgiving Holiday, Nov. 26", published in the USPS Newsroom (the RSS title differs: "USPS to close for Thanksgiving holiday on Nov. 26"; the article uses the page title) | S6 page title | pass |
| C6 | The Holidays & events page lists Thursday, November 26, 2026 as Thanksgiving Day and does not say open or closed | S2 ("2026 holidays": Wed Nov 11 Veterans Day; Thu Nov 26 Thanksgiving Day; Fri Dec 25 Christmas Day; no open/closed wording for them) | pass |
| C7 | Subtitle: self-service options are available in many retail lobbies when Post Offices are closed | S6 "Self-service options are available in many retail lobbies when Post Offices are closed" | pass |
| C8 | On usps.com customers can order stamps and free USPS boxes and use Hold Mail, Change of Address, PO Box rental or renewal, and Click-N-Ship to print prepaid labels | S6 ("pre-paid labels" in the source; the article writes "prepaid") | pass |
| C9 | Self-service kiosks are available in select lobbies nationwide | S6 | pass |
| C10 | Kiosk features: postage printing for Priority Mail, Priority Mail Express and international shipping; stamps for purchase; weighing and mailing packages; package tracking information | S6 (the four bullet items) | pass |
| C11 | As USPS modernizes its retail locations, more self-service options are becoming available at more locations and may include Rapid Dropoff Stations (customers who already printed labels), printing a shipping label from a merchant-provided QR code, and USPS Smart Lockers for drop-off and pick-up | S6 ("created and printed labels online" shortened to "already printed labels") | pass |
| C12 | Many kiosks are available 24/7 | S6 "Many self-service kiosks are available 24/7" | pass |
| C13 | The release does not name the lobbies that have kiosks | S6: "lobb" occurs twice (subtitle and kiosk sentence); no location named | pass |
| C14 | The notice does not say whether Priority Mail Express will be delivered on November 26, either way; its only mention is the kiosk postage-printing list, which is not a delivery statement | S6: "Priority Mail Express" occurs once (kiosk list) | pass |
| C15 | The notice does not list hours for any individual Post Office or lobby | S6: no times, "hour" or "hours" | pass |
| C16 | Apart from the resumption date, the notice does not describe delivery on November 26 | S6: "deliver" occurs twice, in the resumption sentence and the boilerplate ("secure delivery of mail and packages") | pass |
| C17 | The notice does not give mailing deadlines | S6: no "deadline", "mail by", "ship by", "send by" or "recommended" | pass |
| C18 | Weekdays: November 26, 2026 is a Thursday and November 27 a Friday | Calendar (also stated by S6) | pass |
| C19 | "As of November 18, 2026" and "checked on November 18, 2026" | Read date | pass |
| C20 | Source URLs | S6 URL opened (title matches); S2 URL opened | pass |
| C21 | Internal links: `/usps-hold-mail-how-it-works/` (Hold Mail, one of the listed services) and `/usps-holiday-shipping-deadlines-2026/` (recommended Christmas mailing dates) | Both return 200 logged out; the holiday deadlines article does not mention Thanksgiving, so no overlap or conflict | pass |
| C22 | Earlier years' notices are not used | The article contains no 2025 date, quote or comparison | pass |

## Image check

| # | Item | Result |
|---|---|---|
| I1 | Card 1 "Thursday, November 26 / USPS will observe Thanksgiving. All Post Office locations will be closed." matches C1, C2 | pass |
| I2 | Card 2 "Friday, November 27 / Regular mail delivery and retail services will resume." matches C3 | pass |
| I3 | Card 3 "While Post Offices are closed / The notice points customers to usps.com (stamps, Hold Mail, Change of Address, Click-N-Ship) and to self-service kiosks in select lobbies." matches C8, C9 | pass |
| I4 | Card 4 "Not in the notice / Whether Priority Mail Express is delivered on November 26: the notice does not say, either way." matches C14 | pass |
| I5 | Footer "Source: USPS national release, Nov. 17, 2026" matches C4 | pass |
| I6 | No logos, photos or USPS marks; red closed card and green resume card also labeled in words; text at 28 to 46 px on an 800 px canvas; no text past the right margin (script check `[]`); the first render had the footer touching the last card, fixed by lengthening the canvas to 1320 px | pass |
| I7 | Alt text (about 640 characters) says the same as the diagram and the body (alt equals the body image text; SVG `<title>` the same) | pass |
| I8 | Files in the repository: `assets/optimized/usps-post-office-thanksgiving.png` (1200 x 1980, 308,403 bytes, sha256 `ccfd2837cb26a20d...`), `assets/raw/usps-post-office-thanksgiving.svg` (3,292 bytes, `e86a1e8ebdf2e83a...`); the C2PA chunk the transfer added was removed on the device and the hashes read back equal the originals | pass |

## Front matter and format

Title 63 characters; slug `usps-post-office-thanksgiving`; meta description 145 characters ("USPS's Nov. 17, 2026 notice says all Post Office locations are closed Thursday, Nov. 26, and regular delivery and retail services resume Nov. 27."); focus keyword `is the post office open on thanksgiving` appears word for word in the title only (as in the Veterans Day article; noted for Gate 2); category Postal service and stamps; no price or dollar amount; no `[[HOLD` marker left (0). The skeleton's `status` line was replaced by `draft`.

## Open points for Gate 2

- **P1 (Priority Mail Express):** the article says the notice does not say, either way, and uses no other source. The 2025 notice said "only Priority Mail Express will be delivered that day"; it is not used here, as the user directed.
- **P2 (timing):** Thanksgiving is Thursday, November 26. Gate 2, publishing and indexing leave little time; the site's crawl pace has been slow (see the Veterans Day QA). After the holiday the article remains a dated record.
- **P3 (scope):** the article includes the notice's usps.com and kiosk paragraphs (the Veterans Day article omitted them at the user's request). If the reviewer prefers the shorter form, the "What USPS lists while Post Offices are closed" section can be cut without affecting the rest.
- **P4 (links):** two internal links (Hold Mail, holiday shipping deadlines). The Veterans Day article is not linked; it can be added if the reviewer wants the pair connected.
- **P5 (release subtitle vs text):** the subtitle says "many retail lobbies" and the kiosk sentence says "select lobbies nationwide"; the article quotes both and does not reconcile them.
- **P6 (before publishing, mandatory):** re-read the release and the Holidays and Events page; if the release is corrected or a new notice appears, report before publishing.

## Result and next step

Gate 1: **PASS** (22 of 22 claims, 8 of 8 image checks). Next: user push, Gate 2 by commit SHA, then approval to move to `ready`; before publishing, re-read the release and the events page and record the result; WordPress only after the Gate 2 PASS.
