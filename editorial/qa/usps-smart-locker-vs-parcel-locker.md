# QA record — usps-smart-locker-vs-parcel-locker

Article: `content/ready/usps-smart-locker-vs-parcel-locker.md` (moved from `content/drafts/` on 2026-11-24; published as post 165; written as a draft on 2026-11-24, about 2,220 words in the body, one H1, ten H2 sections including Sources; meta description 148 characters; alt text 839 characters).
Brief: `research/briefs/usps-smart-locker-vs-parcel-locker.md`. Sources: `research/sources/usps-smart-locker-vs-parcel-locker.md` (S1 to S9, all read 2026-11-24).
Stage: **published 2026-11-24 (post 165)**. Gate 1 (Claude) run on 2026-11-24. **Gate 2 round 1 (ChatGPT, base `6ddb13c`, user-reported 2026-11-24): FIX, one item (Priority Mail Express count), applied 2026-11-24** (section "Gate 2 FIX round 1"); **Gate 2 round 2 (base `7dd55bb`, user-reported 2026-11-24): FIX, one item (lower diagram card), applied 2026-11-24** (section "Gate 2 FIX round 2"); **Gate 2 round 3 (changed part only, base `3bb374d`, user-reported 2026-11-24): PASS.** Backlog row 42.

## Scope as approved by the user (2026-11-24)

- USPS Smart Locker, approved as the second post of the day, with the difference from a general parcel locker, the hold periods and the conditions of each feature checked on official pages, and a comparison with the redelivery and PO Box posts.
- The relative index of "usps parcel locker" is **not** presented as Smart Locker interest alone; search volume is "not checked". No Trends figure or volume claim appears in the article (Trends are only in the brief and in `docs/next-candidates-2026-11-24.md`).
- Reframing reported to the user: the title and keyword follow the phrase people search ("usps parcel locker") and the article separates three kinds of locker (Smart Locker, gopost, cluster box parcel locker), so the "Smart Locker versus general parcel locker" question is answered on the pages' own words.
- No prices or fees (the Local XChange flat fee is mentioned once without an amount), no locker locations, no business integrations.

## Method

All nine sources were opened in the built-in browser on 2026-11-24 and every statement was tested by script. Normalizer: remove marks and quotation marks, map dashes to a hyphen, collapse whitespace, lowercase; on faq.usps.com pages a single digit glued after a letter or a closing parenthesis was also stripped (footnote markers). Page text was taken from `main` or `body` without style, script, nav, header or footer. A phrase passed when the normalized page text contained the normalized phrase.

| Source | Phrase checks | Matched at once | Notes |
|---|---|---|---|
| S1 FAQ Smart Locker (000008414) | 53 | 52 | miss: my paraphrase "you scan it" (page: "you can scan it"); the article sentence is mine and accurate |
| S2 FAQ Cluster Box / Parcel Locker (000006975) | 10 | 10 | no "days" text on the page (hold-time absence check) |
| S3 FAQ gopost (000007973) | 20 | 20 | |
| S4 USPS.com recipients | 18 | 18 | |
| S5 USPS.com shippers | 8 | 8 | |
| S6 USPS.com Local XChange | 9 | 9 | |
| S7 FAQ Redelivery - The Basics (000005320) | 7 | 7 | |
| S8 FAQ PS Form 3849 (000006180) | 6 | 6 | |
| S9 FAQ Second and Final Notice (000006169) | 4 | 4 | |
| Total | 135 | 134 | |

