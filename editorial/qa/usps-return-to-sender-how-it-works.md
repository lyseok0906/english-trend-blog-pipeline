# QA record — usps-return-to-sender-how-it-works

Article: `content/drafts/usps-return-to-sender-how-it-works.md` (draft, 2026-11-20; about 2,470 words in the body without the alt text, one H1, seven H2 sections including Sources; one table; four internal links).
Brief: `research/briefs/usps-return-to-sender-how-it-works.md`. Sources: `research/sources/usps-return-to-sender-how-it-works.md` (S1 FAQ 000006175, S2 FAQ 000006162, S3 DMM 508, S4 DMM 507, S5 DMM 604).
Stage: **draft, Gate 1 done by Claude 2026-11-20; waiting for Gate 2.** Rule-type post: re-read S1 to S5 right before any publishing.

## Method

The five pages were opened in the built-in browser on 2026-11-20 and every statement the article makes was tested by script after normalization (remove marks and quotes, unify dashes, lowercase; on usps.com FAQ pages also strip a single digit glued after a letter). S1 48 of 48, S2 20 of 21 at once, S3 15 of 15, S4 21 of 22 at once, S5 4 of 4: 108 of 110 phrases matched at once. The two others were my phrasing, not the pages: S2 has the 2-year clause inside a parenthesis ("(for a period not to exceed 2 years) any foreign letter…"), and the article's quote "foreign letter or publication material" was matched separately; S4 has no comma before "and perishable mail" in the Post Office box list, and the article follows the page. Statements about our own posts were checked in the repository files.

