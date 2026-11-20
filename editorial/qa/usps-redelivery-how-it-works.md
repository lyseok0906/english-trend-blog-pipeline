# QA record — usps-redelivery-how-it-works

Article: `content/drafts/usps-redelivery-how-it-works.md` (draft, 2026-11-20; about 2,380 words in the body without the alt text, one H1, nine H2 sections including Sources; two tables; three internal links).
Brief: `research/briefs/usps-redelivery-how-it-works.md`. Sources: `research/sources/usps-redelivery-how-it-works.md` (S1 FAQ 000005320, S2 FAQ 000006169, S3 FAQ 000006180, S4 USPS.com Schedule a Redelivery).
Stage: **draft, Gate 1 done by Claude 2026-11-20; waiting for Gate 2.** Rule-type post: re-read S1 to S4 right before any publishing.

## Method

The four pages were opened in the built-in browser on 2026-11-20 and every statement the article makes was tested by script after normalization (remove marks and quotes, unify dashes, lowercase): S1 81 of 83 phrases at once (the two others failed on list spacing and were confirmed in the text), S2 24 of 24, S3 17 of 17, S4 12 of 12. Absence claims (no list of places; no response time for the service request email) were tested by reading the full text and counting "service request" (S1: only the top-of-page sentence and a technical-support email line; S4: none). Existing posts were read in the repository.

## Gate 1 — Factual QA (claim by claim)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | A free redelivery can be scheduled online, by phone or on the form; a day, not a time; item returned after the return date unless a redelivery is arranged or it is picked up | S1 "Scheduling a Redelivery is free", "may NOT request a specific time"; S2 | pass |
| C2 | Four sources with their numbers and dates (000005320 Sep 16, 2026; 000006169 Apr 7, 2026; 000006180 Jun 29, 2026; USPS.com page without a date) | S1 to S4 | pass |
| C3 | PS Form 3849 "We ReDeliver for You!" is left after an attempt; the five reasons | S1 | pass |
| C4 | The form tells the mailpiece type, why not left and the options (carrier redelivery, Post Office pickup, Smart Locker if the box is checked); "Smart Locker Eligible" label | S3 | pass |
| C5 | Yellow 3849-SD for Sunday attempts: available next business day (excluding holidays) or redelivery by QR code | S1, S3 | pass |
| C6 | Redelivery after the first attempt; Delivery Instructions before | S1 | pass |
| C7 | QR code: quickest way; opens the redelivery page | S1, S3 | pass |
| C8 | Online: tracking or barcode number; 24 hours a day, 7 days a week; address must match; USPS Tracking "Available Actions" only if eligible | S1, S4 | pass |
| C9 | Phone: tracking number; three options only; no Smart Locker; without a tracking number only a notification to the Post Office | S1 | pass |
| C10 | Paper form: non-accountable only; back of the form, a day at least 2 delivery days ahead, where to leave, sign, mailbox; not for Restricted Delivery, Adult Signature, the Sunday form or Smart Locker-eligible items | S1 | pass |
| C11 | In person: notice and photo ID; pickup no later than the day before cancels | S1 | pass |
| C12 | Tracking or barcode number is enough without the paper notice; Informed Delivery can manage redeliveries | S1, S3 | pass |
| C13 | The Informed Delivery article says it does not cover redelivery | repository (`usps-informed-delivery-how-it-works`, scope paragraph) | pass |
| C14 | Availability "many, but not all, areas"; Check Availability with name, address, phone, email | S1, S4 | pass |
| C15 | Same day: by 2 AM CST Monday through Saturday; the page adds "or next day" | S1, S4 | pass |
| C16 | Requested date can be up to the return date; Return Date under "About the missed delivery"; scheduling needs advance notice and not on the return date | S1 | pass (both statements quoted; conflict shown) |
| C17 | Change or cancel no later than the day before; confirmation number and email link, Redelivery page option, Activity History; "Carrier Redelivers" to "Customer will pick up" | S1 | pass |
| C18 | Maximum of one request; Return to Sender cannot be canceled or modified; session expiry | S1 | pass |
| C19 | Weather: next business day; last-day failed attempt: returned; failed scheduled redelivery: service request by email to the Post Office | S1 | pass |
| C20 | Residential: addressee or agent (PS Form 3801 or a letter to the postmaster; identification at the Post Office); original address only; carrier not required to verify an agent | S1 | pass |
| C21 | Name someone on the notice to pick up; not for Registered Mail or Restricted Delivery | S1, S3 | pass |
| C22 | Accountable mail: addressee or agent must sign; signing the notice and leaving it is not enough (both FAQs) | S1, S3 | pass |
| C23 | Business: an individual employee signs; first initial and last name | S1, S3 | pass |
| C24 | USPS Electronic Signature Online for Informed Delivery subscribers: domestic Priority Mail Express, Signature Confirmation, certain insured items | S3 | pass |
| C25 | The Certified Mail article covers who signs | repository (`usps-certified-mail-how-it-works`) | pass |
| C26 | Accountable list and non-accountable list; the Priority Mail Express "unless signature waiver is not required" wording quoted as unexplained | S1 | pass |
| C27 | Return dates table: Priority Mail Express 3 days after the first notice, held 5 days after the first attempt; Certified, Insured, Registered, Signature Confirmation, Adult Signature, Return Receipt for Merchandise, USPS Tracking 5 days and 15 days; COD 5 days and 30 days (table) and 10 days (text); Postage Due 5 days and 15 days | S2 | pass |
| C28 | Calendar days; non-Postal business day goes to the next Postal business day; pickup until close of business on the return date; two notices; no further notice after a late redelivery | S1, S2 | pass |
| C29 | Final Notice box on the peach form; the carrier does not have the item with them | S2 | pass |
| C30 | Ordinary parcel: second attempt next working day, no notice on the first attempt when someone is normally available; notice after the second; notice after the first when nobody is usually available or it is not known; more attempts only on request | S1 | pass |
| C31 | Priority Mail Express: no automatic attempts after the first; second notice on the 3rd calendar day; returned if not picked up or scheduled by close of business 5 calendar days after the first attempt | S1 | pass |
| C32 | Signature mail: notice, available the following business day, redelivery not automatic, second notice 5 days after the first, held by service (usually 15) | S1 | pass |
| C33 | Eligible scan events (eight) and the note "(Customer Pickup and Returned to Sender Only)" | S1 | pass |
| C34 | Reasons you may be unable to schedule: address mismatch, request exists, returned to sender; exceeded attempts message; the Refused / Delivered / Out for Redelivery list shown after the reasons without explanation (not stated as ineligibility) | S1 | pass (wording softened; see FIX note) |
| C35 | Tracking events Prepared for Redelivery and Out for Redelivery | S1 | pass |
| C36 | Differences: return date wording; COD 10 against 30 days; day-before change deadline against the 2 AM CST error-message cutoff; second attempt for ordinary parcels (S1) against the tracking guide's "no automatic second delivery attempt" after the two Notice Left statuses (different situations) | S1, S2; repository tracking post table | pass |
| C37 | The tracking status article reports no time limit; the notice table is where these pages give return dates | repository (tracking post: "it does not give that time limit in these entries"); S2 | pass |
| C38 | No list of places with redelivery; no response time for the service request email | S1, S4 (absence read in full) | pass |
| C39 | No dollar amount or percentage in the article | Body has 0 "$" and no percentage | pass |
| C40 | Internal links return 200: tracking status, Informed Delivery, Certified Mail | to be opened logged out at publication; the three posts are live (checked 2026-11-18 to 2026-11-20 in other QA records) | pass (re-check at publication) |
| C41 | "As of November 20, 2026" and "checked on November 20, 2026" | read dates | pass |

