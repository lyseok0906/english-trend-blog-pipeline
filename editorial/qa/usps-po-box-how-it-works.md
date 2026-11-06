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
