# QA record — usps-holiday-shipping-deadlines-2026

Article: `content/drafts/usps-holiday-shipping-deadlines-2026.md` (draft, 2026-11-13; about 1,080 body words; one H1, six H2 sections; three tables).
Brief: `research/briefs/usps-holiday-shipping-deadlines-2026.md`. Sources: `research/sources/usps-holiday-shipping-deadlines-2026.md` (S1 USPS.com page, no update date; S2 USPS release, Sept. 22, 2026; S3 USPS FAQ 000007712, Oct. 14, 2026).
Stage: **draft, Gate 1 (Claude) done 2026-11-13.** Gate 2 (ChatGPT by the user), ready, WordPress and publication are not done. **Dated post: re-read all three sources right before publishing.**

## Scope

The recommended send-by dates for delivery before Dec. 25, 2026 (Lower 48; Alaska, Hawaii, Puerto Rico and territories; international; military), the footnotes, and what "recommended" means. No prices, Post Office hours, delivery on or around Christmas, other carriers or business mailers.

## Method

After drafting, the three sources were opened again in the built-in browser (2026-11-13; USPS.com accordions expanded and read after about 4.5 seconds) and tested by script after normalization: S1 34 of 34 phrases (every date row, all nine international groups, all five military ZIP rows, footnotes 1 to 5, Hanukkah line, pickup line); S3 21 of 21; S2 10 of 10 (65 of 65). Absence tests: none of the three pages contains "media mail", "library mail" or "parcel select"; none gives a time of day for acceptance (the only clock time on S1 is the Nov. 12 maintenance banner, not used); S1 shows no update date; S3 has no Hanukkah or Kwanzaa line; S1 body has no "return". Internal link checked: the Package Pickup post returns 200 (title matches the link text); the new slug returns 404 (unpublished, no clash). 25 articles are live.

## Gate 1 — Factual QA (claim by claim)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | Lower 48: Ground Advantage Thu Dec. 17; First-Class Mail Thu Dec. 17; Priority Mail Fri Dec. 18; Priority Mail Express Sat Dec. 19; "recommended send-by dates for expected delivery before December 25" | S1; S2; S3 | pass |
| C2 | Alaska, Hawaii, Puerto Rico and territories: First-Class Dec. 17, Priority Dec. 18, Priority Mail Express Dec. 19 (weekdays Thu, Fri, Sat on S1); Ground Advantage "See below" | S1; S2; S3 | pass |
| C3 | Ground Advantage between the contiguous U.S. and AK, HI, American Samoa, PR, USVI, Guam, Northern Mariana Islands and the Freely Associated States: 10-day or more service expectation; days vary; postcalc lookup | S1; S2; S3 | pass |
| C4 | Ground Advantage to or from offshore ZIP Codes may have longer transit times and extended EDD; adjust the induction date | S1; S3 | pass |
| C5 | CBP prepayment of duties, taxes and fees and proof of payment on articles valued up to $2,500 entering the customs territory from American Samoa, Guam, the Northern Mariana Islands and the USVI; see the DMM | S1; S3 | pass |
| C6 | The FAQ labels the First-Class row "including greeting cards" | S3 | pass |
| C7 | International (nine groups, same dates): First-Class Package International Service and Priority Mail International Wed Dec. 9; Priority Mail Express International Wed Dec. 16 | S1; S3 | pass |
| C8 | The FAQ adds "including customs delays"; the USPS.com note does not | S3; S1 | pass (absence tested) |
| C9 | Military: Ground Advantage Wed Nov. 4; First-Class and Priority Mail Wed Dec. 9; Priority Mail Express Military Wed Dec. 16, N/A for ZIP 093; rows for ZIPs 090-092, 094-099, 340, 962-966 and 093 | S1; S3 | pass |
| C10 | PMEMS available to selected military and diplomatic Post Offices; check with the local Post Office | S1; S3 | pass |
| C11 | The Nov. 4 date has passed as of 2026-11-13 | date arithmetic | pass |
| C12 | The release recommends the holiday shipping page for the full military and international list beginning mid-October | S2 | pass |
| C13 | Delivery date may vary with origin, destination, Post Office acceptance time (FAQ: acceptance date and time) and other conditions; release: plan to mail early to ensure arrival by Dec. 25 | S1; S3; S2 | pass |
| C14 | Priority Mail Express guarantee notes, each scoped to its table (corrected after Gate 2): S1 footnote 5 sits on the Priority Mail Express column of the Alaska, Hawaii, Puerto Rico and territories table (as of Aug. 1, 2023, no refund requests for guaranteed service; loss refunds processed); S1 Lower 48 table has no such footnote; S3 footnote 5 sits on the same table's Priority Mail Express row ("Excluding Puerto Rico..."); S3 footnote 2 on the Lower 48 Priority Mail Express row, repeated at the top of the page, is the 1-Day Dec. 22 to 25 note, which S1 lacks; the article does not reconcile | S1; S3 | pass (DOM checked) |
| C15 | Hanukkah (Dec. 4 to Dec. 12) is earlier this year; no send-by dates specific to Hanukkah or Kwanzaa | S1; S3 | pass |
| C16 | The page points to free shipping supplies, printing labels and a free package pickup | S1 | pass |
| C17 | None of the pages gives a time of day for acceptance or Post Office hours; USPS.com shows no update date; release Sept. 22, 2026; FAQ Oct. 14, 2026 | S1; S2; S3 | pass |

