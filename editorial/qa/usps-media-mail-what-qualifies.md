# QA record — usps-media-mail-what-qualifies

Article: `content/drafts/usps-media-mail-what-qualifies.md` (draft, 2026-11-09; about 1,300 words including the sources list; one H1, ten H2 sections; one table).
Brief: `research/briefs/usps-media-mail-what-qualifies.md`. Sources: `research/sources/usps-media-mail-what-qualifies.md` (S1 USPS.com "Mail & Shipping Services", Media Mail section, no update date; S2 Domestic Mail Manual 173 "Media Mail and Library Mail", no revision date).
Stage: **draft, Gate 1 (Claude) done 2026-11-09.** Gate 2 (ChatGPT by the user), ready, WordPress and publication are not done.

## Scope

Only what the two pages state: qualifying items, what the pages say does not qualify, inspection, the 70 lb maximum weight (USPS.com), the existence of extra fees (no amounts), delivery-time wording, enclosures and writing on the piece (DMM 4.2, 6.1 to 6.3), address and return address, the Library Mail pointer. No prices (S1 shows a starting price; not used), no Library Mail details, no international or commercial mail.

## Method

After drafting, both sources were opened again in the built-in browser (2026-11-09) and tested by script after normalization (apostrophes, quotation marks, dashes, trademark signs, whitespace, lower case): S1 18 of 18 phrases (read inside the Media Mail section) plus the footnote on service outside the contiguous U.S. and the eligibility-standards link to DMM 173; S2 26 of 26 phrases. Absence tests: DMM 173 has no "video game", no weight limit wording (no "70 lbs", "maximum weight"), no dollar amount, no revision or update date, and no "magazine" in section 4.0; S1 has no update date; the old page https://www.usps.com/ship/media-mail.htm shows "This Page Has Moved" and links to the Mail & Shipping Services page.

## Gate 1 — Factual QA (claim by claim)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | USPS.com: Media Mail is for eligible books, media and educational materials; only certain types of media; including something not allowed means you or the recipient pay higher postage | S1 | pass |
| C2 | USPS.com: all Media Mail packages are subject to opening and inspection | S1 | pass |
| C3 | USPS.com gives a maximum weight of 70 lbs; the DMM page has no weight limit wording | S1; S2 | pass (absence tested) |
| C4 | USPS.com list: eight entries (books of at least 8 pages; 16-millimeter or narrower films; printed music and test materials; video and sound recordings (tapes, albums, CDs/DVDs); playscripts and manuscripts; printed educational reference charts; medical loose-leaf pages and binders; computer-readable media) | S1 | pass |
| C5 | DMM: "Only these items may be mailed at the Media Mail prices"; books at least eight printed pages, wholly reading matter or scholarly bibliography or reading matter with incidental blank spaces for notations, no advertising other than incidental announcements of books | S2 | pass |
| C6 | DMM films: 16-millimeter or narrower, positive prints in final form for viewing; films and film catalogs sent to or from commercial theaters do not qualify | S2 | pass |
| C7 | DMM: printed music in bound or sheet form; printed objective test materials and accessories used by or on behalf of educational institutions | S2 | pass |
| C8 | DMM: sound recordings including incidental announcements and guides or scripts; video recordings and player piano rolls classified as sound recordings | S2 | pass |
| C9 | DMM: playscripts and manuscripts for books, periodicals and music | S2 | pass |
| C10 | DMM charts: single printed sheet, information conveyed primarily by graphs, diagrams, tables or other nonnarrative matter; a chart conveyed primarily by narrative text does not qualify | S2 | pass |
| C11 | DMM: medical loose-leaf pages and binders for distribution to doctors, hospitals, medical schools and medical students; computer-readable media containing prerecorded information and guides or scripts | S2 | pass |
| C12 | USPS.com note: video games, computer drives and digital drives do not qualify for Media Mail prices; the DMM does not mention video games | S1; S2 | pass (absence tested) |
| C13 | DMM: matter mailed or required to be mailed as First-Class Mail, or entered as Periodicals, is not Media Mail (3.0, worded as a condition for being mailable as Media Mail) | S2 | pass |
| C14 | Inspection: DMM 2.2 not sealed against postal inspection; mailing at Media Mail prices constitutes consent to inspection, regardless of how closed | S2 | pass |
| C15 | USPS.com: additional fees for a package that is large and lightweight, has a nonstandard size, shape or material, or has perishable items; DMM 1.2 per pound or fraction thereof, any fraction a whole pound; no amounts | S1; S2 | pass |
| C16 | Delivery time: USPS.com "Shipping in 2-8 Days" with a footnote on service outside the contiguous U.S.; DMM 2.1 does not guarantee delivery within a specified time; not reconciled | S1; S2 | pass |
| C17 | DMM 4.2 and 6.1: one envelope or one addressed postcard and one order form bound into a book; incidental announcements of books; printed matter mailable as USPS Marketing Mail may be included loose | S2 | pass |
| C18 | DMM 6.3: an invoice relating solely to the matter mailed may be inside or in an envelope marked "Invoice Enclosed" attached outside | S2 | pass |
| C19 | DMM 6.2: markings with the character of personal correspondence need additional First-Class postage, with exceptions (names and addresses, marks describing contents, instructions for use, words such as "Do Not Open Until Christmas" and "Happy Birthday, Mother") | S2 | pass |
| C20 | DMM 2.3: delivery address with the correct ZIP Code or ZIP+4; sender's return address | S2 | pass |
| C21 | Library Mail: USPS.com calls it a related service for eligible organizations (schools, museums, nonprofits and other groups); DMM 173 covers both and section 5.0 names eligible senders and addressees; not covered in the article | S1; S2 | pass |
| C22 | Neither page shows an update date; the old USPS.com Media Mail page shows "This Page Has Moved"; no prices used | S1; S2; old page | pass (absence tested) |
| C23 | Table: 9 rows match C4 to C11 | S1; S2 | pass |