## Image check

| # | Item | Result |
|---|---|---|
| I1 | Card "Notice left: PS Form 3849" matches C3, C4 | pass |
| I2 | Card "Schedule it: free, pick a day" matches C1, C7 to C10, C15 | pass |
| I3 | Card "Change or cancel" matches C17, C18 | pass |
| I4 | Card "Who can accept it" matches C20, C22 | pass |
| I5 | Card "How long it is held (calendar days)": Priority Mail Express 5 days after the first attempt; extra-service items 15 days; COD 30 in one table and 10 in the text; Return Date on the final notice (C27, C29, C36) | pass |
| I6 | Card "When you cannot schedule one": an item already returned to the sender; a request already exists; address does not match (C34); "delivered / refused" removed after the source check because the FAQ list was not explained | pass |
| I7 | Footer "Sources: USPS Redelivery FAQs and the USPS.com Schedule a Redelivery page; read Nov. 20, 2026" | pass |
| I8 | No logos, photos or USPS marks; text 28 to 46 px on an 800 px canvas; no text past the right margin (script check `[]`) | pass |
| I9 | Alt text (1,295 characters) says the same as the diagram and the body (alt equals the body image text and the front matter); the SVG `<title>` is the same text without the sources line | pass |
| I10 | Files: `assets/optimized/usps-redelivery-how-it-works.png` (1200 x 3447, 614,746 bytes, sha256 `d76325424237c79f...`), `assets/raw/usps-redelivery-how-it-works.svg` (6,245 bytes, `705c6604f0be1cee...`); the C2PA chunk and SVG metadata added by the device transfer were removed on the device and the hashes and sizes equal the originals | pass |

## Front matter and format

