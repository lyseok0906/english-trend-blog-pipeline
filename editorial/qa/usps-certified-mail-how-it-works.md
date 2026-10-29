# QA record — usps-certified-mail-how-it-works

Article: `content/drafts/usps-certified-mail-how-it-works.md` (draft, 2026-10-29, about 1,620 words in the body after the Gate 2 FIX round).
Brief: `research/briefs/usps-certified-mail-how-it-works.md`. Sources: `research/sources/usps-certified-mail-how-it-works.md` (S1 USPS FAQ, S2 DMM 503 section 3.0 and 1.8, S3 USPS.com extra-services page, S4 Notice 123, **S5 DMM 508 sections 1.1.7 and 1.1.8, added in the FIX round**).
Stage: draft. Gate 1 (Claude) run on 2026-10-29. **Gate 2 round 1 (ChatGPT, base commit `aa72f32`): FIX. The FIX round was applied on 2026-10-29 (last section). Gate 2 on the revised version has not run. Nothing is in `content/ready/`, nothing is uploaded to WordPress, nothing is published.**

## Scope as approved by the user (2026-10-29)

- Legal effect and Registered Mail comparison are out (lead, "What this article does not cover", diagram footer).
- No fee number in the body; the article points to Notice 123 (linked). The only dollar figure is "$100", the insurance coverage of Priority Mail in the FAQ's example (not a fee).
- The 15-day period is attributed to the FAQ and to DMM 508.1.1.7, with its conditions stated as the pages state them (C31 to C36).
- "(PM only)" in the DMM 503 exhibit is not interpreted and not mentioned in the body (P3).

## Method

Gate 1 (first version): the four pages then used were opened after drafting and tested phrase by phrase by script (FAQ 36 of 36, DMM 503 16 of 16, USPS.com 2 of 2, Notice 123 4 of 4).
FIX round (changed and new statements): after the edits, DMM 508 was opened (sections 1.1.1 to 1.1.8 read in full) and tested by script (9 of 9 phrase checks on 1.1.7 and 1.1.8, text normalized for whitespace, apostrophes and quotation marks); DMM 503 was opened again (8 of 8: Form 3800 label and receipt wording, the round-dating sentence, the detach-and-mark sentence, label placement, the named-individual rule, the record of delivery, the Form 3811 sentence); the FAQ was opened again (10 of 10, including the 15-day sentence, the receipt number, the eligible classes, the fee pointer and the date "May 12, 2026"; the words "starts", "begin", "extend", "extension" and "unclaimed" do not occur on the page). Notice 123 was tested at Gate 1 (effective date and fee row); the changed fee paragraph states no value, so no further test of values is needed. DMM 508 shows no revision date in the page text read.

