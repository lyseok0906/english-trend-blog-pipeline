# QA record — usps-missing-mail-search-how-it-works

Article: `content/drafts/usps-missing-mail-search-how-it-works.md` (draft, 2026-11-13; about 1,330 body words without the alt text; one H1, nine H2 sections; one table of 3 columns).
Brief: `research/briefs/usps-missing-mail-search-how-it-works.md`. Sources: `research/sources/usps-missing-mail-search-how-it-works.md` (S1 USPS FAQ 000007968, May 19, 2026; S2 USPS.com "Find Missing Mail", no update date).
Stage: **published 2026-11-13** (Gate 1 by Claude; Gate 2 FIX on `a2f1755` applied in `fbdf9b3`, re-check PASS on `fbdf9b3`; see the sections below). **Rule-type post: re-read both search sources and the File a Claim page before any later republish.**

## Scope

How USPS says a Missing Mail search works: check tracking, the per-service wait table, the 7 to 365 day window, what to have ready, where to file, unsearchable items, statuses and results, multiple items, edit and cancel, and the pointer to refunds and claims. No prices, claim process detail, Mail Recovery Center, international mail, delivered-but-not-received packages or other carriers.

## Method

After drafting, both pages were opened again in the built-in browser (2026-11-13) and tested by script after normalization: S1 62 of 62 phrases (the only miss, "Domestic Claims - The Basics", sits in the Related Articles list outside the article body slice and was read there earlier the same day); S2 20 of 20. Absence tests: S1 body has no "fee", "free", "charge", "$" or "%", the only "cost" is "includes tracking in the cost of mailing", no retention period length, no sentence linking the 7-day minimum to the 14-day rows; S2 has no "365", no fee or cost, no "14 days" or "fourteen", no "retention", no update date. Internal links checked: Informed Delivery, Package Intercept and Certified Mail posts return 200 (titles match the link text); the new slug returns 404 (unpublished, no clash). 27 articles are live.

## Gate 1 — Factual QA (claim by claim)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | Filing opens 7 days after the mailing date and closes 365 days after it; USPS strongly suggests filing as soon as possible within the window | S1 | pass |
| C2 | USPS.com gives only the start ("starting 7 days from mailing") | S2 (no "365") | pass (absence tested) |
| C3 | A search "does not guarantee a successful outcome"; "sometimes we cannot find missing mail items" | S1; S2 | pass |
| C4 | Both pages put tracking first | S1; S2 | pass |
| C5 | Informed Delivery line on USPS.com: an item may be delayed; see the Informed Delivery FAQs | S2 | pass |
| C6 | Missing Mail defined as not delivered by the expected delivery date, including undelivered, lost or late; lost, late or missing 7 days or more: four options (search request, Mail Recovery Center article, claim for insured items meeting the appropriate timeframe, local Post Office) | S1 | pass |
| C7 | Table: Priority Mail Express 7 or more days and recipient confirmed; Domestic Registered Mail 14 or more days, search and/or claim; Parcel Select 8 days to arrive, 14 or more days and recipient confirmed, search and/or email; the last row (Priority Mail, First-Class with trackable service, Ground Advantage, Tracking/Signature Confirmation/Certified Mail) lists no wait and says to check USPS Tracking | S1 | pass |
| C8 | The FAQ does not say whether Registered Mail or Parcel Select requests are accepted before day 14 | S1 (absence tested) | pass |
| C9 | What to have ready (FAQ list, the 12 x 10 brown box example; USPS.com list, mailing receipt or Click-N-Ship receipt) | S1; S2 | pass |
| C10 | MissingMail.USPS.com; sign in or register; drafts expire after 7 days; Customer Care cannot submit it for you; USPS.com: confirmation email and periodic updates | S1; S2 | pass |
| C11 | Unsearchable list (hazardous material, live ammunition, opened hair or beauty products, over-the-counter and prescription drugs, perishables and food) and the handgun note; "not safe to forward"; the recovery restrictions page was not read | S1; S2 | pass |
| C12 | Six statuses and their meanings; updates by email to the address under "Whom can we contact about this search?"; final email; found items rewrapped and sent to the address on the form; not found: runs until it expires | S1 | pass |
| C13 | Several items in one mailpiece in one request; separate mailpieces separate requests; only the contents can be edited, otherwise cancel and resubmit; cancel from Search History; no further matches after cancel | S1 | pass |
| C14 | USPS.com: refund for money-back guarantee services such as Priority Mail Express; insured mail may be claimed; the "immediately" and 60-day sentence is limited to "damaged or missing contents" (scope corrected after Gate 2); the FAQ says "meeting the appropriate timeframe" with no number | S2; S1 | pass (after FIX) |
| C15 | Absence statements: no retention length, no update frequency, no find rate, no fee, no sentence on who may file; the FAQ intro says "whether you are sending it or receiving it" | S1; S2 (absence tested) | pass |
| C16 | Domestic Claims article listed as related and not read | S1 | pass |

