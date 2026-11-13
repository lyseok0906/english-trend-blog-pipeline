# QA record — tsa-locks-checked-bag-what-tsa-says

Article: `content/drafts/tsa-locks-checked-bag-what-tsa-says.md` (draft, 2026-11-13; about 1,210 body words; one H1, seven H2 sections; one table).
Brief: `research/briefs/tsa-locks-checked-bag-what-tsa-says.md`. Sources: `research/sources/tsa-locks-checked-bag-what-tsa-says.md` (S1 TSA Security Screening, checked baggage section; S2 TSA Travel Tips, "TSA recognized locks"; S3 TSA Claims; none shows an update date).
Stage: **published 2026-11-13** (Gate 1 by Claude; Gate 2 FIX on `cd35086` applied in `baa6d7d`, re-check PASS on `baa6d7d`; see the sections below).

## Scope

What three TSA pages say about locking a checked bag, TSA recognized locks, locks that may be cut, TSA's stated position on the locks, inspection notices, conveyor-belt damage and claims. No prices, no lock brands or models, no firearms cases, no airline rules, no claim amounts or approval rates.

## Method

After drafting, the three pages were fetched again in the built-in browser (2026-11-13) and tested by script after normalization (apostrophes, quotation marks, dashes, trademark signs, whitespace, lower case): S1 12 of 12 phrases; S2 15 of 15; S3 16 of 16 (43 of 43). Absence tests: none of the three pages shows an update date (script search for "updated", "last reviewed", "modified" found none). The private-screening airport list was counted from the page markup: 20 airports, including San Francisco International and Kansas City International. The 404 of the TSA "whatcanibring/items/locks" URL was checked and the URL is not cited. Internal link checked: the shoes and laptops post returns 200 (title matches the link text); the new slug returns 404 (unpublished, no clash). 25 articles are live.

## Gate 1 — Factual QA (claim by claim)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | TSA screens approximately 1.3 million checked bags a day; the majority are screened without a physical bag search | S1 | pass |
| C2 | TSA may inspect checked baggage; if physically inspected, a notice of baggage inspection goes inside the bag to inform that an officer inspected it | S1; S2 | pass |
| C3 | Technology generally screens bags without opening them, but there are times TSA needs to physically inspect | S2 | pass |
| C4 | Unlocked bag: "our officer will simply open and screen the baggage" if an item alarms | S2 | pass |
| C5 | Recognized locks: TSA developed locks with several companies that officers can open with universal "master" keys so locks may not have to be cut; available at most airports and many travel stores nationwide; packaging indicates whether TSA can open them | S2 | pass |
| C6 | Security Screening names Safe Skies Luggage Locks and Travel Sentry; locks commercially available; packaging "should indicate they may be opened by TSA officers" | S1 | pass |
| C7 | Other lock: if TSA cannot open it through other means, the lock may have to be cut | S2 | pass |
| C8 | Body only (removed from the diagram and alt after Gate 2): Travel Tips says "for soft-sided baggage, this process will not damage your zippers or zipper pulls"; the article attributes it to TSA, notes that the page says nothing about hard-sided baggage or how a lock is cut, and places the liability sentence beside it | S2 | pass (absence of hard-sided tested) |
| C9 | TSA is careful not to damage belongings but is "not liable for damage caused to locked bags that must be opened for security purposes" | S2 | pass |
| C10 | TSA has no position on the validity or effectiveness of the locks as a security measure and will be forced to remove them if necessary during inspection | S1 | pass |
| C11 | Conveyor belts can damage locks and bags; 244 locks pulled from under a baggage-handling conveyor belt at a New York airport over one month | S2 | pass |
| C12 | Lost or damaged during screening: file a claim with TSA; during transport to the plane or baggage claim: contact the airline | S1; S3 | pass |
| C13 | Claims: acknowledgment letter and control number four to six weeks after submission; save the control number; FTCA governs; suit possible if denied or unresolved after six months; allow up to six months, longer with law enforcement investigation; TSA makes the final decision | S3 | pass |
| C14 | In many cases claims are denied when TSA officers did not open a bag for a physical inspection; the page points to TSA recognized locks | S3 | pass |
| C15 | Receipts, appraisals, flight information; contact the airline for lost baggage; TSA lost and found for items left at the checkpoint | S3 | pass |
| C16 | Private-company screening at certain airports; the page lists 20 airports on 2026-11-13 | S3 | pass (counted) |
| C17 | Differences shown: "may not have to be cut" against "will be forced to remove these products if necessary"; the article says it does not resolve how they fit | S1; S2 | pass |
| C18 | None of the three pages shows an update date | S1; S2; S3 | pass |

