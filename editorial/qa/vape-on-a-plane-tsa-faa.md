# QA record — vape-on-a-plane-tsa-faa

Article: `content/drafts/vape-on-a-plane-tsa-faa.md` (draft, 2026-11-06; about 1,100 words in the body including the sources list, one H1, seven H2 sections; one table).
Brief: `research/briefs/vape-on-a-plane-tsa-faa.md`. Sources: `research/sources/vape-on-a-plane-tsa-faa.md` (S1 TSA, S2 FAA PackSafe, S3 FAA news item of Jan. 17, 2020, S4 49 CFR 175.10(a)(19)).
Stage: **draft, Gate 1 (Claude) done 2026-11-06.** Gate 2 (ChatGPT by the user), ready, WordPress and publication are not done.

## Scope

Only what the four sources state about vapes, e-cigarettes and similar devices; no airline rules, other countries, cannabis, age limits, e-liquid or disposable vapes as a category (no page read states a rule for them); the 2020 FAA statement on use on board is attributed and dated and no regulation is named for it.

## Method

After drafting, the four sources were opened again in the built-in browser (2026-11-06) and every statement the article relies on was tested by script after normalization: TSA page 8 of 8, FAA PackSafe page 16 of 16, FAA news item 7 of 7, eCFR paragraph (a)(19) 7 of 7. Absence claims were tested by searching the page texts for e-liquid, e-juice, refill, cartridge, disposable and pods (no match on the TSA page, the FAA page or the news item), for "checked" on the FAA page (no match), and for "CFR" or "regulation" in the news item (no match). The diagram was rendered and read on screen (1200 x 2103 PNG) and compared with the article.

