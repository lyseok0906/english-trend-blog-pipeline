# QA record — tsa-shoes-laptops-what-tsa-says

Article: `content/drafts/tsa-shoes-laptops-what-tsa-says.md` (draft, 2026-11-09; about 1,412 body words; one H1, six H2 sections; one table).
Brief: `research/briefs/tsa-shoes-laptops-what-tsa-says.md`. Sources: `research/sources/tsa-shoes-laptops-what-tsa-says.md` (S1 national release July 8, 2025; S2 Laptops page, July 15, 2026; S3 Steel Toe Boots page, May 26, 2022; S4 Travel Checklist, no date; S5 Tablets page, July 21, 2026; S6 Computed Tomography page, no date; S7 Juneau local release, July 13, 2026; S8 Security Screening page, no date).
Stage: **draft, Gate 1 (Claude) done 2026-11-09.** Gate 2 (ChatGPT by the user), ready, WordPress and publication are not done.

## Scope

Only what the eight TSA pages state about shoes and large electronics at the checkpoint, by lane (standard, CT, PreCheck). No belts, jackets or liquids detail, no airport list, no children or medical-need rules, no international airports, no statement about which wording controls where the pages differ.

## Method

After drafting, all eight pages were opened again in the built-in browser (2026-11-09) and tested by script after normalization (apostrophes, quotation marks, dashes, trademark signs, whitespace, lower case): 8 of 8 pages passed; the only difference found was a comma inside one Juneau-release sentence. Absence tests: the July 8, 2025 release has no "additional screening" and no "officer"; the Tablets page has no "remove", "bin" or "x-ray"; the Travel Checklist has no step about removing shoes and mentions shoes only in the packing-layers tip; the CT page shows no update date and no airport list; the Juneau release does not mention shoes. Internal links checked: the PreCheck post, the 3-1-1 post and the Media Mail post return 200; the two new slugs return 404 (unpublished, no clash). 23 articles are live.

## Gate 1 — Factual QA (claim by claim)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | July 8, 2025 national release "DHS to End 'Shoes-Off' Travel Policy": the policy allows passengers traveling through domestic airports to keep their shoes on at TSA checkpoints; subhead "Passengers can now keep their shoes on at TSA security checkpoints" | S1 | pass |
| C2 | Same release: other layered-security aspects still apply; identity verification, Secure Flight vetting and other processes | S1 | pass |
| C3 | The release does not say whether an officer can still ask for shoes to be removed or about additional screening | S1 | pass (absence tested) |
| C4 | Laptops page (Last Updated July 15, 2026): carry-on Yes, checked Yes; remove the laptop from the bag into a separate bin for X-ray screening | S2 | pass |
| C5 | Laptops page and Steel Toe Boots page (Last Updated May 26, 2022): TSA PreCheck travelers do not need to remove shoes, laptops, 3-1-1 liquids, belts or light jackets | S2; S3 | pass |
| C6 | The PreCheck sentence names shoes only for PreCheck travelers; the pages do not say how it fits with the July 2025 release (difference shown, not resolved) | S1; S2; S3 | pass |
| C7 | Travel Checklist, "In Standard Screening Lane": remove the 3-1-1 bag into the bin; empty pockets and remove bulky jewelry; remove personal electronic devices larger than a cell phone into a bin with nothing on or under them for X-ray screening (laptops, tablets, e-readers, handheld game consoles) | S4 | pass |
| C8 | The checklist lists no shoe step, shows no update date, and mentions shoes only as one layer in a bag packed in layers | S4 | pass (absence tested) |
| C9 | Tablets page (Last Updated July 21, 2026): carry-on Yes, checked Yes; FAA pointer for portable electronic devices; no instruction to take the tablet out of the bag, while the checklist names tablets | S5; S4 | pass (absence tested) |
| C10 | CT page: latest checkpoint X-ray equipment for carry-on bags; builds a 3-D image; the goal is to keep laptops and 3-1-1 liquids in the bag in the future; under current procedures for this technology laptops may remain in the bag; no update date | S6 | pass |
| C11 | Juneau release (local, July 13, 2026): two new CT machines at Juneau International Airport; passengers using them may leave laptops and other electronics in carry-ons; 3-1-1 liquids need not be removed | S7 | pass |
| C12 | Juneau release: all carry-on items including roller-bags go into a bin; slightly smaller entry tunnel; not all larger carry-ons fit; TSA recommends checking large carry-ons | S7 | pass |
| C13 | The pages do not list which airports or lanes have CT units; the Juneau release is local to one airport; the CT page and the checklist show no date | S6; S7; S4 | pass (absence tested) |
| C14 | Dating note: the Laptops page (July 15, 2026) is dated a year after the July 2025 release; the Steel Toe Boots page (May 26, 2022) is dated before it | S2; S3; S1 | pass |
| C15 | Security Screening page: TSA adjusts processes and procedures; travelers may notice changes from time to time | S8 | pass |
| C16 | Table: standard lane, CT lane and PreCheck lane rows match C4 to C12; the CT row's shoe cell says the CT pages do not address shoes (S6 and S7 have no shoe wording) | S1; S2; S4; S6; S7 | pass |

