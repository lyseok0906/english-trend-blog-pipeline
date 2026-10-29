# QA record — usps-certified-mail-how-it-works

Article: `content/drafts/usps-certified-mail-how-it-works.md` (draft, 2026-10-29, about 1,265 words in the body).
Brief: `research/briefs/usps-certified-mail-how-it-works.md`. Sources: `research/sources/usps-certified-mail-how-it-works.md` (S1 USPS FAQ, S2 DMM 503 section 3.0, S3 USPS.com extra-services page, S4 Notice 123).
Stage: draft. Gate 1 (Claude) run on 2026-10-29. **Gate 2 (ChatGPT, by commit SHA) has not run. Nothing is in `content/ready/`, nothing is uploaded to WordPress, nothing is published.**

## Scope as approved by the user (2026-10-29)

- Legal effect and Registered Mail comparison are out. The article says so in the lead, in one sentence after the quoted USPS.com line, and in "What this article does not cover".
- No fee number in the body; the article points to Notice 123 (linked) and says prices change when the list is reissued. Check: the body contains no Certified Mail, Return Receipt or other fee amount. The only dollar figure is "$100", the insurance coverage of Priority Mail in the FAQ's example (not a fee).
- The 15-day hold is attributed to the USPS FAQ, with its conditions stated as what the FAQ says and does not say (see C26 to C28).
- The unresolved "(PM only)" footnote in the DMM exhibit is **not interpreted and not mentioned in the body**. Adult Signature services appear in one sentence that follows the FAQ and says the article does not go further.

## Method

After drafting, all four pages were opened again in the built-in browser on 2026-10-29 and every statement the draft relies on was tested against the page text by script (whitespace, apostrophes and ®/™ normalized): S1 FAQ 36 of 36 phrase checks pass (page date "May 12, 2026"); S2 DMM 503 section 3.0 and 1.8 16 of 16 pass, including the eligibility table row read from the page's table; S3 USPS.com 2 of 2 pass; S4 Notice 123 4 of 4 pass (effective date, "per item, in addition to postage and other fees", Certified Mail row present, title "Price List"; the price value was not copied into the article). Absence checks: the FAQ text has no mention of what starts the 15 days, of a notice, an extension or an unclaimed status in connection with the hold (the word "notice" on the page is "Notice 123"); the whole DMM 503 page has no "16th day" and no Certified Mail hold rule; S3 shows no page date; S2 shows no revision date.