Title 61 characters; slug `usps-redelivery-how-it-works`; meta description 145 characters; focus keyword `usps redelivery` appears in the title and the meta description; category Postal service and stamps; no price. The body is long (about 2,380 words); deadlines and how to schedule come before the hold table, and the differences are kept because accuracy comes first.

## Comparison with published posts

No direct contradiction was found.

1. **Tracking status post.** It lists three options for the two Notice Left statuses and says a redelivery cannot be scheduled for Available for Pickup and Held at Post Office, At Customer Request. S1 agrees: "Available for Pickup" is on the eligible list only for "Customer Pickup and Returned to Sender". The tracking post says the guide gives no time limit; the new post gives the return dates from S2. "No automatic second delivery attempt" (tracking guide) and the ordinary-parcel second attempt (S1) concern different situations; shown in the new article.
2. **Informed Delivery post.** Says it does not cover package redelivery. Consistent; the new post says so.
3. **Certified Mail post.** Says Certified Mail is held 15 days and returned on the 16th day (FAQ), and DMM 508.1.1.7 on notice and redelivery. S2 gives 15 days for Certified Mail. Consistent. The COD difference does not touch that post.
4. **Hold Mail post.** Mentions a PS Form 3849 for overflow mail; not contradicted.
5. **Follow-up edits (not applied, need approval after publication):** a link-only edit to the tracking status post (sentence "it does not give that time limit") and possibly to the Certified Mail post.

## Open points for Gate 2

- **P1 (length):** about 2,380 words; the reviewer may ask for a shorter hold section.
- **P2 (COD):** shown as "30 days in the table (10 days in the text)"; the article does not pick one.
- **P3 (return date):** the two FAQ statements are quoted and left open.
- **P4 (Refused / Delivered / Out for Redelivery):** shown as an unexplained list, not as ineligibility.
- **P5 (before publishing, mandatory):** re-read S1 to S4; if a cutoff, a return day, a method or the eligibility list changed, report before publishing.

## Result and next step

Gate 1: **PASS** (41 of 41 claims, 10 of 10 image checks). Next: user push, Gate 2 by commit SHA, then approval to move to `ready`; WordPress only after the Gate 2 PASS.

## Gate 2 round 1 (reviewer, on `5662d08`): FIX — applied 2026-11-20

**Finding.** The diagram, the front-matter alt and the body image alt said that for signature mail "you or your agent must be there", and the body sentence before the electronic-signature sentence said the addressee or an agent "must be present to sign". The PS Form 3849 FAQ (S3) answers "Do I have to be present to sign for my mailpiece?" with "Maybe": an Informed Delivery subscriber can sign up for USPS Electronic Signature Online and sign electronically for domestic Priority Mail Express items, Signature Confirmation items and insured items over a stated value; "Otherwise, you or an authorized agent must be present to sign for accountable mail being delivered by a mail carrier"; and signing the notice and leaving it for the carrier "does not meet the minimum requirements for redelivery".

**Changes (four places, same meaning):**
1. Body, "Who can accept it", second paragraph: now quotes the FAQ's question and "Maybe", gives the Electronic Signature Online option limited to Informed Delivery subscribers and the three named services (insured items "over a stated value", no amount), then "Otherwise … you or an authorized agent must be present", then "signing the notice and leaving it … does not meet the minimum requirements for redelivery". The business-signer sentence and the Certified Mail link are unchanged.
2. Diagram card "Who can accept it": "Signature mail: you or your agent must be there, unless you use USPS Electronic Signature Online (Informed Delivery; certain services). Signing the notice is not enough." Card grew by three lines; image now 1200 x 3654.
3. Front-matter `image_alt` and 4. body image alt: "for signature mail, you or your agent must be there unless you use USPS Electronic Signature Online, which Informed Delivery subscribers can use for certain services; signing the notice is not enough." The SVG `<title>` has the same text.

**Re-check against S3 (read again 2026-11-20 in the built-in browser):** 7 of 7 phrases matched (the question and "Maybe"; the Informed Delivery subscriber and Electronic Signature Online sentence; the three services; "Otherwise …"; the minimum-requirements sentence; the business employee sentence and the first-initial-and-last-name sentence). The earlier claim C22 ("both FAQs say that signing the notice … is not enough") is kept; the body wording "minimum requirements" follows S3. The COD 10 days (text) against 30 days (table) display is kept, as the reviewer said it may be.

**Files after the fix:** md 17,826 B `e484d0c8b0097886`; PNG 1200 x 3654, 656,925 B `c150364d073cced2`; SVG 6,680 B `a51ccf29174defed` (no C2PA data; equal to the originals). The script check for text past the right margin returned an empty list. The WordPress draft and mobile layout are still not checked.