Article statements that are the article's own: the scope paragraph, the sentence that the pages do not list lock brands or models, do not say whether to lock a bag, do not say what "other means" are, and do not give approval shares. Checked by absence test where stated (no update dates).

## Image checks

Diagram `assets/optimized/tsa-locks-checked-bag-what-tsa-says.png` (1200 x 3183, sha256 prefix 7f1f1ae60617ce62) and `assets/raw/tsa-locks-checked-bag-what-tsa-says.svg` (sha256 prefix d1fcbf4e48cb20b5). Render check printed `[]` (no text beyond the right-edge limit). Opened the PNG top and bottom and read every card. Card text matches C4 to C7 and C9 to C16 (the zipper line was removed after Gate 2). The file transfer tool had added C2PA provenance metadata (a caBX chunk in the PNG, a metadata block and a namespace in the SVG); it was removed on the device and the hashes now equal the files built here. Alt text in the front matter equals the alt in the body (script check).

## Format

Meta description 146 characters; title 57 characters; focus keyword `tsa lock` in the title (as "TSA Locks"); one internal link (shoes and laptops post, live); sources list with URLs; no prices; no photos.

## Open points for Gate 2

- The Travel Tips section reads like an older first-person tip and shows no date; the article treats it as current TSA wording only as of 2026-11-13 and says no page shows a date.
- The "may not have to be cut" against "will be forced to remove" tension is shown, not resolved.
- Search volume was not checked; Trends relative indexes only (see the candidates file).

## Gate 2 FIX on `cd35086` — applied 2026-11-13 (changed parts only)

**Finding:** the diagram line "Soft-sided bags: zippers are not damaged" read as a guarantee that zippers are not damaged.
**Change:** the line is removed from the diagram and from the alt (front matter and body, equal by script check). The Travel Tips sentence stays only in the body, as a quoted TSA statement ("for soft-sided baggage, this process will not damage your zippers or zipper pulls") described as TSA's own statement about cutting a lock, with the notes that the page says nothing about hard-sided baggage and does not say how a lock is cut, followed in the same paragraph by TSA's liability sentence. "What the pages do not say" now also says the pages say nothing about hard-sided bags.
**Check against the source (2026-11-13):** the Travel Tips section was fetched again; the soft-sided sentence reads as quoted (script match); the section contains no "hard-sided", "hard shell" or "hard side" (absence test); the word "zipper" now appears only twice in the draft, both in the body paragraph (none in the diagram, alt or front matter). The "not liable" sentence was matched earlier at Gate 1 and is unchanged. Diagram rebuilt (render check `[]`, text right edge within the limit), the PNG and SVG opened and the "Other locks" card read; C2PA metadata added by the transfer tool was removed again and the hashes equal the files built here. No other claim, table, diagram card or source was changed.

## Publication and live QA (2026-11-13)

Gate 2 re-check on `baa6d7d` = PASS (user-reported). Moved to `content/ready/` (front matter `status: ready`; text unchanged). WordPress draft post 115, media 113 (original file URL used in the image block; alt saved on the media item; category Airport security rules; comments and pings closed; Rank Math description and focus keyword `tsa lock` set). The body was produced by a script from the draft on `main` and matched the local conversion by hash. Editor check: 26 blocks, none invalid; Rank Math keyword and description read back correctly. Phone preview: at 375 px the one table fits (315 px, 12 px font); at 320 px it fits (260 px, 11 px font); no page overflow (post-only table font `clamp(11px, 3.2vw, 18px)`).

**Right before publishing**, the three TSA pages were re-read and tested after normalization: Security Screening 12 of 12, Travel Tips 15 of 15, Claims 16 of 16 (43 of 43), 20 airports on the claims list, no update date on any page, no "hard-sided" wording. No change and no new conflict, so the post was published directly under the standing rule: **2026-11-13 02:29:55 UTC** (post 115).

**Live QA (logged out):** https://statesideexplained.com/tsa-locks-checked-bag-what-tsa-says/ returns 200; canonical correct; title, 146-character meta description and Open Graph description match; robots index, follow; JSON-LD types present (BlogPosting among them); one H1, eight H2 (seven in the draft plus one theme heading), one table; no comment form and no pingback link; image returns 200, sha256 equal to the repository file (7f1f1ae60617ce62...); alt 1,325 characters (equal to the draft); the internal link (shoes and laptops post) returns 200; the liability sentence, the soft-sided quote, the "20 airports" sentence, the two master-key programs and the hard-sided note are present in the live text; the removed diagram line is absent from the live text; the post is in `/post-sitemap.xml`, `/feed/`, the home page and the Airport security rules category page.