## Gate 1 — Factual QA (claim by claim)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | Lead: Smart Locker is in a Post Office lobby and opens with a one-time QR code | S1 | pass |
| C2 | Lead: gopost needs a registered account, a card and a PIN | S3 | pass |
| C3 | Lead: a parcel locker in a cluster box unit opens with a key the carrier leaves in the mailbox | S2 | pass |
| C4 | Lead: for packages other than Priority Mail Express, Smart Locker 5 calendar days in the locker, 10 more at the retail counter, return to sender 15 days after the first notification; Priority Mail Express has its own count (FAQ: returned to the sender 5 calendar days after the first delivery attempt; USPS.com: after 5 days in the locker) | S1, S4 | pass (FAQ: 5 + 10; S4: "15 days after the initial notification"; the Priority Mail Express note is in S1 and S4, re-read after round 1) |
| C5 | Article states the Smart Locker pages' scope: date as of Nov. 24, 2026; FAQ dates Jul 28, Aug 4, Oct 22, 2026; Redelivery FAQ Sep 16; PS Form 3849 FAQ Jun 29; return-dates FAQ Apr 7; USPS.com pages show no update date | S1 to S9 | pass |
| C6 | Table: Smart Locker in Post Office lobbies | S1 | pass |
| C7 | Table: gopost near certain Post Offices, grocery stores, pharmacies, transportation hubs and more | S3 | pass |
| C8 | Table: cluster box locker in a CBU, beside neighborhood delivery and collection box units, or with PO Boxes in a retail facility | S2 | pass |
| C9 | Table: gopost opens with card and PIN; USPS.com account then authentication | S3 | pass |
| C10 | Table: no account step named for Smart Locker pickup; cluster box account "not described" | S1, S2 | pass (absence check) |
| C11 | Table: Smart Locker "Other packages: 5 days in the locker, 10 more at the counter. Priority Mail Express: 5 days, counted from the first delivery attempt (FAQ) or in the locker (USPS.com)"; gopost up to 15 days, 5 for Priority Mail Express; cluster box time "not stated" | S1, S4, S3, S2 | pass |
| C12 | Smart Locker described as "electronic" and "keyless" and a "free, secure, and convenient" alternative | S1 | pass |
| C13 | gopost units "automated, secured, self-service parcel lockers" | S3 | pass |
| C14 | Cluster box FAQ definition of a parcel locker | S2 | pass |
| C15 | Three routes to a Smart Locker: store checkout, individual sender with Click-N-Ship or kiosk and recipient email, redelivery | S1, S4 | pass |
| C16 | Redelivery to a locker via usps.com/redelivery, option appears only if the local Post Office has a Smart Locker, cannot be scheduled for another location | S1 | pass |
| C17 | Smart Locker not available when redelivery is requested by phone | S7 | pass |
| C18 | Eligible services: Ground Advantage, Priority Mail Express, Priority Mail (and Return services), Media Mail; commercial also Bound Printed Matter and Library Mail | S4, S5 | pass |
| C19 | Domestic only, "No cards, letters, or anything that requires a customs form." | S4 | pass |
| C20 | Sender needs the recipient email; notice and QR code go there | S4, S1 | pass |
| C21 | Absolute maximum 22.5 x 18 x 16.5 inches, some lockers smaller (USPS.com); FAQ: maximum varies by locker, 70 pounds | S4, S5, S1 | pass |
| C22 | A package that cannot go to a locker is held at the retail counter with an email | S1 | pass |
| C23 | Informed Delivery Daily Digest: email address must match; tracking beginning within 3 days; a note and a one-time QR code expiring after 5 calendar days | S1 | pass (one phrase, "stays until pickup", is my wording for the FAQ sentence; noted for Gate 2) |
| C24 | Pickup email contents; scan at the kiosk; final email; 5 calendar days with daily reminders; QR code may be shared with a trusted person | S1 | pass (miss "you scan it" is paraphrase) |
| C25 | After 5 days: removed, held at the retail window 10 more days, acceptable identification; S4 gives the same timeline and return at 15 days after the initial notification | S1, S4 | pass |
| C26 | Local XChange section of the FAQ: at 15 days treated as Undeliverable as Addressed and mailed back to the seller | S1 | pass (wording kept to that section, not to the recipient timeline) |
| C27 | QR code not received: deleted or junk email, Post Office during retail hours, 1-800-ASK-USPS to resend; not scanning: brighten and clean the screen or enter the six-digit access code; a USPS employee can help | S1 | pass |
| C28 | Hours: many 24/7, lobby hours in the pickup email, After Hours Access free at select Post Offices where the lobby is not open around the clock | S1 | pass |
| C29 | Local XChange page: "many" kiosks 24/7, "some are only available during lobby hours" | S6 | pass |
| C30 | Returns from a Smart Locker with a Label Broker QR code: scan to print a label, attach, scan the new label, put the package in a compartment | S1 | pass |
| C31 | Local XChange conditions: free USPS.com account, locker within 50 miles of the return address, buyer name and valid email, box or polybag that fits; flat fee mentioned and not repeated | S6 | pass |
| C32 | Local XChange FAQ: 5 + 10 days, mailed back at 15 days after the initial notification; label cannot be refunded once scanned at the kiosk | S1 | pass |
| C33 | Ineligible items: cremated remains, live animals, day-old poultry, perishables, hazmat affected by extreme temperature, "Restricted Matter"; seller and buyer cannot use the same contact information | S1 | pass |
| C34 | gopost registration: free USPS.com account; authentication by scanning a driver's license or state ID at a unit, or a government-issued photo ID at a Post Office; account number, card, PIN; no specific locker assigned; 24/7 "as long as the gopost unit is operational and available to the public" | S3 | pass |
| C35 | gopost address uses name, account number and the unit's address; 15 days (5 for Priority Mail Express), then returned; not accepted: Certified Mail, Registered Mail, Adult Signature, Restricted Delivery ("including") | S3 | pass |
| C36 | Cluster box: parcel locker for items too large for an individual compartment; key in the mailbox with a tag; the key stays in the locker; accountable mailpieces to the point of address; no hold time | S2 | pass (absence check) |
| C37 | Link sentence to the tracking status post: its guide's version of the key rule | published post 128 (not re-read here) | open for Gate 2: compared with the post text at drafting time |
| C38 | PO Box link sentence: an oversized package goes either to the counter by slip or to a secure parcel locker, including USPS Smart Lockers at select locations | published PO Box post (88), which cites USPS.com | open for Gate 2: depends on the published post; not re-read on USPS.com in this check |
| C39 | PS Form 3849: February 2021 version "Parcel Locker Eligible" for a gopost parcel locker; September 2022 version "USPS Smart Locker Eligible"; earlier versions still in use | S8 | pass |
| C40 | Redelivery FAQ: "Parcel Locker Eligible" if eligible for gopost Parcel Locker Delivery (limited ZIP Codes); also checked if the "USPS Smart Locker" option is available | S7 | pass |
| C41 | PME: S4/S5 "after 5 days in the locker: Priority Mail Express packages will be immediately returned to sender"; S1 "returned to sender 5 calendar days after the initial delivery attempt, no matter when the 'USPS Smart Locker' option is selected"; S9 table: Priority Mail Express "5 days after first attempt" and held 5 days before return; the article says the pages give different starting points (first delivery attempt in the FAQs, time in the locker on USPS.com), does not say which applies, and tells a reader near the deadline to ask the Post Office that holds the package | S4, S5, S1, S9 | pass (re-read on 2026-11-24 after round 1) |
| C42 | Hours difference: S4 "anytime, anywhere" against lobby hours in S1 and S6 | S4, S1, S6 | pass |
| C43 | Size difference: 22.5 x 18 x 16.5 (S4, S5) against maximum compartment 22.5 x 19.5 x 14.5 (S6); FAQ: varies by locker, Click-N-Ship shows the limit | S4, S5, S6, S1 | pass |
| C44 | "What the pages do not say": locker count, free-locker check, tell-apart on older notices, cluster box hold time, ID check at the locker, treatment of a shared QR code | S1 to S9 | pass (absence checks on the pages read) |