## Gate 1 — Factual QA (claim by claim)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | Certified Mail is an Extra Service that gives the sender a mailing receipt and, if requested, electronic verification that an item was delivered or that a delivery attempt was made | S1 (mailing receipt; "If requested, provides electronic verification..."); S2 3.1.1 | pass |
| C2 | The FAQ says it is bought at the time of mailing, requires a signature from the addressee, and can go with Priority Mail or First-Class Mail | S1 | pass |
| C3 | Dated "as of October 29, 2026"; four USPS pages | Reads | pass |
| C4 | The FAQ calls it a numbered Extra Service that can be bought at the time of mailing at a Post Office | S1 | pass |
| C5 | DMM: dispatched and handled in transit as ordinary mail | S2 3.1.1 | pass |
| C6 | FAQ: the item travels at the speed of the mail class it is bought with | S1 | pass |
| C7 | USPS.com puts the service in one line that begins "Prove you sent it." (four-word quote, attributed; no legal reading) | S3 | pass |
| C8 | USPS says the sender gets a mailing receipt as confirmation an item was sent (PS Form 3800, "Receipt for Certified Mail") | S1 | pass |
| C9 | DMM: green Form 3800 label, above the delivery address and to the right of the return address (to the left of the address on parcels) | S2 3.2.1 | pass (the DMM also names the non-barcoded Label 3800-N in one case; the article says "the green Form 3800 label", a simplification that does not contradict it) |
| C10 | DMM: the sender writes the name and complete address of the recipient on the form | S2 3.2.1 | pass |
| C11 | DMM: if a postmarked receipt is requested, the USPS employee round-dates the receipt; otherwise the sender detaches the receipt, marks the date and mails the item | S2 3.2.1 | pass |
| C12 | USPS: electronic verification of delivery or a delivery attempt (provided "if requested") | S1; S2 3.1.1 | pass |
| C13 | FAQ: status by USPS.com with the number shown on the mailing receipt, by telephone with that number, or by bulk electronic file transfer for mailers who send an electronic manifest | S1 | pass |
| C14 | DMM gives 1-800-222-1811 as the telephone number | S2 1.8 | pass |
| C15 | Signature, three wordings: FAQ "requires a signature from the addressee"; DMM: USPS keeps a record of delivery that includes the recipient's signature and a delivery record can be obtained by buying a return receipt at mailing; USPS.com: the signature of the person who accepts the mailing comes when combined with Return Receipt | S1; S2 3.1.1; S3 | pass |
| C16 | Eligible classes: FAQ lists Priority Mail and First-Class Mail; the DMM eligibility table lists the same two | S1; S2 exhibit 1.4.1 (row read from the table) | pass |
| C17 | One FAQ sentence in the insurance section also names Priority Mail Express; the FAQ's own eligibility list does not include it; the article lists only the two classes in the list | S1 | pass (a source inconsistency, reported as P2) |
| C18 | Not available with international mail; may go to APO, FPO and DPO addresses and to U.S. possessions and territories | S1 | pass |
| C19 | Return Receipt is bought at the time of mailing and gives a delivery record showing the recipient's signature; FAQ: by mail or electronically; DMM: hard copy (Form 3811) received by mail | S1; S2 1.8; S3 | pass |
| C20 | Restricted Delivery: direct delivery only to the addressee or the authorized agent; DMM: the addressee must be an individual specified by name | S1; S2 3.2.2 | pass |
| C21 | FAQ lists Adult Signature Required and Adult Signature Restricted Delivery, for an adult age 21 or older, and says they are not available at retail | S1 | pass |
| C22 | The article does not go further into those two services | (scope statement) | pass |
| C23 | DMM: no insurance coverage is provided when purchasing Certified Mail, except for Priority Mail pieces with included insurance | S2 3.1.1 | pass |
| C24 | FAQ: insurance cannot be bought as an extra service when Certified Mail is selected; example: Priority Mail with included insurance (up to $100) keeps that coverage | S1 | pass |
| C25 | FAQ: "held at the Post Office for 15 days and returned to sender on the 16th day" (stated in the article as: Certified Mail will be held at the Post Office for 15 days and returned on the 16th day) | S1 | pass |
| C26 | The FAQ does not say what starts the 15 days, whether a notice is left first, or whether the sender or addressee can change the period | S1 absence checks | pass |
| C27 | The DMM Certified Mail section read does not repeat the 15-day rule | S2 (section 3 and the whole page: no "15 days" in 3.0, no "16th day" anywhere) | pass |
| C28 | The DMM's section on delivery (508) was not read | Method (it was not opened) | pass (a stated limit) |
| C29 | Refunds: service fee, not postage; four cases (receipt and verification not received after 30 days but delivery known; non-delivery when USPS is at fault; incorrect charges; paid services not provided) | S1 | pass |
| C30 | Request 30 to 60 days after the mailing date, on USPS.com (usps.com/help/refunds.htm) or at a Post Office with PS Form 3533 and evidence of mailing and postage | S1 | pass |
| C31 | Refunds at the discretion of the local Post Office; no refund for the Certified Mail service if the item is undeliverable but a delivery was attempted | S1 | pass |
| C32 | Fees: the FAQ sends readers to Notice 123 and to the page on insurance and extra services; Notice 123 lists the fee per item in addition to postage and other fees, and shows its effective date at the top | S1; S4 | pass |
| C33 | The article states no price; prices change when the list is reissued (the draft's statement, not USPS's) | Draft statement; S4 effective date shows the list is dated | pass (not attributed to USPS in the text) |
| C34 | Sources list: FAQ "page shows May 12, 2026"; DMM no revision date shown; USPS.com no date shown; Notice 123 "Effective October 04, 2026" | Reads | pass |