## Gate 1 — Factual QA (claim by claim, revised version)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | Certified Mail is an Extra Service giving the sender a mailing receipt and, if requested, electronic verification of delivery or of a delivery attempt | S1; S2 3.1.1 | pass |
| C2 | The FAQ says it is bought at the time of mailing, requires a signature from the addressee, and can go with Priority Mail or First-Class Mail | S1 | pass |
| C3 | Dated "as of October 29, 2026"; five USPS pages | Reads | pass |
| C4 | FAQ: a numbered Extra Service that can be bought at the time of mailing at a Post Office | S1 | pass |
| C5 | DMM: dispatched and handled in transit as ordinary mail | S2 3.1.1 | pass |
| C6 | FAQ: the item travels at the speed of the mail class it is bought with | S1 | pass |
| C7 | The FAQ says the sender gets a mailing receipt as confirmation an item was sent (PS Form 3800, "Receipt for Certified Mail"); "in plain terms, Form 3800 has a green label that goes on the item and a receipt for the sender" (the article's plain-language gloss of the FAQ line and DMM 3.2.1: green label part of Form 3800; sender's receipt) | S1; S2 3.2.1 | pass (gloss kept to what both pages state; not "the part the sender keeps", which is not stated) |
| C8 | DMM: label above the delivery address and to the right of the return address (left of the address on parcels) | S2 3.2.1 | pass |
| C9 | DMM: the sender writes the name and complete address of the recipient on the form | S2 3.2.1 | pass |
| C10 | DMM: if a postmarked receipt is requested, the USPS employee round-dates the receipt to show when the item was accepted | S2 3.2.1 | pass |
| C11 | DMM: otherwise the sender detaches the receipt, marks the date and mails the item | S2 3.2.1 | pass |
| C12 | The number on the receipt is the one used to look up the item's status | S1 ("certified mail extra service number shown on the mailing receipt") | pass |
| C13 | USPS: electronic verification that an item was delivered or that a delivery attempt was made | S1; S2 3.1.1 | pass |
| C14 | FAQ: status on USPS.com by the number on the receipt, by telephone with that number, or by bulk electronic file transfer for mailers with an electronic manifest | S1 | pass |
| C15 | DMM gives 1-800-222-1811 | S2 1.8 | pass |
| C16 | Signature wording in three pages: FAQ "requires a signature from the addressee"; DMM 503 record of delivery includes the recipient's signature, delivery record via return receipt bought at mailing; USPS.com signature of the person who accepts the mailing when combined with Return Receipt | S1; S2 3.1.1; S3 | pass |
| C17 | DMM 508: for Certified Mail among others, a mailpiece may not be opened or given to the recipient before the recipient signs and prints his or her name on the form or label, unless an electronic signature is used | S5 1.1.7 | pass |
| C18 | DMM 508: an acceptable form of identification may be required of the recipient before delivery | S5 1.1.7 | pass |
| C19 | DMM 508: when delivery is not restricted at the sender's request, mail addressed to a person at a hotel, apartment house and similar places may be delivered to any person in a position to whom mail for that location is usually delivered | S5 1.1.7 | pass (the article does not generalize beyond the DMM's example and says it does not list every case) |
| C20 | Eligible classes: FAQ lists Priority Mail and First-Class Mail; DMM eligibility table lists the same two | S1; S2 exhibit 1.4.1 | pass |
| C21 | One FAQ sentence in the insurance section also names Priority Mail Express; the eligibility list does not; the article lists only the two classes | S1 | pass (source inconsistency, P2) |
| C22 | Not available with international mail; may go to APO, FPO and DPO and to U.S. possessions and territories | S1 | pass |
| C23 | Return Receipt: bought at mailing; delivery record showing the recipient's signature; FAQ by mail or electronically; DMM hard copy (Form 3811) received by mail | S1; S2 1.8; S3 | pass |
| C24 | Restricted Delivery: only the addressee or the authorized agent (FAQ); DMM 503: the addressee must be an individual specified by name | S1; S2 3.2.2 | pass |
| C25 | DMM 508.1.1.8: postal employees deliver mail marked Restricted Delivery only to the addressee or a person authorized in writing as the addressee's agent; an acceptable form of identification may be required | S5 1.1.8 | pass |
| C26 | DMM 508.1.1.8: mail addressed to two or more persons jointly requires all addressees or their agents to be present to accept delivery together | S5 1.1.8 | pass |
| C27 | DMM 508.1.1.8 lists conditions for particular cases, such as mail for minors; the article does not cover them | S5 1.1.8 | pass |
| C28 | FAQ lists Adult Signature Required and Adult Signature Restricted Delivery (age 21 or older), "not available at retail"; the article goes no further | S1 | pass |
| C29 | DMM: no insurance coverage with Certified Mail, except Priority Mail pieces with included insurance | S2 3.1.1 | pass |
| C30 | FAQ: insurance cannot be bought as an extra service with Certified Mail; Priority Mail with included insurance (up to $100) keeps it | S1 | pass |
| C31 | FAQ: Certified Mail will be held at the Post Office for 15 days and returned to sender on the 16th day | S1 | pass |
| C32 | DMM 508.1.1.7 (covers Certified Mail among other accountable mail): a notice is provided to the addressee for a mailpiece that cannot be delivered; if the piece is not called for or redelivery is not requested, it is returned to the sender after 15 days, unless the sender specifies fewer days on the piece | S5 1.1.7 | pass |
| C33 | The DMM mentions only fewer days for a sender's choice; the pages read do not say how the sender specifies it on the piece | S5 1.1.7 (no "how" in the text); S1 | pass (absence check) |
| C34 | Neither page says which day the count starts from (delivery attempt, notice); the article calculates no date | S1 and S5 1.1.7 text (no start-of-count wording); S2 3.0 has no hold rule | pass (absence check) |
| C35 | The two pages word the period differently ("held for 15 days and returned on the 16th day" in the FAQ, "returned after 15 days" in the DMM); both given, not reconciled further | S1; S5 | pass |
| C36 | DMM 508.1.1.7 gives other periods for Priority Mail Express (5 days) and COD (10 days); not covered | S5 1.1.7 | pass |
| C37 | Refunds: service fee, not postage; four cases | S1 | pass |
| C38 | Request 30 to 60 days after the mailing date, on USPS.com (usps.com/help/refunds.htm) or at a Post Office with PS Form 3533 and evidence of mailing and postage | S1 | pass |
| C39 | Refunds at the local Post Office's discretion; no refund if undeliverable but a delivery was attempted | S1 | pass |
| C40 | Fees: the FAQ sends readers to Notice 123 and to the page on insurance and extra services; Notice 123 lists the fee per item in addition to postage and other fees and shows its effective date | S1; S4 | pass |
| C41 | "A newer version of the list may show different fees, so check the version in effect" (a conditional statement; it does not say fees will change) | Draft statement | pass (replaces the earlier wording that said prices change when the list is reissued) |
| C42 | Sources list: five pages with the dates shown (FAQ May 12, 2026; DMM 503 and DMM 508 no revision date; USPS.com no date; Notice 123 "Effective October 04, 2026") | Reads | pass |