## Image checks

- After round 2: PNG 1200 x 3504 px, 668,658 bytes, SHA-256 prefix `cd8f61ee8cd7901f`; SVG 6,281 bytes, `e0db9681822c4739`; md 16,669 bytes, `8f0cd8b9a21e27db` (unchanged in round 2); the rendering script printed no text beyond the right margin; C2PA chunk and metadata stripped on the device (hashes equal the originals). (After round 1: PNG 3435 px, 655,367 bytes, `e48dffcc40a5a110`; SVG `573fe4d1fd51fb13`.) Earlier note: C2PA chunk and metadata stripped on the device (hashes equal the originals). (First version: PNG 1200 x 3090, `28dec880d7562b9b`; SVG `e125e0e864a7d923`; md `16cfe457f760b40f`.)
- Text in the image is limited to: card headings (USPS Smart Locker, gopost, Cluster box parcel locker), facts also in the article body, a dashed "Where the pages differ" card, and a sources footer. The rendering script printed no text beyond the right margin.
- Alt text (979 characters after round 1; 839 before) matches the front matter `image_alt` and the Markdown alt text; it gives the three cards and the two differences.

## Comparison with the published posts (overlap)

| Post | What it already says | Handling here |
|---|---|---|
| usps-redelivery-how-it-works (155) | scope sentence leaves Smart Lockers to a later post; Smart Locker not available by phone | one sentence, one link, one added fact (phone) from S7 |
| usps-po-box-how-it-works (88) | oversized packages to the counter or a locker | one sentence, one link |
| usps-tracking-status-what-it-means (128) | the key rule for a cluster box | one sentence, one link |
| usps-informed-delivery-how-it-works (30) | Daily Digest content | one sentence on the QR code in the digest, one link |
| usps-package-pickup (not linked) | different service | not linked |