## Image checks

800 px wide SVG, 1200 px wide PNG (scale 1.5), render check printed `[]` (no text beyond 745 px), viewed in crops. Alt text equals the front-matter alt and describes every card. C2PA metadata stripped on the device and the SHA-256 and sizes equal the originals (PNG 488,193 bytes; SVG 3,954 bytes). Diagram wording avoids guarantees: waits are "listed by the FAQ", and the last card repeats USPS's own non-guarantee line.

## Format

One H1 in the body, H2 sections only, a single 3-column table (mobile-safe, post-only table font at publishing), prose with a bulleted list only for Sources, meta description 152 characters.

## Open points for Gate 2

- Confirm the handling of the Registered Mail and Parcel Select 14-day rows against the 7-day application rule (shown, not resolved).
- Confirm the claim timing paragraph reads as a source difference and not as claim advice.
- Dated rule post: both sources are re-read right before publishing; report before publishing if the window, the table, the unsearchable list, the statuses or the claim wording changed.

## Gate 2 FIX on `a2f1755` (applied 2026-11-13)

1. **Scope of the 60-day claim sentence.** The reviewer read the draft as applying 60 days to all insured mail. Cause: the draft quoted the sentence without its lead-in. USPS.com's sentence begins "For damaged or missing contents" (S2 page text, tested again). Fix: the Claims and refunds section now says the sentence is limited to damaged or missing contents of insured mail, says it is not treated as a deadline for every lost or late item, and points to USPS "File a Claim" (S3, https://www.usps.com/help/claims.htm). S3 was fetched and tested 6 of 6 phrases (no update date): it separates "Damaged or Missing Contents" (no later than 60 days after the mailing date) from "Lost Mail or Package" (the time period for the service used); no table value is used. The Sources list, the scope paragraph, the brief, the backlog row and the candidates note were changed to match.
2. **Application link.** The two body mentions of MissingMail.USPS.com are now links to https://missingmail.usps.com/, the target of "Start Your Missing Mail Search" on S2 (the link target was read from the page; a no-cors request returns an opaque response, so only the page's own href is relied on).
3. **FAQ check.** The reviewer could not open the FAQ. It opened for Claude on 2026-11-13 and was tested 62 of 62 (the only miss is the related-articles title outside the article body), including the 7 and 365 day window, the per-service table and the unsearchable list; the verbatim lines are in the source notes (S1). Re-read the FAQ right before publishing.
Changed parts only: the scope paragraph, the two links, the Claims and refunds section and the Sources list. The diagram and its alt do not mention claims and are unchanged.

## Publication record (2026-11-13)

Moved to `content/ready/` after the Gate 2 PASS on `fbdf9b3`. WordPress: media 120 (alt equals the front-matter alt, checked), post 123 created as a draft (category 6, Postal service and stamps; comments and pingbacks closed; Rank Math description and focus keyword `usps missing mail` set). The body was generated by script from the draft on `main` (12,492 characters, 29 block comments) and matched the local Python conversion by SHA-256 (`b6e4066e...`); the image was fetched from `main` and matched the repository hash before upload. Editor check: 27 blocks, none invalid; Rank Math keyword and description read back. Phone preview of the table at 375 px (table 315 px wide, no page overflow, font 12 px) and 320 px (260 px, no overflow, 11 px); the 3-column table wraps and stays inside the content width. **Re-read right before publishing:** FAQ 62 of 62 phrases (text length 10,312 characters, same as at Gate 1, article date May 19, 2026), USPS.com "Find Missing Mail" 20 of 20, "File a Claim" 6 of 6, absence tests unchanged (no fee, no "365" on USPS.com, no update date); the page links still go to https://missingmail.usps.com/ and https://www.usps.com/help/claims.htm; no change and no conflict. Published 2026-11-13 03:13 UTC.
Live QA (logged out): 200; canonical equals the URL; title and meta description equal the draft; Open Graph title, description and image present; robots index, follow; one JSON-LD block with a BlogPosting; one H1; no comment form or pingback link; image SHA-256 equals the repository (`6ea0513d...`) and the live alt is the front-matter alt; key sentences present (lead, "does not guarantee a successful outcome", the 60-day sentence and its damaged-or-missing-contents scoping, the File a Claim pointer); internal links to Informed Delivery, Certified Mail and Package Intercept return 200; the two USPS links are present; the post is in `/post-sitemap.xml`, `/feed/`, the home page and the category page `/category/postal-service-and-stamps/`; 29 posts total (`x-wp-total`). No indexing request. Search volume was never checked; Trends relative indexes only.