Result: 34 of 34 claims pass as attributed statements or as stated limits.

## Open points reported

- **P1 — 15-day hold conditions.** The FAQ states the rule without a trigger. The article repeats it as stated, lists what the FAQ does not say, and attributes it to the FAQ alone. A reader cannot learn from the pages read when the 15 days start or what happens to a notice. (The DMM delivery section 508 was not read; reading it could settle this, but the user asked for the FAQ as the basis.)
- **P2 — Priority Mail Express.** The FAQ's insurance sentence names it as a class Certified Mail can be added to, but the FAQ's eligibility list and the DMM table do not list it. The article names only the two listed classes and says why.
- **P3 — "(PM only)" in the DMM exhibit.** A footnote next to the Adult Signature rows; its meaning could not be confirmed from the page text. Not interpreted and not mentioned in the body.
- **P4 — Signature wording.** The FAQ, DMM and USPS.com word the signature point differently; the article gives each wording and does not reconcile them.
- **P5 — "Prove you sent it."** USPS.com's wording, quoted once with the statement that the article does not discuss its legal meaning. Gate 2 may ask to cut the quote if it reads as legal framing.
- **P6 — Dates.** The DMM and USPS.com pages show no revision date; the article says so.

## Image and alt text

| # | Check | Result |
|---|---|---|
| I1 | Diagram cards compared with the article: "How it works" (bought at the time of mailing with Priority Mail or First-Class Mail; mailing receipt, PS Form 3800; if requested, electronic verification of delivery or a delivery attempt; status online or by phone with the number on the receipt), "Add-ons" (Return Receipt, hard copy or electronic; Restricted Delivery, only the addressee or the authorized agent), "Not included" (insurance of its own, Priority Mail's included insurance stays; international mail not available), "The 15-day hold" (per the USPS FAQ, held 15 days, returned to sender on the 16th day); footer "Legal effect is not covered here." "No price shown: see USPS Notice 123" and the source line. Each matches C1 to C25 | pass |
| I2 | No fee, no logo, no photo, no USPS eagle, no picture of the green label; only the words "USPS", "Priority Mail", "First-Class Mail", "PS Form 3800" used as USPS names | pass |
| I3 | Image viewed after export (1200 x 2697, PNG8, 64 colors, 100,337 bytes): no clipped text, no widow line in the footer; source SVG (`assets/raw/usps-certified-mail-how-it-works.svg`) has a title element and no embedded metadata | pass |
| I4 | Alt text 454 characters, same string in front matter and in the body image; matches the diagram and says "No price shown" | pass |
| I5 | Meta description 155 characters (<160): "USPS Certified Mail adds a mailing receipt and delivery information to Priority Mail or First-Class Mail. See what it includes, the add-ons and the limits." | pass |
| I6 | Front matter complete (title, slug, meta description, category, focus keyword, status, date, internal-link note, image, image alt); one H1, nine H2 sections plus Sources; no internal link used (none fits; a Gate 2 option) | pass |

## Gate 2 — English + SEO QA

Not run. To request from ChatGPT by commit SHA after the user pushes. Points for the reviewer: the 15-day hold section (P1), the sentence on Priority Mail Express (P2), whether the "Prove you sent it." quote should stay (P5), whether the signature paragraph is clear (P4), and whether one internal link is wanted.

## Not done yet

- Gate 2 (independent).
- Fresh re-check of all four pages before approval and again right before publishing (the price list in particular).
- User approval to move to `content/ready/`; WordPress draft; publishing.