Result: 42 of 42 claims pass as attributed statements or stated limits.

## Open points reported

- **P1 — 15-day period (partly settled).** DMM 508.1.1.7 supplies the conditions (a notice to the addressee; piece not called for or redelivery not requested; return after 15 days; the sender may specify fewer days on the piece) and the FAQ's "held 15 days, returned on the 16th day" fits it. **Still not stated by either page:** which day the count starts from, how the sender specifies fewer days, and whether the FAQ's "16th day" and the DMM's "after 15 days" are the same day. The article says so and calculates no date.
- **P2 — Priority Mail Express.** The FAQ's insurance sentence names it; the FAQ's eligibility list and the DMM table do not. The article lists only the two listed classes and says why.
- **P3 — "(PM only)" in the DMM 503 exhibit.** Meaning not confirmed; not interpreted, not mentioned in the body.
- **P4 — Signature wording.** FAQ, DMM 503 and USPS.com word it differently; DMM 508 adds who may sign. The article gives each wording and does not go beyond them.
- **P5 — Removed.** The "Prove you sent it." quote is deleted from the article (Gate 2 instruction); the mailing receipt is explained plainly (C7, C10 to C12).
- **P6 — Dates.** DMM 503, DMM 508 and USPS.com show no revision date; the article says so.

## Image and alt text (revised)