Internal links: four, each once, link text equal to the live title (tracking status uses the short form "USPS Tracking Status" as a name).

## Open points for Gate 2

1. Is the three-locker framing (and the title "Smart Locker vs. Parcel Locker") fair to the pages, given that USPS pages use "parcel locker" for gopost and the cluster box, and the Redelivery FAQ also ties the notice label "Parcel Locker Eligible" to the Smart Locker option?
2. (Round 1 asked for the Priority Mail Express count to be shown by source; applied. Re-check the new wording.)
3. C23 ("stays until pickup") and C37/C38 (statements about our own published posts) should be checked against the posts.
4. Four internal links in an article of this length: acceptable?

## Not checked

WordPress draft, editor, mobile (375 and 320 px) and live page: not yet built. Search volume: not checked (Trends relative only). The USPS.com business page, the locator and gopost registration pages beyond the FAQ were not read.

## Gate 2 FIX round 1 (2026-11-24, base `6ddb13c`): applied

Reviewer result: the three-locker structure and the four internal links are appropriate; the checks on the tracking status post (cluster box key), the PO Box post (oversized packages) and the Daily Digest QR code wording matched. One item to fix: the Smart Locker hold-time summary presented 5 days in the locker, 10 at the counter and return as the rule for all packages, while the FAQ treats Priority Mail Express separately (returned 5 calendar days after the first delivery attempt). The diagram and alt said only "returned after 5 days", which a reader could take as 5 days from the notice or from locker placement. The "pages do not say which day the count starts" sentence was wrong, because the FAQ names the first delivery attempt.

Applied: (1) lead and "Picking up" section: the 5 + 10 + 15 timeline is stated for packages other than Priority Mail Express, with the Priority Mail Express count (FAQ: returned to the sender 5 calendar days after the first delivery attempt; USPS.com: after 5 days in the locker) given right after it; the comparison table row says the same; (2) diagram card 1 and the "Where the pages differ" card, and the alt text (front matter and body, identical): the FAQ's first-delivery-attempt count and USPS.com's in-locker count are labeled by source; (3) the "Where the USPS pages differ" bullet: the pages give different starting points for the count, the article does not say which applies, and a reader near the deadline is told to ask the Post Office that holds the package; the earlier sentence that the pages do not say when the count starts is removed.

Re-checked on 2026-11-24 in the built-in browser: the Smart Locker FAQ note ("Priority Mail Express items are returned to sender 5 calendar days after the initial delivery attempt, no matter when the USPS Smart Locker option is selected" follows the pickup section; "all other items not picked up are removed from the locker" follows it), the USPS.com recipient and shipper pages ("After 5 days in the locker: Priority Mail Express packages will be immediately returned to sender. All other packages ..."), and the redelivery return-dates FAQ table (Priority Mail Express: second notice 3 days after receipt of first notice, return 5 days after first attempt; "Priority Mail Express which is held for 5 days, before being returned"). The article's own paraphrase "returned" was changed to the pages' "returned to sender" wording. No other wording changed. Nothing is published; Gate 2 round 2 is needed.

## Gate 2 FIX round 2 (2026-11-24, base `7dd55bb`): applied