## Image check

| # | Item | Result |
|---|---|---|
| I1 | "Standard lane" card: electronics larger than a cell phone into a bin; no shoe step in the checklist matches C7, C8 | pass |
| I2 | "CT lane" card: laptops and other electronics may stay in the bag; 3-1-1 liquids need not be removed; every carry-on in a bin; sources CT page and Juneau release matches C10 to C12 | pass |
| I3 | "PreCheck lane" card matches C5 | pass |
| I4 | "Shoes: two TSA wordings" card matches C1, C5, C6 and says the pages do not say how they fit | pass |
| I5 | "Page dates" card: July 8, 2025; July 15, 2026; July 21, 2026; checklist and CT page show no date matches C4, C5, C9, C10 | pass |
| I6 | Alt text (964 characters) in front matter and body is identical and says the same as the diagram | pass |
| I7 | Files `assets/raw/tsa-shoes-laptops-what-tsa-says.svg` and `assets/optimized/tsa-shoes-laptops-what-tsa-says.png` (1200 x 2673, 458,798 bytes, sha256 8e2759c2eab874114e88d9f0c58a6a8ef90b2dcf36fd745de0b22c235a8f7d10) in the repository; no logos or photos; no text past the right margin (render check printed an empty list); footer "Sources: eight TSA pages; read Nov. 9, 2026" | pass |

## Format

Title 52 characters; slug `tsa-shoes-laptops-what-tsa-says`; meta description 150 characters; focus keyword `tsa shoes off` (the title says "TSA Shoes Off"); one H1; plain markdown table with four columns (long cells; check at 375 and 320 px at the WordPress preview, a per-post table font may be needed); two internal links (3-1-1 post, PreCheck post); no prices.

## Open points

- **P1 (source tension):** the July 2025 release against the PreCheck-only shoe sentence on the Laptops page (updated July 15, 2026). Shown, not resolved; Gate 2 may judge whether the wording is neutral enough.
- **P2 (CT scope):** the CT page has no date and no airport list; the Juneau release is local. The article attributes both and says which lane a traveler meets is not stated.
- **P3 (demand):** only Google Trends relative indexes were measured; search volume was not checked (`docs/next-candidates-2026-11-09.md`).
- **P4 (re-check):** rule-type post; re-read all eight TSA pages right before approval and before publishing, and report first if the shoes wording or the CT wording changed.

## Gate 2 FIX round 1 (base `5010b89`, applied 2026-11-09) — changed parts only

**Gate 2 requests:** (1) do not write standard screening and CT equipment as mutually exclusive lanes, and tell travelers to follow on-site instructions, in body, table, diagram and alt; (2) the PreCheck shoe wording must not read as an opposite rule for other passengers; (3) state the scope of the bin instruction (Juneau local release).