| # | Check | Result |
|---|---|---|
| I1 | Diagram cards compared with the article and the sources: "How it works" (1 bought at the time of mailing with Priority Mail or First-Class Mail; 2 mailing receipt, PS Form 3800; 3 the recipient signs and prints a name, DMM 508 (C17); 4 if requested, electronic verification of delivery or an attempt, checked on USPS.com or by phone with the receipt number (C12 to C14)); "Add-ons" (Return Receipt hard copy or electronic; Restricted Delivery only the addressee or an agent authorized in writing, DMM 508 (C23, C25)); "Not included" (insurance of its own, Priority Mail's included insurance stays; international mail not available); "If it cannot be delivered" (notice to the addressee; if not called for or redelivery not requested, returned after 15 days, DMM 508; FAQ: held 15 days, returned on the 16th day; the sender may specify fewer days on the piece; the pages do not say when the count starts (C31 to C35)); footer "Legal effect is not covered here.", "No price shown: see USPS Notice 123", source line "USPS FAQ, DMM 503 and 508, Notice 123" | pass |
| I2 | The diagram separates the general signature step (card 1, step 3) from Restricted Delivery (card 2) | pass |
| I3 | **File checked as it will be committed.** The PNG and SVG were read from the repository working tree after the write (not from the build folder): PNG 1200 x 3207, 135,539 bytes, pixel-identical to the rendered image (difference box empty); SVG height 2138, 13,279 bytes, all 37 text elements match the diagram text above. Both files carry an embedded provenance manifest added by the file transfer (a `caBX` chunk of 5,758 bytes in the PNG, a `<metadata>` block in the SVG). The earlier QA line "no embedded metadata" is withdrawn | pass (note) |
| I4 | Alt text 504 characters, the same string in the front matter and in the body image; matches the diagram cards (how it works; add-ons; not included; notice, 15 days or fewer if the sender specifies, start of the count not stated; no price shown) | pass (long; can be cut if Gate 2 asks) |
| I5 | Meta description unchanged, 155 characters | pass |
| I6 | Front matter complete; one H1, nine H2 sections plus Sources; no internal link used | pass |

## Gate 2 FIX round (applied 2026-10-29, base `aa72f32`)

| # | Gate 2 instruction | Change made |
|---|---|---|
| G1 | Check DMM 508.1.1.7 against the FAQ for the non-delivery and not-called-for conditions of the 15-day period and the sender's shorter period | DMM 508 read in full for 1.1.1 to 1.1.8. Section "If the item cannot be delivered: the 15-day period" now gives both pages: FAQ (held 15 days, returned on the 16th day) and DMM 508.1.1.7 (notice for a mailpiece that cannot be delivered; not called for or redelivery not requested; returned after 15 days; unless the sender specifies fewer days). C31 to C36 |
| G2 | Do not estimate the start of the count without clear support | The article says neither page states which day the count starts from, names the two examples without choosing, and calculates no date (C34, P1). Diagram says "The pages do not say when the count starts." |
| G3 | Change body, diagram and alt together; distinguish ordinary signature from the Restricted Delivery receiving scope | Body: "A signature" now has the DMM 508 rule for Certified Mail in general (recipient signs and prints a name unless an electronic signature; identification may be required; the hotel and apartment example for unrestricted delivery); "Add-ons" has the Restricted Delivery scope (addressee or a person authorized in writing; identification; joint addressees). Diagram: new step 3 and the Restricted Delivery line; new fourth card. Alt rewritten. C17 to C19, C24 to C27, I1 to I4 |
| G4 | Fix the sentence saying fees necessarily change when a new price list is issued | Now: "A newer version of the list may show different fees, so check the version in effect." (C41) |
| G5 | Remove "Prove you sent it." and explain the mailing receipt plainly | Quote deleted (also from the source-note use list). New plain explanation: Form 3800 has a green label for the item and a receipt for the sender; the clerk round-dates the receipt to show when the item was accepted; otherwise the sender detaches it and marks the date; the number on the receipt is used to look up status (C7, C10 to C12) |

## Gate 2 — English + SEO QA

Round 1: FIX (above). Round 2 on the revised version: not run. Request from ChatGPT by commit SHA after the user pushes. Points for the reviewer: the 15-day section (P1), the signature paragraph (P4), the Priority Mail Express sentence (P2), whether the alt text is too long, whether one internal link is wanted.

## Not done yet

- Gate 2 round 2 (independent).
- Fresh re-check of all five pages before approval and again right before publishing (Notice 123 in particular).
- User approval to move to `content/ready/`; WordPress draft; publishing.