## Image checks

Diagram `assets/optimized/usps-holiday-shipping-deadlines-2026.png` (1200 x 2796, sha256 prefix e776f16242409379; unchanged) and `assets/raw/usps-holiday-shipping-deadlines-2026.svg` (sha256 prefix 74da7ac525a1b0bb). Render check printed `[]`. Opened the PNG top and bottom and read every card. Card text matches C1 to C13 and C17. The file transfer tool had added C2PA provenance metadata (caBX chunk, metadata block, namespace); removed on the device and the hashes equal the files built here. Alt text in the front matter equals the alt in the body (script check).

## Format

Meta description 149 characters; title 65 characters; focus keyword `usps holiday shipping deadlines` in the title; one internal link (Package Pickup post, live); three tables, each with three columns; sources list with URLs; no prices; no photos.

## Open points for Gate 2

- Dated, time-bound content: right before publishing, re-read all three sources and report first if a date or footnote changed. A later republish should follow the same rule.
- The refund-wording difference between the USPS.com page and the FAQ is shown, not resolved.
- The military table labels ZIP 340 and 962-966 as "AE" on USPS.com; the article repeats the ZIP prefixes without the label.
- Search volume was not checked; Trends relative indexes only. The 12-month average is low; the article is chosen on seasonality (see the candidates file).

## Gate 2 FIX on `cd35086` — applied 2026-11-13 (changed parts only)

**Finding:** the Priority Mail Express refund footnote is attached on the USPS.com page to the table for Alaska, Hawaii, Puerto Rico and U.S. territories, but the draft read as a general condition.
**Scope check (2026-11-13, page markup, superscripts read in each table):** USPS.com: footnote 5 is on "Priority Mail Express Service" in the Alaska, Hawaii, Puerto Rico and territories table only; the Lower 48 table has no footnote on that row; the number 5 is also used on the military table for the PMEMS availability note (a different note). The USPS.com page has no "1-Day", "December 22" or "Excluding Puerto Rico" text (absence test); its refund sentence matches. FAQ: footnote 5 ("Excluding Puerto Rico...") is on "Priority Mail Express Service" in the Alaska, Hawaii, Puerto Rico and territories table; footnote 2 on "Priority Mail Express Service" in the Lower 48 table is the 1-Day Dec. 22 to 25 note, and the same note is repeated at the top of the page (two occurrences); footnote 2 on the military table's PMEMS is the availability note.
**Change:** the paragraph in "What "recommended" means" now says which table each note is attached to, quotes the FAQ's "Excluding Puerto Rico" sentence in full, says the Lower 48 USPS.com table has no such footnote and that the 1-Day note is on the FAQ's Lower 48 row and top of page and absent from USPS.com, and says the article does not reconcile the pages and does not apply any note outside its table. The scope was clear enough to keep the explanation. Title, tables, diagram, alt and other sections are unchanged (diagram and alt do not mention refunds).
