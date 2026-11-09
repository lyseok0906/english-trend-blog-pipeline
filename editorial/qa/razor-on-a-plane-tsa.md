# QA record — razor-on-a-plane-tsa

Article: `content/drafts/razor-on-a-plane-tsa.md` (draft, 2026-11-09; about 975 words in the body including the sources list; one H1, eight H2 sections; one table).
Brief: `research/briefs/razor-on-a-plane-tsa.md`. Sources: `research/sources/razor-on-a-plane-tsa.md` (S1 Disposable Razor, S2 Safety Razor With Blades (allowed without blade), S3 Razor-Type Blades, S4 Electric Razors; all TSA "What Can I Bring?" pages).
Stage: **draft, Gate 1 (Claude) done 2026-11-09.** Gate 2 (ChatGPT by the user), ready, WordPress and publication are not done.

## Scope

Only what the four TSA pages say about disposable razors, safety razors, razor-type blades and electric razors in carry-on and checked bags. No straight razors (TSA's own item search for "razor" returns only these four pages), no shaving cream (one pointer sentence to the published liquids post), no scissors, knives or box cutters, no airline or international rules, no battery rules for electric razors (the page points to the FAA website; no FAA page is read or used).

## Method

After drafting, the four TSA pages were opened again in the built-in browser (2026-11-09) and every statement the article relies on was tested by script after normalization: S1 4 of 4, S2 7 of 7, S3 5 of 5, S4 4 of 4. Absence statements were tested against the page text: no "cartridge", "blade", "limit", "number" or "battery" on the disposable razor page; no "limit", "number of", "straight" or "cartridge" on the safety razor page; no "straight", "limit", "number of" or "battery" on the razor-type blades page; no "batter", "lithium", "blade", "foil", "sharp", "cartridge" or "limit" on the electric razor page. The item list was searched through TSA's own filter (`all?combine=razor`): exactly four items (Disposable Razor, Electric Razors, Razor-Type Blades, Safety Razor With Blades (allowed without blade)); `combine=shav` returns only Shaving Cream (aerosol); URL guesses `straight-razor`, `straight-razors`, `safety-razor` returned 404. The diagram was rendered and read on screen (1200 x 2379 PNG) and compared with the article.

## Gate 1 — Factual QA (claim by claim)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | TSA lists disposable razors as carry-on Yes and checked Yes | S1 | pass |
| C2 | TSA lists electric razors as carry-on Yes and checked Yes | S4 | pass |
| C3 | Safety razor page: header "Carry On Bags: No" and "Checked Bags: Yes"; text: allowed through the screening checkpoint without the blade; blade must be removed before entering the checkpoint; officers are not authorized to remove the blades from the holder | S2 | pass |
| C4 | Razor-type blades: carry-on No, checked Yes; "box cutters, razor blades not in a cartridge are prohibited in carry-on" | S3 | pass |
| C5 | First answer: allowed in both for disposable and electric; safety razor allowed through the checkpoint without the blade; blades not in a cartridge prohibited in carry-on and allowed in checked bags | S1 to S4 | pass |
| C6 | Table: the four rows (carry-on and checked lines, what each page adds, page dates May 4, 2017; June 22, 2023; May 4, 2017; July 14, 2026) | S1 to S4 | pass |
| C7 | Disposable razor page: its only other instruction is that sharp objects in checked bags should be sheathed or securely wrapped; no mention of cartridges or a limit on number | S1 | pass (absence tested) |
| C8 | "So, as TSA writes it, the razor can go through the checkpoint when the blade is already out"; the page says no more about a razor that still has its blade than that officers are not authorized to take the blade out | S2 | pass (reading of the page text; no extra rule added) |
| C9 | Safety razor page repeats the wrapping line in "checked baggage" | S2 | pass |
| C10 | Razor-type blades page names only blades not in a cartridge and says nothing about blades in a cartridge | S3 | pass (absence tested) |
| C11 | Electric razors page adds "If you have questions regarding regulations, please see the FAA website."; it is the only one of the four with a 2026 date; it does not mention batteries; the article reads no FAA page | S4 | pass (absence tested) |
| C12 | The disposable, safety razor and razor-type blades pages say sharp objects in checked bags (safety razor page: "checked baggage") should be sheathed or securely wrapped to prevent injury to baggage handlers and inspectors; the electric razor page does not include that line | S1; S2; S3; S4 | pass |
| C13 | None of the four pages mentions straight razors; TSA's item search for "razor" returns exactly these four pages | S1 to S4; TSA item list | pass |
| C14 | None of the pages gives a limit on the number of razors or blades | S1 to S4 | pass (absence tested) |
| C15 | Each page says the final decision rests with the TSA officer on whether an item is allowed through the checkpoint | S1 to S4 | pass |
| C16 | Dates in the sources list: May 4, 2017; June 22, 2023; May 4, 2017; July 14, 2026; all read 2026-11-09; "three of the four pages carry dates from 2017 or 2023" | S1 to S4 | pass |
| C17 | Internal link to the 3-1-1 post: live (https://statesideexplained.com/tsa-3-1-1-liquids-rule/), title "What Is the TSA 3-1-1 Liquids Rule? What's Exempt?" matches the link text; the sentence says shaving cream has its own TSA page and is a liquids and aerosols question (no TSA text quoted) | Site; TSA item list (a "Shaving Cream (aerosol)" page exists) | pass |

## Image check

| # | Item | Result |
|---|---|---|
| I1 | Card "Disposable razor": Carry-on Yes, Checked Yes; sheathe or wrap sharp objects in a checked bag matches C1, C7, C12 | pass |
| I2 | Card "Safety razor with blades": header carry-on No, checked Yes; text allowed without the blade; blade out before the checkpoint; officers are not authorized to remove it matches C3 | pass |
| I3 | Card "Razor-type blades": carry-on No, checked Yes; box cutters and razor blades not in a cartridge prohibited in carry-on matches C4 | pass |
| I4 | Card "Electric razors": Yes, Yes; for regulation questions see the FAA website matches C2, C11 | pass |
| I5 | Card "Every page says": the final decision rests with the TSA officer matches C15; footer "four TSA What Can I Bring? pages (2017 to July 2026), read Nov. 9, 2026" matches C16 | pass |
| I6 | Alt text (779 characters) in front matter and body is identical and says the same as the cards | pass |
| I7 | Files `assets/raw/razor-on-a-plane-tsa.svg` and `assets/optimized/razor-on-a-plane-tsa.png` (1200 x 2379, 354,331 bytes, sha256 1820a334...99a7c) read back from the repository; no logos or photos; colors also named in words in the cards; text 25 to 46 px on an 800 px canvas; no overflow reported | pass |

## Format

Title 63 characters; slug `razor-on-a-plane-tsa`; meta description 156 characters; the focus keyword `can you bring a razor on a plane` appears word for word in the title only; one H1; plain markdown table (5 columns); one internal link; no prices; no search-volume numbers in the body.

## Open points

- **P1 (old pages):** three pages are dated 2017 or 2023; the article gives each date and does not call them current beyond "TSA's page says".
- **P2 (safety razor page):** its header says carry-on "No" while its text allows the razor without the blade; the article gives both as TSA wrote them and adds no rule.
- **P3 (cartridges):** the article does not say that razors with cartridges or blades in a cartridge are allowed beyond what the Disposable Razor page says; the Razor-Type Blades page only names blades not in a cartridge.
- **P4 (table width):** five columns; check the phone preview at 375 and 320 px before publishing.

## Result and next step

Gate 1: **PASS** (17 of 17 claims, 7 of 7 image checks). Next: push, Gate 2 by commit SHA (user to ChatGPT). Under the user's standing rule of 2026-11-06, after a Gate 2 PASS the file moves to `content/ready/`, a WordPress draft is made, the four TSA pages are re-read right before publishing, and the post is published if nothing changed, followed by live QA and records. If a page changed, report first.

## Gate 2, WordPress, publication and live QA (2026-11-09)

**Gate 2 (ChatGPT, base `1dd0826`): PASS**, no changes requested. Moved to `content/ready/` (`status: ready`).

**WordPress draft:** post 92, media 91 (original file URL used in the image block; PNG fetched from GitHub main and verified sha256 1820a334...9a7c, 354,331 bytes, before upload). Content hash verified in the browser before posting (e649464e...). Category 5 (Airport security rules); comments and pings closed; Rank Math focus keyword `can you bring a razor on a plane` and the 156-character description set and read back in the editor; 20 blocks, none invalid. Table font first set to `clamp(12px, 3.6vw, 18px)`: at 375 px the five-column table was 347 px wide in a 315 px box and the last column ("Page date") was cut off (it scrolled inside the table box, the page did not overflow). Changed to `clamp(11px, 3.2vw, 18px)` in the post only (the repository file has no table style; the conversion step adds it): at 375 px the table fits (315 px, 12 px text); at 320 px it is 283 px in a 260 px box and scrolls sideways inside the table box only (page scrollWidth 320, no page overflow). Block validity rechecked after the change.

**Sources re-read right before publishing (2026-11-09):** the four TSA pages unchanged (Disposable Razor: carry-on Yes, checked Yes, last updated May 4, 2017; Safety Razor With Blades: header No / Yes, text unchanged, June 22, 2023; Razor-Type Blades: No / Yes, May 4, 2017; Electric Razors: Yes / Yes, FAA sentence, July 14, 2026); TSA item search "razor" still returns exactly those four pages. No change, no conflict.

**Published:** 2026-11-09 01:06:26 UTC, https://statesideexplained.com/razor-on-a-plane-tsa/ .

**Live QA (logged out, no cache):** 200; canonical correct; title and meta description (156 characters) and og tags present, og description identical; robots index, follow; JSON-LD includes BlogPosting and WebPage; one H1; no comment form, no pingback; image served from the original upload, sha256 identical to the repository PNG, alt 779 characters; the internal link to the liquids post returns 200; five links in the body: the four TSA source links and one internal link to the liquids post; in `/post-sitemap.xml`, `/feed/`, the home page and the Airport security rules category page; table present with the `clamp(11px, 3.2vw, 18px)` style.