**What changed:** title now "TSA Shoes Off and Laptops Out: What TSA Says" (44 characters; "by Lane" removed); meta description 150 characters; lead and scope rewritten; table renamed "situation by situation" with a sentence that CT is equipment and PreCheck is a program and that the pages do not say how they combine; new section "On the day: the officer's instructions"; PreCheck shoe sentences rewritten (three pages, described as PreCheck wording, not a shoe rule for other passengers, with TSA's "no individual is guaranteed expedited screening"); Security Screening page's "standard screening requires that you remove all items" shown and stated not to name shoes; CT section retitled "Where CT equipment is used", with the Juneau bin, liquids, tunnel and checking-large-bags statements scoped to the two new Juneau machines; "What the pages do not say" rewritten. Diagram rebuilt (six cards: Standard screening; Where CT equipment is used; TSA PreCheck; Shoes: July 2025 release; On the day; Page dates). Alt rewritten (1,454 characters, identical in front matter and body).

**Method:** Security Screening page 10 of 10 phrases, CT page 3 of 3, Juneau release 3 of 3 tested after normalization on 2026-11-09 (all pass); absence tests on the main text (CT page: no PreCheck, no bin, no shoe, no airport names, no date; Juneau release: no PreCheck, no shoe; Security Screening page: no date). Details in `research/sources/tsa-shoes-laptops-what-tsa-says.md` (T11 to T17).

| # | Changed claim | Source | Result |
|---|---|---|---|
| F1 | Security Screening page: standard-lane electronics sentence, examples, exclusions (hair dryers, electric shavers, electric toothbrushes) | S8 | pass |
| F2 | Security Screening page: with PreCheck you do not need to remove shoes, laptops, liquids, belts and light jackets; no individual is guaranteed expedited screening | S8 | pass |
| F3 | Security Screening page: standard screening requires removing all items and placing them on the X-ray belt; the sentence does not name shoes | S8 | pass |
| F4 | Three pages (Laptops, Steel Toe Boots, Security Screening) describe PreCheck; none states a shoe requirement for other passengers; none mentions the July 2025 release (absence tested on the three PreCheck sentences and the release) | S2; S3; S8; S1 | pass |
| F5 | Security Screening page: "Listen to the instructions of the TSA officer" is in the food paragraph; an officer will be available to guide you; officers may instruct travelers to separate other items; procedures change from time to time. The article states where the sentence sits and labels the advice to follow the officer's instructions as the article's own | S8 | pass |
| F6 | CT page: further-screening sentence; current procedures let laptops remain in the bag; no bin instruction; no date | S6 | pass (absence tested) |
| F7 | Juneau release: two new CT machines at one airport; laptops and other electronics may stay in carry-ons; 3-1-1 liquids need not be removed in lanes with CT units; all carry-on items including roller bags go in a bin; smaller tunnel; TSA recommends checking large carry-ons. The article scopes these to the Juneau machines and says the pages do not say whether other airports' CT units work the same way | S7 | pass |
| F8 | The pages do not list which airports, lanes or checkpoints have CT units and do not say how CT equipment and PreCheck work together | S6; S7 | pass (absence tested) |
| F9 | Table: three rows (standard screening, CT equipment, PreCheck) match F1 to F8 and C1 to C12; the CT row attributes the laptop statement to the CT page and the liquids statement to the Juneau release | S1-S8 | pass |

Earlier claim rows C1 to C16 other than those above are unchanged. Row C16's table description and the image checks I1 to I7 are superseded by F9 and the image checks below.

**Image check (round 1):** cards match the body: Standard screening (F1, C8), Where CT equipment is used (F6, F7, T17 scope "Juneau's new CT scanners"), TSA PreCheck (F2, F4), Shoes July 2025 release (C1, C2, F4), On the day (F5, F8), Page dates (C4, C5, C9, C10, F2, F5; Steel Toe Boots May 26, 2022 added). Files in the repository: `assets/optimized/tsa-shoes-laptops-what-tsa-says.png` 1200 x 3597, 649,911 bytes, sha256 98460e2bae2a73d540101eef043a25748facd9698e8bf888d8d236fddcbc91b0 (equal to the render); `assets/raw/tsa-shoes-laptops-what-tsa-says.svg` 5,023 bytes. Render check printed an empty list (no text past the right margin). Alt equals body alt (1,454 characters).

**Open points after the FIX:** P1 now reads: the July 2025 release against PreCheck wording on three pages (shown, not resolved, wording stated as PreCheck description). P2: CT page undated and Juneau release local (stated). P3 and P4 unchanged. The article's advice to follow the officer's instructions is the writer's, marked as such; Gate 2 may judge it.

## Publication and live QA (2026-11-09)

Gate 2 re-check on `8fbce79` = PASS (user-reported). Moved to `content/ready/` (front matter `status: ready`; text unchanged). WordPress draft post 107, media 106 (original file URL used in the image block because WordPress made a `-scaled` copy of the tall image; alt saved on the media item; category Airport security rules; comments and pings closed; Rank Math description and focus keyword `tsa shoes off` set). Editor check: 26 blocks, none invalid. Phone preview: at 375 px the four-column table fits (315 px, 12 px font) and at 320 px it scrolls inside its own box (269 px in a 260 px box); no page overflow at either width (post-only table font `clamp(11px, 3.2vw, 18px)`).

**Right before publishing**, all eight TSA pages were reopened and the quoted phrases tested after normalization: release, checklist, Laptops, Tablets, Steel Toe Boots, CT, Juneau and Security Screening pages all passed (0 missing); absence tests held (the release's main text has no "officer" and no "additional screening"; the Tablets page has no removal instruction; the CT page's main text has no "PreCheck" and no bin instruction; the Juneau release has no "PreCheck" and no shoes). No change and no new conflict, so the post was published directly under the standing rule: **2026-11-09 05:30:46 UTC** (post 107).

**Live QA (logged out):** https://statesideexplained.com/tsa-shoes-laptops-what-tsa-says/ returns 200; canonical correct; title and 150-character meta description and Open Graph description match; robots index, follow; JSON-LD types present (WebSite, ImageObject, WebPage, Person, BlogPosting); one H1, eight H2, one table; no comment form and no pingback link; image returns 200, 649,911 bytes, sha256 equal to the repository file; alt 1,454 characters (equal to the draft); both internal links (3-1-1 post, PreCheck post) return 200; the Juneau scope, officer's-instructions and PreCheck sentences are present in the live text; the post is in `/post-sitemap.xml` (25 entries), `/feed/`, the home page and the category page. No indexing request.
