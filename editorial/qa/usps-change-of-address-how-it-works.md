# QA — USPS Change of Address

Article: `content/drafts/usps-change-of-address-how-it-works.md` (draft, 2026-11-26, about 1,490 words including sources, one H1, Sources included; meta description 147 characters; alt text 1,298 characters).

Stage: draft. Gate 1 (Claude) run on 2026-11-26. Gate 2 round 1 (on `10872f5`) = FIX on the timing section; fixed in `3cf9bce`. Gate 2 round 2 (on `3cf9bce`) = FIX on the diagram card only; fixed 2026-11-26 (see below), waiting for Gate 2 on the changed parts. Backlog row 47.

## Gate 1 — claim groups
- FAQ 000005313 (Oct 15, 2026), read directly: 63 of 63 claim phrases found (one extra string was my own typo and one a page spacing artifact; both verified by reading the page).
- USPS.com Standard Forward Mail page: 30 of 30 claim phrases found.
- Live link texts match published titles: forwarding (`usps-mail-forwarding-how-long`), Informed Delivery (`usps-informed-delivery-how-it-works`) and Hold Mail (`usps-hold-mail-how-it-works`), titles read from the repository front matter; link status 200 to be confirmed in the WordPress build.
- No dollar sign or percent sign in the article (no fee amounts: the FAQ and USPS.com state them, the article does not).
- The two timing details (the 7-10 days; the temporary limits) are shown as stated; after Gate 2 round 1 they are no longer presented as conflicts (see Gate 2 fix).

## Gate 2 round 1 — FIX and what changed
Gate 2 (ChatGPT, on `10872f5`): the section "Where the USPS pages differ" wrongly treated two things as conflicts. (1) Temporary forwarding: the FAQ gives a total maximum of 364 days and, separately, a first request of up to 185 days extendable by up to 179 more days; USPS.com's "15 days up to 1 year" is not necessarily in conflict. (2) The 7-10 days: USPS.com means the time for a change to go into effect after approval; the FAQ means the time for mail to arrive after the start date; two points and two subjects.
Fix (this commit): section renamed "Two timing details the pages word differently"; the 7-10 bullet now states the two points and subjects and says the pages do not link them; the temporary bullet states the FAQ's minimum 15 days, 364-day maximum, 185 + 179 extension, 12-month total and the 45-day restart, and says the pages do not present these as conflicting. Diagram card renamed "Two timing details" and rewritten; alt text rewritten to match (front matter and Markdown alt text identical). Nothing else in the article changed.
Re-checked on the pages on 2026-11-26: FAQ 9 of 9 new phrases (15-day minimum, 364 days from the start date, 185 days, extension up to 179 days, 12-month total, 45-day restart, 7-10 postal business days of the start date, inaccessible during the period, no estimated delivery time); USPS.com 3 of 3 (once approved allow at least 7-10 business days; 15 days up to 1 year; temporary request).

## Gate 2 round 2 — FIX and what changed
Gate 2 (on `3cf9bce`): body and alt text accepted; the diagram's bottom card dropped conditions the pages state. USPS.com: "allow at least 7-10 business days" after approval ("at least" and "business" were missing); FAQ: mail starts arriving "within 7-10 postal business days" of the start date ("within" and "business" were missing). Gate 2 could not open the PNG and checked the SVG text.
Fix: the card now reads "USPS.com: allow at least 7-10 business days after approval for the change to take effect. FAQ: mail starts arriving within 7-10 postal business days of the start date." Card 4 now says "within 7-10 postal business days of the start date" as well. The alt text was changed to the same wording (front matter and Markdown alt text identical). The PNG was viewed again after rendering; no text past the right margin. Body unchanged in this round.

## Image checks
PNG 1200 x 3303 px, 608015 bytes, SHA-256 prefix `f9d7b3f46a4befa1`; SVG 6244 bytes; md 12522 bytes, `e27f325562f6095d` (after the Gate 2 fix and the round 2 card fix; before: PNG 3096 px `b7a996d9cc6a83bf`, md `dcb0a32b166e2dd8`); C2PA chunk and metadata stripped on the device. The rendering script printed no text past the right margin; the PNG was viewed. Diagram text only repeats facts from the article; alt text matches the front matter and the Markdown alt text.

## Not checked
Search volume; DMM 507.2.0; accepted photo IDs; WordPress (no draft or schedule exists); mobile and editor checks (after Gate 2 PASS); the pre-publication source re-read.
