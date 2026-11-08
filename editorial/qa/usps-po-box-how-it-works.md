# QA record — usps-po-box-how-it-works

Article: `content/drafts/usps-po-box-how-it-works.md` (draft, 2026-11-06; about 1,366 words including the sources list; one H1, eight H2 sections; one table).
Brief: `research/briefs/usps-po-box-how-it-works.md`. Sources: `research/sources/usps-po-box-how-it-works.md` (S1 USPS.com "Rent a PO Box", S2 Domestic Mail Manual 508 section 4.0; neither page shows an update or revision date).
Stage: **draft, Gate 1 (Claude) done 2026-11-06.** Gate 2 (ChatGPT by the user), ready, WordPress and publication are not done.

## Scope

Only what the USPS.com page and DMM 508 section 4.0 state about a standard PO Box: sizes, applying, identification wording, waiting list, service periods, payment, keys, access, packages, Street Addressing and Signature on File as USPS.com describes them, closing. No prices or fee groups, no free (Group E) service, no Caller Service, no business accounts, no list of acceptable ID (DMM 608.10.3 and 608.10.4 were not read and the article says it does not list them), no legal questions.

## Method

After drafting, both sources were opened again in the built-in browser (2026-11-06). The USPS.com page was tested by script with 35 phrases after normalization (apostrophes, dashes, whitespace): all matched once the "A PO Box is a secure, numbered box" sentence was tested case-insensitively (the first run failed only because of the capital "A" in my pattern). The DMM page text was read for sections 4.1 to 4.8 and every statement the article attributes to the DMM was compared with the text. Absence claims were tested: no dollar amounts appear in the USPS.com page text (the only "$" on the DMM page is a $500 insured-mail threshold in another section), and neither source gives an update date.

One fix at Gate 1: the keys sentence said both sources say "two keys, or the combination"; the DMM (4.7.1) says only that two PO Box keys are initially issued to each new box customer, so the sentence now attributes the combination to USPS.com and the two keys to both. The diagram says "2 keys or the combination" in card 3 under USPS.com and needs no change.