## Gate 1 — Factual QA (claim by claim)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | TSA lists carry-on "Yes (Special Instructions)" and "Checked Bags: No" | S1 | pass |
| C2 | TSA: electronic smoking devices are allowed only in carry-on baggage | S1 | pass |
| C3 | FAA: the devices must be carried on one's person or in carry-on baggage; the regulation says the same with "only" | S2; S4 | pass |
| C4 | TSA and FAA: passengers are required to take effective measures to prevent accidental activation of the heating element; TSA points to the FAA regulations for examples | S1; S2 | pass |
| C5 | FAA describes the devices as battery powered with a heating element that vaporizes liquid | S2 | pass |
| C6 | FAA's five examples (remove the battery; separate the battery from the heating coil; protective case; protective cover, safety latch or locking device on the heating coil activation button; electronics designed to prevent accidental activation, such as power-on before the coil button works), introduced as "include, but are not limited to" | S2 | pass |
| C7 | Spare lithium batteries: on one's person or in carry-on baggage only (FAA, regulation), individually protected against short circuits | S2; S4 | pass |
| C8 | The FAA's six methods (retail packaging, tape over terminals, battery case, battery sleeve in a camera bag, snugly in a plastic bag, protective pouch) | S2 | pass |
| C9 | TSA, FAA and the regulation: each lithium ion battery 100 Wh or less; each lithium metal battery 2 grams of lithium or less | S1; S2; S4 | pass |
| C10 | FAA and the regulation: recharging the devices or batteries on board is not permitted | S2; S4 | pass |
| C11 | FAA news item, January 17, 2020: devices considered hazardous materials when transported on aircraft; contain lithium batteries that pose a fire risk (stated as two separate sentences, no causal link added); vapes, e-cigarettes and spare lithium batteries in carry-on luggage only | S3 | pass |
| C12 | FAA news item: just as passengers are not allowed to smoke cigarettes on an aircraft, they should never use their vapes or e-cigarettes on an aircraft; "a federal offense"; the item cites no regulation | S3 (no "CFR" or "regulation" in the text) | pass |
| C13 | TSA and FAA: check with the airline on any limits on the number of devices; neither gives a number | S1; S2 | pass |
| C14 | None of the pages mentions e-liquid or refill bottles or names disposable vapes | S1; S2; S3 | pass (absence tested) |
| C15 | The FAA page does not say "checked bag"; TSA is the only source that says "Checked Bags: No" in words (the table row on checked bags attributes accordingly) | S2 vs S1 | pass |
| C16 | TSA: the officer makes the final decision on whether an item goes through the checkpoint | S1 | pass |
| C17 | Dates: TSA "Last Updated on March 29, 2023"; FAA "Last updated: Monday, April 13, 2026"; FAA news "Friday, January 17, 2020"; eCFR "up to date as of 11/04/2026"; all read 2026-11-06 | S1 to S4 | pass |
| C18 | The article names the covered devices as vapes, e-cigarettes, vape pens and similar devices; the regulation's list (e-cigars, e-pipes, e-hookahs, personal vaporizers, electronic nicotine delivery systems) and the FAA's list (vaporizers, atomizers) are not claimed as exhaustive | S2; S4 | pass |
| C19 | Internal link to the power bank post for spare batteries in general: the target is live (https://statesideexplained.com/power-bank-on-a-plane-tsa-faa/) and its title matches the link text | Site | pass (checked 2026-11-06) |

## Image check

| # | Item | Result |
|---|---|---|
| I1 | Card 1 "Carry-on bag or on your person: Allowed. TSA: Yes (Special Instructions). Take measures so the heating element cannot turn on by accident." matches C1, C3, C4 | pass |
| I2 | Card 2 "Checked bag: Not allowed. TSA: Checked Bags: No." matches C1, C2 (the FAA page itself does not say "checked"; the card attributes the words to TSA) | pass |
| I3 | Card 3 spare batteries matches C7, C9 | pass |
| I4 | Card 4 "No recharging ... FAA (2020): passengers should never use a vape or e-cigarette on an aircraft." matches C10, C12 | pass |
| I5 | Card 5 "Number of devices: Check with your airline (TSA and FAA)." matches C13 | pass |
| I6 | Footer sources and dates match C17; alt text (727 characters) says the same as the card text and the body | pass |
| I7 | Files `assets/raw/vape-on-a-plane-tsa-faa.svg` and `assets/optimized/vape-on-a-plane-tsa-faa.png` (1200 x 2103, 336,363 bytes, sha256 9dccb82b...5df81) read back from the repository; no logos or photos; colors also labeled in words; text 25 to 46 px on an 800 px canvas | pass |

## Format

Title 59 characters; slug `vape-on-a-plane-tsa-faa`; meta description 143 characters; the focus keyword `can you bring a vape on a plane` appears word for word in the title only (the first paragraph answers the question without repeating the phrase); one H1; plain markdown table; one internal link; no prices or search-volume numbers in the body.

## Open points

- **P1 (2020 statement):** the use-on-board sentence rests on a 2020 FAA news item that cites no regulation; the article says so. Gate 2 may ask for it to be dropped; it can go without breaking anything else (table row, section "Charging and use on board", diagram card 4).
- **P2 (TSA page age):** TSA's page is dated March 29, 2023; it agrees with the FAA page of April 13, 2026 and the regulation on every point it states.
- **P3 (scope):** e-liquid and disposable vapes are out because no page read addresses them; the article says so in one sentence.

## Result and next step

Gate 1: **PASS** (19 of 19 claims, 7 of 7 image checks). Next: push, Gate 2 by commit SHA (user to ChatGPT). Under the user's standing rule of 2026-11-06, after a Gate 2 PASS the file moves to `content/ready/`, a WordPress draft is made, all four sources are re-read right before publishing (TSA page, FAA PackSafe page, FAA news item, eCFR 175.10(a)(19)), and the post is published if nothing changed, followed by live QA and records. If a source changed or the sources now conflict on a point the article states, report first.

---

## Gate 2, pre-publication check, publication and live QA (2026-11-06)

**Gate 2 (ChatGPT, base `bed1e85`, user-reported 2026-11-06): PASS**, no change requested. Gate 1 and Gate 2 were not repeated.

**Move to ready and WordPress draft (under the user's standing rule of 2026-11-06):** file moved to `content/ready/` with `status: ready`; image fetched from the repository (GitHub raw, main) and verified by hash before upload (sha256 9dccb82b...5df81, 336,363 bytes); media 84 (alt text set, 727 characters, identical to the front matter); WordPress draft post 85 (category Airport security rules, comments and pings closed); Rank Math focus keyword `can you bring a vape on a plane` and description (143 characters) set and read back in the editor; 18 blocks, none invalid; typed content verified by SHA-256 before posting; table block set with the responsive font size used on the other posts.

**Phone preview (draft, logged in):** 375 px and 320 px: no horizontal overflow, image visible, table within the page width.

**Pre-publication source check (2026-11-06, minutes before publishing): no change.**

| Source | Result |
|---|---|
| S1 TSA page | text identical in all relied-on parts (Carry On Bags: Yes (Special Instructions); Checked Bags: No; carry-on only; accidental activation; 100 Wh / 2 grams; airline limit on the number of devices; final decision with the officer); page still shows "Last Updated on March 29, 2023" |
| S2 FAA PackSafe page | unchanged (carry-on or on one's person; battery-powered with heating element; five example measures; spare batteries and six methods; 100 Wh / 2 grams; no recharging; airline check; cites 49 CFR 175.10(a)(19)); still "Last updated: Monday, April 13, 2026" |
| S3 FAA news item | unchanged (Jan. 17, 2020; hazardous materials; fire risk; carry-on only; never use on an aircraft; "federal offense"; no "CFR" or "regulation" in the text) |
| S4 eCFR 175.10(a)(19) | paragraph text identical; "up to date as of 11/04/2026"; Title 49 last amended 10/28/2026 |

No source conflict; no regulation change.

**Published:** 2026-11-06 08:24:50 UTC (site time 03:24:50) by Claude under the standing rule. Post 85, media 84. URL https://statesideexplained.com/vape-on-a-plane-tsa-faa/. No indexing request.

**Live QA (logged out, no-store fetch): PASS.** 200; canonical is the post URL; title "Can You Bring a Vape on a Plane? What TSA and the FAA Say - Stateside Explained"; meta description 143 characters, og:description identical; robots index, follow; JSON-LD WebSite, WebPage, Person, ImageObject and BlogPosting; one H1, eight H2; no comment form and no pingback link; image served from `/wp-content/uploads/2026/11/vape-on-a-plane-tsa-faa.png`, hash 9dccb82b...5df81 identical to the repository, alt 727 characters; the internal link to the power bank post returns 200 and four official source links are present; the live text contains the checked sentences (including the statement that the 2020 item cites no regulation and the e-liquid and disposable absence statement); post is in `/post-sitemap.xml` (18 URLs), in `/feed/` and on the home page; phone width 375 px: no horizontal overflow. Counts: 18 live (12 pilot, 6 post-pilot).

**Open:** none for this post. Re-read the four sources if the article is revisited.