Reviewer result: the body, table and alt separate the two Priority Mail Express counts correctly; one item left. The lower diagram card "Where the pages differ" said the 5 days start at the first delivery attempt or after 5 days in the locker, which mixes the starting point with the return point (USPS.com says the package is returned after 5 days in the locker; it does not give a start for the count). The upper card and the alt already had the intended meaning.

Applied: the lower card now reads "Priority Mail Express: the FAQ says it is returned 5 days after the first delivery attempt; USPS.com says it is returned after 5 days in the locker." Only the diagram changed (PNG and SVG); the article text and the alt are unchanged, and the alt already matches this wording ("the FAQ says it is returned to the sender 5 days after the first delivery attempt, USPS.com says after 5 days in the locker"). The rendered card was viewed (no text cut off). The article bullet in "Where the USPS pages differ" says "different points for the count to start" for the FAQs against USPS.com; the reviewer found the body acceptable, so it is not changed. Nothing is published; Gate 2 round 3 is needed.

## Gate 2 round 3 and publication (2026-11-24)

Round 3 on `3bb374d` was PASS for the changed part (lower diagram card), with the instruction to re-read the official sources right before publishing and to report first only if an important change appeared.

**Sources re-read on 2026-11-24 right before publishing** (built-in browser, normalized phrase checks; no important change):

- S1 Smart Locker FAQ (Jul 28, 2026): 34 phrases; 28 matched at once and the other 6 were my phrasing, checked by reading the page: "one-time" appears as "one-time pickup QR Code or access code" and "one-time use Smart Locker QR Code", the QR code "will expire after 5 calendar days", "Day Old Poultry" (capitals, no hyphen), the label is "not eligible for a refund once it has been scanned at the Smart Locker kiosk", "Can the Seller and Buyer have the same contact info? No". Priority Mail Express note unchanged ("returned to sender 5 calendar days after the initial delivery attempt, no matter when the USPS Smart Locker option is selected").
- S2 Cluster Box FAQ (Aug 4, 2026): 12 of 12; key left in the mailbox with a tag, key stays in the locker, no "days" text.
- S3 gopost FAQ (Oct 22, 2026): 25 phrases, 23 at once; the page says "Show a government-issued picture ID" where the article says "government-issued photo ID" (same meaning, left as is) and "You will not be assigned a specific parcel locker" (the article says "you are not assigned a specific locker").
- S7 Redelivery FAQ (Sep 16, 2026): 6 of 6; S8 PS Form 3849 FAQ (Jun 29, 2026): 7 of 7; S9 return-dates FAQ (Apr 7, 2026): date, Priority Mail Express "5 days after first attempt" and "held for 5 days" present.
- S4 recipients page: all matched except two of my own phrasings (the page says "15 days after initial notification" and "an email address"); S5 shippers page and S6 Local XChange page: all matched.

**Build:** repository md (16,669 bytes, `8f0cd8b9a21e27db`) and PNG (668,658 bytes, `cd8f61ee8cd7901f`) read from raw `main` and matched; the browser conversion of the md matched the Python converter (18,809 characters, hash `f9ef8946...`). Media 164, post 165 as a draft in the category Postal service and stamps (id 6), comments and pings closed, Rank Math description (148 characters) and focus keyword set. Editor: 31 blocks (9 headings, 1 image, 3 lists, 17 paragraphs, 1 table), 0 invalid. Mobile preview: at 375 px the page has no horizontal overflow (table 317 px inside a 315 px figure); at 320 px no page overflow, image 260 px, the 4-column table is 291 px wide inside a 260 px figure and scrolls inside its figure, font 11 px. Published 2026-11-24.

**Live QA (logged out):** page 200; canonical, title and og tags correct; meta description 148 characters; robots index, follow; BlogPosting JSON-LD; one H1 and 9 H2; no comment form or pingback; image src and alt (979 characters) correct, hash `cd8f61ee8cd7901f`, 668,658 bytes; the Priority Mail Express sentences, the notice label sentences and the "ask the Post Office that holds the package" sentence present; no `$` or `%`; 4 internal links all 200; 9 external links all `target=_blank rel=noopener`; the post is in `/post-sitemap.xml`, `/feed/`, the home page and the category page; `x-wp-total` 39.