## Gate 1 — Factual QA (claim by claim)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | USPS pages describe three situations (mail for someone else, mail you refuse, a sender's mail that could not be delivered) with different rules | S1, S2, S3, S4 | pass (framing; each row below tested) |
| C2 | Source numbers and dates: FAQ 000006175 May 19, 2026; FAQ 000006162 Sep 3, 2026; DMM 508, 507, 604 with no update date; DMM pages read Nov 20, 2026 | S1 to S5 | pass |
| C3 | Table row 1: "Not at this address" to carrier or collection box; wrong location: put back unmarked | S1 | pass |
| C4 | Table row 2: refuse when offered, or mark "Refused" and return unopened within a reasonable time | S2, S3 | pass |
| C5 | Table row 3: returned to the return address; none: local Post Office or Mail Recovery Center (and dead mail, DMM 507.1.9) | S1, S4 | pass |
| C6 | USPS "will deliver the mail as addressed"; delivered to residential or business addresses even if the name differs from the known residents | S2 | pass |
| C7 | Previous resident, address unknown: collection box or other receptacle, "Not at this address" on the envelope | S1 | pass |
| C8 | Wrong location: do not erase, mark over or endorse; mailbox or carrier | S1 | pass |
| C9 | Right location, wrong person: write "Not at this address", do not erase the address, carrier or collection box | S1 | pass |
| C10 | The FAQ does not explain how to tell wrong location from right location with the wrong person | S1 (absence; confirmed by reading the full section) | pass (absence) |
| C11 | Priority Mail Express only: number of the Reporting Unit by calling 1-800-ASK-USPS (1-800-275-8777) | S1 | pass |
| C12 | Misdelivered "We ReDeliver for You" PS 3849 for another address: "Other", write "Refused", mailbox or carrier | S1 | pass |
| C13 | Destroying mail may be prohibited by US laws; willful destruction may be punishable by the federal government; questions to local law enforcement | S1 | pass |
| C14 | Mail to a company delivered to the company, including "Personal and Confidential"; applies to former employees; responsibility ends; company policy | S1 | pass |
| C15 | DMM 508.1.1.2 refuse when offered; 508.1.1.3 mark "Refused", reasonable time, unopened | S3 | pass |
| C16 | Opened (even resealed) cannot be marked "Refused"; new envelope, correct address and new postage (DMM and FAQ) | S2, S3 | pass |
| C17 | Not returnable postage-free after delivery: Registered Mail, insured, Certified Mail, COD, Adult Signature; response mail to a promotion not refused when offered | S3 | pass |
| C18 | FAQ list names Registered, Insured, Certified, COD and the response mail; the customer pays postage to return them | S2 | pass |
| C19 | Accountable mail can be refused before signing: "Refused" on the back of the notice, sign by the "X", put it back in the mailbox | S2 | pass |
| C20 | DMM 508.1.1.7: addressee or representative may obtain the sender's name and address while held, before accepting delivery and endorsing the receipt | S3 | pass |
| C21 | Adding an extra service to a piece being returned: pay return postage and the extra service | S2 | pass |
| C22 | Shortpaid piece refused: "Returned for Additional Postage" to the return address (FAQ) | S1 | pass |
| C23 | DMM 604.8.1.2: refused or undeliverable with insufficient postage: "Returned for Additional Postage" if First-Class Mail with a return address; dead mail with no return address | S5 | pass |
| C24 | Written request to the postmaster to withhold foreign letter or printed matter for no more than 2 years (DMM 508.1.1.4); FAQ wording "foreign letter or publication material" | S2, S3 | pass |
| C25 | DMAchoice (ANA, independent of USPS) and the credit-reporting companies' prescreen opt-out are not USPS actions; no fee given | S2 | pass |
| C26 | FAQ: USPS uses the return address to try to return undeliverable mail | S1 | pass |
| C27 | DMM 507.1.8.3: Priority Mail Express, Priority Mail, First-Class Mail, Ground Advantage Retail and Commercial returned "at no additional charge" unless the sender asks otherwise; 507.1.8.4 other classes | S4 | pass |
| C28 | A returned piece may not be remailed without a new envelope, correct address and new postage (DMM 508.1.1.6); a shortpaid piece can have postage added to the original; FAQ: "postage due" message left intact | S3, S1 | pass |
| C29 | No postage or postage fell off: "Returned for Postage Mail"; greeting cards without a return address generally delivered postage due in December, domestic First-Class Mail only | S1 | pass |
| C30 | Apartment number: delivered if any one of four elements is present (listed) | S1 | pass |
| C31 | Marketing Mail not automatically forwarded or returned; handled by the sender's endorsements; no endorsement: disposed of by USPS | S1 | pass |
| C32 | Post Office box: deliverable mail not returned until the box is declared vacant, except certified, COD, insured, registered, postage due, Adult Signature and perishable mail | S4 | pass |
| C33 | Mail forwarding article reports USPS returning mail for 6 months with a new-address label after forwarding ends | repository (`usps-mail-forwarding-how-long`, "When forwarding ends") | pass |
| C34 | DMM 507.1.8.5: return receipt on certified, COD, numbered insured, registered or Priority Mail Express: reason shown on the face, receipt stays attached | S4 | pass |
| C35 | Sender signs for returned Priority Mail Express, Registered Mail, COD, Adult Signature and mail insured above a stated value; Certified Mail, Signature Confirmation and Priority Mail Express with a waiver may be returned without a signature when returned as undeliverable | S4 | pass (insured threshold left out on purpose, no amounts) |
| C36 | No return address or unreadable: handled by the local Post Office or sent to the Mail Recovery Center; foreign return address: dead mail procedures | S1 | pass |
| C37 | DMM 507.1.9: dead mail defined; some types opened at a mail recovery center; inquiry by MRC search form at the local Post Office or the Missing Mail online application | S4 | pass |
| C38 | Not arrived within 7 days of mailing: Find Missing Mail, a MissingMail.USPS.com request, or an online claim for insured items | S1 | pass |
| C39 | Missing Mail article covers the search; tracking status article covers "Insufficient Address" and "No Such Number" | repository | pass |
| C40 | Endorsements listed (four names); some require an address-correction fee; definitions not read | S1 | pass |
| C41 | Differences list: citation 604.8.1.2 and 507.1.8.2 against text in 508.1.1.2 and 508.1.1.3; four types against five; "customer pays" against "postage-free"; markings; opened mail; "Returned for Postage Mail" against "Returned for Additional Postage" | S1 to S5 | pass |
| C42 | Not said: "reasonable time" undefined; transit time of a returned piece; telling misdelivery from delivery as addressed; a piece opened by mistake; whom to contact for repeated wrong mail; how long the Mail Recovery Center holds a piece | S1 to S5 (absence; "reasonable time" appears once in DMM 508 and is not defined) | pass (absence) |
| C43 | No prices, fees or percentages; no search-volume claim | article scan (no `$`, no `%`) | pass |