## Gate 1 — Factual QA (claim by claim)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | A PO Box is a secure, numbered box at a Post Office where mail is kept until collected | S1 | pass |
| C2 | Apply online or at a Post Office; keys or lock combination picked up at the Post Office where the box is, after the staff verify identification | S1 | pass |
| C3 | The article gives no fees; fee depends on size and location (S1 "prices differ"; S2 4.4.1 bases fees on size and fee group) | S1; S2 | pass |
| C4 | Five box sizes; USPS.com: "most Post Offices", depending on availability; DMM 4.1.3: availability varies by facility | S1; S2 | pass |
| C5 | Table: front dimensions 3 x 5.5, 5 x 5.5, 5.5 x 11 (DMM lists 11 by 5.5), 11 x 11, 12 x 22.5 (DMM lists 22.5 by 12); the article says the order of width and height differs for sizes 3 and 5 | S1; S2 | pass |
| C6 | Table: what USPS.com says each size holds (10-15 letters and 3 rolled magazines; 15+ letters, 5 rolled magazines or 1 Small Priority Mail Flat Rate Box; and so on) | S1 | pass (tested) |
| C7 | Table: DMM capacities under 296; 296 through 499; 500 through 999; 1,000 through 1,999; 2,000 or more cubic inches | S2 4.1.3 | pass |
| C8 | Four online steps (search, choose location/size/period, complete application which generates PS Form 1093 and pay, print and take to the counter with 2 forms of acceptable U.S. ID within 30 days) | S1 | pass |
| C9 | In person: bring payment and 2 forms of acceptable U.S. identification | S1 | pass |
| C10 | DMM: each applicant listed (including both spouses and others listed, except minors) presents two items of valid, current identification, one primary (608.10.3) and one secondary (608.10.4); those sections are not read or listed | S2 4.2.1 | pass |
| C11 | DMM: spouses may complete and sign one Form 1093; minors may be provided with service unless a parent or guardian submits a written objection; minors cannot apply online | S2 4.2.1 | pass |
| C12 | Renting in another city or state is allowed, but the keys or combination are picked up at the Post Office where the box is, with the proper documentation | S1 | pass |
| C13 | If the box is unavailable: choose another size, another location, or a wait list; USPS contacts by email or phone; 2 days to reserve before it goes to the next person | S1 | pass |
| C14 | DMM 4.1.5 and 4.1.6: the postmaster may refer to another facility, use a waiting list, provide general delivery, or offer a different size or Caller Service; online customers cannot apply for an unavailable box but can join the waiting list | S2 | pass |
| C15 | USPS.com lists terms of 3, 6 and 12 months; DMM 4.1.7 says 3-, 6- or two 6-month (semi-annual) prepaid periods and does not mention 12 months | S1; S2 | pass |
| C16 | 3-month option requires automatic recurring renewal (both); USPS.com: no opt-out on 3 months, opt-out possible on 6 or 12 months; DMM: 3-month option not available at locations on the April/October schedule | S1; S2 | pass |
| C17 | Four payment methods on USPS.com (online card, self-service kiosk, mail with check or money order payable to "U.S. Postal Service" to the Postmaster, in person); payment by the 10th; box closed on the 11th if unpaid | S1 | pass |
| C18 | Full rental period paid at the start; USPS.com: partial refund depending on how long the box was kept | S1 | pass |
| C19 | DMM 4.8.3: failing to pay by the due date is one case in which a box is surrendered | S2 | pass |
| C20 | USPS.com: 2 keys or the lock combination; more than 2 keys cost an additional fee; DMM 4.7.1: two keys initially issued to each new box customer | S1; S2 | pass (fixed at Gate 1) |
| C21 | USPS.com: most locations allow 24/7 access; hours vary by Post Office | S1 | pass |
| C22 | DMM 4.1.4: mail for a box must show the PO Box number in the address immediately above the city, state and ZIP Code | S2 | pass |
| C23 | Packages that do not fit: slip for the counter during normal business hours, or a secure parcel locker, including USPS Smart Lockers at select locations | S1 | pass |
| C24 | Signature items: notice in the box, sign at the counter; with free Signature on File the item is left in the box | S1 | pass |
| C25 | Street Addressing where available: Post Office street address plus the box number; packages from UPS, FedEx, DHL, Amazon if they comply with USPS standards | S1 | pass |
| C26 | Close online through Manage PO Box or at the Post Office; then file a Change of Address, mail forwarded up to one year | S1 | pass |
| C27 | DMM 4.8.3: a written notice to discontinue service and a permanent change-of-address order are cases of surrender | S2 | pass |
| C28 | Neither page shows an update or revision date; both read 2026-11-06; no prices | S1; S2 | pass (absence tested) |

## Image check

| # | Item | Result |
|---|---|---|
| I1 | Step 1 "Choose": a Post Office, five sizes, a term; prices differ by location matches C3, C4, C15 | pass |
| I2 | Step 2 "Apply": online or at a Post Office, PS Form 1093 matches C8, C9 | pass |
| I3 | Step 3 "Show ID": 2 forms of ID (the DMM: one primary, one secondary); online applicants within 30 days; then 2 keys or the combination matches C8, C10, C20 | pass |
| I4 | Step 4 "Keep it": pay by the 10th, unpaid box closes on the 11th; terms of 3, 6 or 12 months (USPS.com) and the DMM's 3-, 6- or two 6-month periods matches C15, C17 | pass |
| I5 | Packages note: slip for the counter or a secure parcel locker (USPS.com) matches C23; footer sources and read date match the article | pass |
| I6 | Alt text (706 characters) in front matter and body is identical and says the same as the diagram | pass |
| I7 | Files `assets/raw/usps-po-box-how-it-works.svg` and `assets/optimized/usps-po-box-how-it-works.png` (1200 x 2172, 321,690 bytes, sha256 d69c9d2f...64226) read back from the repository; no logos or photos; text 25 to 46 px on an 800 px canvas | pass |

## Format

Title 58 characters; slug `usps-po-box-how-it-works`; meta description 142 characters; the focus keyword `how does a usps po box work` appears word for word in the title only; one H1; plain markdown table; no prices; one internal link candidate (`usps-mail-forwarding-how-long`, to be decided at Gate 2; no link is in the body yet).

## Open points