## Image check

| # | Item | Result |
|---|---|---|
| I1 | "What qualifies (USPS.com list)" card lists the eight USPS.com entries matches C4 | pass |
| I2 | "Does not qualify" card: USPS.com video games, computer drives, digital drives; DMM films to or from commercial theaters and narrative-text charts; items not allowed cost higher postage matches C1, C6, C10, C12 | pass |
| I3 | "Inspection and limits" card: open to postal inspection, 70 lbs (USPS.com), extra fees for large, lightweight or nonstandard packages, no amounts matches C2, C3, C15 | pass |
| I4 | "Delivery time: the pages differ" card matches C16; footer sources, "no update dates" and read date match the article | pass |
| I5 | Alt text (1,027 characters) in front matter and body is identical and says the same as the diagram | pass |
| I6 | Files `assets/raw/usps-media-mail-what-qualifies.svg` and `assets/optimized/usps-media-mail-what-qualifies.png` (1200 x 2490, 413,796 bytes, sha256 b3ad9cdd...3ddc) in the repository; no logos or photos; text 25 to 46 px on an 800 px canvas; no text past the right margin | pass |

## Format

Title 52 characters; slug `usps-media-mail-what-qualifies`; meta description 154 characters; the focus keyword `usps media mail` appears word for word in the title; one H1; plain markdown table with three columns (long cells; check on a phone at the WordPress preview); no prices.

## Open points

- **P1 (price intent):** the head phrase "usps media mail" is probably price-driven; the article gives no price and does not link a price page. Gate 2 may judge.
- **P2 (no dates):** neither page shows a date; the article says so.
- **P3 (differences):** delivery time and the handling of video games and digital media differ between the pages; shown, not resolved.
- **P4 (length):** about 1,300 words; the enclosure and writing section is detailed and could be cut at Gate 2.
- **P5 (table on phones):** three long-cell columns; check 375 and 320 px.

## Result and next step

Gate 1: **PASS** (23 of 23 claims, 6 of 6 image checks). Next: push, Gate 2 by commit SHA. After a Gate 2 PASS under the standing rule: ready, WordPress draft, phone preview, re-read of both pages right before publishing, publish if unchanged, live QA and records.