## Image checks (diagram 1200 x 3366)

1. Card 1 matches C7 to C9, C11, C13 (the line "Do not erase the address" replaced an earlier "Keep the address legible" that was not the FAQ's wording). 2. Card 2 matches C15 to C19. 3. Card 3 matches C26, C27, C31, C36, C38; "Marketing Mail: not returned unless endorsed" is the FAQ's wording. 4. The gray card matches C41 and C42. 5. No fee, price or percentage in the picture or the alt text. 6. No text past the right margin (script check returned an empty list). 7. Alt text (1,657 characters) says the same as the picture plus the sources. 8. The SVG and PNG carry no C2PA data (chunk and metadata removed; sizes and hash prefixes equal the originals: PNG 651,486 B `6cb87c7381eb5560`, SVG 6,864 B `63b8d01cc11ba03b`, md 18,995 B `4e94b5b1a20b42dd`).

## Comparison with published posts

| Post | What it already says | Overlap with this draft | Handling |
|---|---|---|---|
| Missing Mail (`usps-missing-mail-search-how-it-works`) | The 7-day search, what to have ready, statuses, items USPS cannot search for | The FAQ 000006175 "not arrived within 7 days" line | One sentence and a link; no search detail repeated |
| Mail Forwarding (`usps-mail-forwarding-how-long`) | Forwarding length, what is forwarded, "returns your mail to the sender for 6 months with a label" after forwarding ends | A forwarding order that has ended as a reason for return | One bullet reporting that post's statement, with a link |
| Tracking status (`usps-tracking-status-what-it-means`) | "Insufficient Address" and "No Such Number": the package is going back and the sender reships | Return as a tracking status | One sentence and a link; the draft does not describe tracking statuses |
| Certified Mail (`usps-certified-mail-how-it-works`) | Signature, 15-day hold, return on the 16th day | Accountable mail refused before signing | One link in the accountable-mail sentence; no hold days repeated |
| Redelivery (draft, `5662d08`) | Scheduling; a "Return to Sender" request in the Redelivery application that cannot be canceled | Choosing return after a notice | Not mentioned in the body because that post is not live; a link is proposed after it is published (internal_link_candidates) |
| How to Address an Envelope | Return address top left; an undeliverable letter can be returned | Why a return address matters | Not linked; no duplicate sentence |

No conflicts in the facts of the published posts were found. The wording "returned to the sender" is used in several posts for different mechanisms; this draft says which page each rule comes from.

## Open points for Gate 2 (shown in the article, not resolved)

- P1. The refusal FAQ cites DMM 604.8.1.2 and 507.1.8.2; the refusal text read is in DMM 508.1.1.2 and 508.1.1.3 (604.8.1.2 on the page covers insufficient postage). The article cites numbers where it found the text and says so.
- P2. The FAQ's non-refusable list has four types; the DMM adds Adult Signature; "customer pays postage" against "postage-free".
- P3. "Refused" on a misdelivered redelivery notice against "Not at this address" on a letter; for the wrong location, write nothing.
- P4. Whether "Not at this address" mail must be unopened is not stated.
- P5. "Reasonable time" is not defined.
- P6. A decision for the reviewer: four internal links (Certified Mail, Mail Forwarding, Missing Mail, Tracking status); each appears once.

## Not checked

The WordPress draft, mobile layout (375 px, 320 px), editor validity and the live page have not been checked; this is a repository draft. Search volume was not checked; Trends numbers are relative indexes.