- **P1 (wording differences):** terms (USPS.com 3, 6, 12 months vs the DMM's 3-, 6- or two 6-month periods) and identification ("2 forms of acceptable U.S. identification" vs one primary and one secondary under 608.10.3 and 608.10.4, not read). The article shows both and does not decide between them.
- **P2 (no dates):** neither page shows a date; the article says so and gives the read date.
- **P3 (demand):** the phrase "usps po box" is partly navigational and price-driven (people may be looking for the rental page or fees); the article gives no fees. Relative index only (see brief).
- **P4 (length):** about 1,366 words with many facts; every claim is attributed to the page or the DMM.

## Result and next step

Gate 1: **PASS** (28 of 28 claims, 7 of 7 image checks). Next: push, Gate 2 by commit SHA (user to ChatGPT). Under the user's standing rule of 2026-11-06, after a Gate 2 PASS the file moves to `content/ready/`, a WordPress draft is made, both sources are re-read right before publishing (USPS.com page and DMM 508 section 4.0), and the post is published if nothing changed, followed by live QA and records. If a source changed or the two sources now conflict on a point the article states, report first.

---

## Gate 2 round 1 = FIX (ChatGPT, base `bed1e85`) and the fix (2026-11-06)

**FIX points:** (1) the diagram and alt gave "10th" and "11th" without the month basis; (2) the 3/6/12-month wording against the DMM's "two 6-month" prepaid periods must not be called a confirmed conflict; compare DMM 4.1.7, 4.4.3, 4.4.4 and the USPS.com renewal guidance, and state the limit if the relation cannot be confirmed; (3) refund wording must be conditional and link to USPS's detailed guidance.

**Sources re-opened (built-in browser, 2026-11-06):** USPS.com page (payment, renewal, refund and closing sections), the USPS FAQ "PO Box - The Basics" (dated Oct. 16, 2026; the page USPS.com links for refunds; new source S3), DMM 508 4.1.7, 4.4.3, 4.4.4, 4.6, 4.7.5, 4.8.3. Notes in `research/sources/usps-po-box-how-it-works.md`.

**Findings:** USPS.com: pay by the 10th of the month the payment is due, closed on the 11th of that month. The FAQ: terminated if payment is not received by the 10th day after the due date; fees due on the 15th or the last day of the month by billing cycle. DMM: renewal fee payable in the last 30 days of the period, no later than the last day (4.4.4); late payment charge after more than 10 days (4.7.5). The FAQ lists 12 months (annual); the DMM lists 3, 6 or two 6-month periods and says a fee may be paid up to one year in advance (4.4.3). No page says how the dates or the terms relate, so the article states the limit and sends the reader to the Post Office where the box is. Refunds: USPS.com says a partial refund depending on how long you have had the box; the FAQ says eligibility depends on the term (3-month: not eligible once activated); the article now says "may be eligible for a refund" with the condition dependence and links the FAQ refund section.

**Changes:** body section "Service periods, payment and renewal" rewritten (terms, payment methods, deadline wording by source, refund paragraph with link); intro and Sources list now name three sources (FAQ added with its date); diagram rebuilt (card 4 "Keep it up" with the month basis, new cards "Where the pages differ" and "Closing and refunds", footer with three sources, subtitle "Per USPS.com, a USPS FAQ and the DMM"); alt text rewritten (1,069 characters, front matter and body identical).

**Re-check of the changed parts**

| # | Statement now in the article | Source | Result |
|---|---|---|---|
| F1 | USPS.com lists 3, 6, 12 months; FAQ lists 3-month, 6-month (semi-annual), 12-month (annual) | S1; S3 | pass |
| F2 | DMM 4.1.7: 3-, 6- or two 6-month (semi-annual) prepaid periods; 4.4.3: a fee may generally be paid up to one year in advance | S2 | pass |
| F3 | The pages do not say how a 12-month term relates to two 6-month periods (absence: no sentence equating them found in the three pages) | S1; S2; S3 | pass |
| F4 | All three say the 3-month option involves automatic recurring renewal; USPS.com: no opt-out on 3 months, opt-out on 6 or 12; DMM: not at April/October-schedule locations | S1; S2; S3 | pass |
| F5 | USPS.com: payments by the 10th of the month the payment is due; closed on the 11th of that month | S1 | pass |
| F6 | FAQ: terminated if not received by the 10th day after the due date, incoming mail returned to senders; fees due on the 15th or the last day of the month by billing cycle | S3 | pass |
| F7 | DMM 4.4.4 (last 30 days of the period, no later than its last day); 4.7.5 (lock replacement fee as a late payment charge after more than 10 days); 4.8.3 (failing to pay by the due date = surrendered) | S2 | pass |
| F8 | The pages do not say how the dates fit together; the article gives no single deadline and refers to the Post Office where the box is | S1; S2; S3 | pass |
| F9 | USPS.com: may be eligible for a refund; depends on how long the box was held (wording on the page: "you'll get a partial refund depending on how long you've had the box"; the article uses the conditional form per Gate 2) | S1 | pass |
| F10 | FAQ: refund conditions by term, 3-month term not eligible once activated; DMM 4.6 sets refund rules by service period | S3; S2 | pass |
| F11 | Link https://faq.usps.com/s/article/PO-Box-The-Basics#refund is the link USPS.com gives for "See full details on refunds" and opens the FAQ | S1; S3 | pass |
| F12 | Diagram card 4 and alt: "pay by the 10th of the month the payment is due; closes on the 11th of that month" = F5 | S1 | pass |
| F13 | Diagram card "Where the pages differ": FAQ 10 days after the due date; terms 3/6/12 (USPS.com, FAQ) against 3/6/two 6-month (DMM); ask the Post Office = F1, F2, F6, F8 | S1; S2; S3 | pass |
| F14 | Diagram card "Closing and refunds": a refund may be possible, depends on term and time held = F9, F10 | S1; S3 | pass |
| F15 | Alt text (front matter = body) states the same as the diagram cards and the footer sources | image | pass |
| F16 | Repository PNG `assets/optimized/usps-po-box-how-it-works.png` (1200 x 3045, 490,806 bytes, sha256 65ebd6b0...2719) and SVG `assets/raw/usps-po-box-how-it-works.svg` read back; text within the 745 px limit (no overflow reported); rendered and read on screen | image | pass |

**Remaining open points:** P1 now reads: three sources, wording differences shown, not resolved; P2: USPS.com and the DMM carry no date, the FAQ is dated Oct. 16, 2026; the FAQ's late-fee amount and refund percentages are deliberately not used. Alt text is long (1,069 characters) because it mirrors seven cards; Gate 2 may ask to shorten it.

**Result:** FIX applied; Gate 1 for the changed parts: PASS (16 of 16). Next: push; Gate 2 re-review of the changed parts by the new commit SHA.

---

## Gate 2 round 2 = FIX (ChatGPT, base `78ead03`) and the fix (2026-11-06)

**FIX point:** the diagram's "Pay-by date" label made the FAQ's service-termination condition look like a payment deadline. Change only the diagram and alt (and check the body); no other item to be re-reviewed.

**Source re-opened:** USPS FAQ "PO Box - The Basics" (dated Oct. 16, 2026), tested by script: "If we have not received your payment by the 10th day after the due date, your PO Box service will be terminated and all incoming mail will be returned to senders." (present); "After 10 days of nonpayment, your mail is treated as undeliverable mail and your PO Box is closed." (present); "Box fees are due either on the 15th or the last day of the month" (present). The FAQ gives this as what happens when payment has not been received by the 10th day after the due date, not as a pay-by date.

**Changes (changed parts only):**

| # | Where | Before | After |
|---|---|---|---|
| G1 | Diagram card "Where the pages differ" | "Pay-by date: a USPS FAQ says 10 days after the due date." | "Late payment: a USPS FAQ says service ends if payment is not received by the 10th day after the due date." |
| G2 | Alt text (front matter and body, identical, 1,123 characters) | "a USPS FAQ says 10 days after the due date" | "a USPS FAQ says service ends if payment has not been received by the 10th day after the due date" |
| G3 | Body, lead-in to the payment-date paragraph | "The pages give the payment deadline in different words." | "The pages describe the payment date and late payment in different words." (the FAQ sentence below it already read "if payment has not been received by the 10th day after the due date, the service is terminated and incoming mail is returned to senders") |

**Check against the body and sources:** diagram G1, alt G2 and the body sentence now say the same thing as the FAQ; USPS.com's "by the 10th of the month the payment is due ... closed on the 11th of that month" (card 4, alt, body) is unchanged and labeled as USPS.com; the card still states that the pages are not reconciled and sends the reader to the Post Office where the box is.

**Image:** `assets/optimized/usps-po-box-how-it-works.png` (1200 x 3114, 508,390 bytes, sha256 066722385c3a15ada3ca936f32ff932568e4330833afa688617b98e395db4f39) and `assets/raw/usps-po-box-how-it-works.svg` read back from the repository; text within the 745 px limit; rendered and read on screen; the card now has six lines and the page height grew by 46 px.

**Result:** FIX applied; changed-part check: PASS (3 of 3). Other items not repeated, as instructed. Next: push; Gate 2 re-review of the changed parts by the new SHA; then under the standing rule: ready, WordPress draft, re-read of the three sources right before publishing, publish if unchanged, live QA, records.

---

## Gate 2 re-review, ready, WordPress, pre-publication check, publication and live QA (2026-11-08 UTC / 2026-11-09 KST)

**Gate 2 round 3 (ChatGPT, base `e30cc5d`, user-reported): PASS** for the changed diagram, alt and body; no further change requested. Earlier items not repeated.

**Move to ready and WordPress draft (standing rule):** file moved to `content/ready/` with `status: ready`; image fetched from the repository (GitHub raw, main) and verified by hash before upload (sha256 066722385c3a...4f39, 508,390 bytes); media 87 (WordPress also made a `-scaled` copy; the post uses the original file URL, whose served hash was verified identical); alt text 1,123 characters, identical to the front matter; WordPress draft post 88 (category Postal service and stamps, comments and pings closed); Rank Math focus keyword `how does a usps po box work` and description (142 characters) read back in the editor; 28 blocks, none invalid; typed content verified by SHA-256 (b37f9db2...cef1) before posting; table block with the responsive font size used on the other posts.

**Phone preview (draft, logged in):** 375 px and 320 px: no horizontal overflow; the four-column size table fits (cells wrap, no word wider than its cell); image visible.

**Pre-publication source check (2026-11-09 KST, minutes before publishing): no change, no conflict.**

| Source | Result |
|---|---|
| S1 USPS.com "Rent a PO Box" | 31 relied-on statements tested; 30 matched exactly and 1 differed only by the registered mark ("USPS® Smart Lockers"); the "See full details on refunds" link still points to the FAQ refund section; still no update date; no dollar amounts |
| S3 USPS FAQ "PO Box - The Basics" | 8 of 8 statements matched (date "Oct 16, 2026"; 3, 6, 12-month increments; 3-month automatic renewal; service terminated if payment is not received by the 10th day after the due date; fees due on the 15th or the last day of the month; 3-month term not eligible for a refund once activated; "may be eligible for a refund"; refund section heading) |
| S2 DMM 508 | 19 of 19 statements matched (4.1.3 sizes and chart; 4.1.4; 4.1.5; 4.1.6; 4.1.7; 4.4.3; 4.4.4; 4.7.5; 4.2.1 identification, spouses, minors; 4.7.1; 4.8.3; 4.6.1); page text length identical to the 2026-11-06 read (126,080 characters) |

**Published:** 2026-11-08 23:43:11 UTC (site time 2026-11-08 18:43:11; 2026-11-09 08:43 KST) by Claude under the standing rule. Post 88, media 87. URL https://statesideexplained.com/usps-po-box-how-it-works/ . As-of dates in the text stay November 6, 2026 (content of all three sources unchanged). No indexing request.

**Live QA (logged out, no-store fetch): PASS.** 200; canonical is the post URL; title "How Does a USPS PO Box Work? Sizes, ID and Service Periods - Stateside Explained"; meta description 142 characters, og:description identical; robots index, follow; JSON-LD WebSite, WebPage, Person, ImageObject and BlogPosting; one H1, nine H2, one table; no comment form, no pingback; image from `/wp-content/uploads/2026/11/usps-po-box-how-it-works.png`, hash 066722385c3a...4f39 identical to the repository, alt 1,123 characters; four external links (the FAQ refund anchor, USPS.com, the FAQ, DMM 508); the live text contains the checked statements (the pages do not say how the dates fit together; FAQ termination wording; "may be eligible for a refund"; no claim that the terms conflict; refund-details link); in `/post-sitemap.xml` (19 URLs), `/feed/`, the home page and the Postal service and stamps category page. Counts: 19 live (12 pilot, 7 post-pilot).

**Open:** the alt text is long (1,123 characters); the page and the DMM carry no date; no internal link was added (the mail forwarding post remains a possible later link). Re-read all three sources if the article is revisited.
