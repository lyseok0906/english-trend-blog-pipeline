# QA record — usps-passport-services-what-the-post-office-does

Article: `content/drafts/usps-passport-services-what-the-post-office-does.md` (draft, 2026-11-13; about 1,470 body words without the alt text; one H1, eight H2 sections; no table).
Brief: `research/briefs/usps-passport-services-what-the-post-office-does.md`. Sources: `research/sources/usps-passport-services-what-the-post-office-does.md` (P1 USPS.com "Passports", no update date; P2 USPS FAQ 000007488, Nov 5, 2026).
Stage: **draft, Gate 1 done 2026-11-13** (waiting for Gate 2). **Rule-type post: re-read both pages (and try the State Department pages again) before any publish or republish.**

## Scope

What two USPS pages say about passport services: the Post Office's role, who applies in person, minors, renewing as USPS.com describes it, appointments and walk-in hours, photos and documents, the two payments without amounts, what happens after applying. **The State Department pages were not read in full** (Cloudflare challenge, not bypassed); the article says so and attributes every rule to USPS. No prices, expedited detail, processing times, lost or stolen passports or international travel rules.

## Method

After drafting, both pages were opened again in the built-in browser (2026-11-13) and tested by script after normalization: P1 45 of 45 phrases (page `textContent`, which includes the collapsed step text); P2 47 of 47 phrases (article slice 20,004 characters; article number 000007488 and the date Nov 5, 2026 present). Absence tests: P1 has "walk-in" once (the banner), no "last updated" or "revised"; "cash" appears once on P1 (in the money order note, not as an acceptance fee method), which matches the article's statement that USPS.com lists a check, money order, debit card or credit card; P2 has no "walk-in" and no "16 or under"; P2 has no "cannot renew in". Internal link checked from the live site (logged out): the REAL ID post returns 200 (title matches) and states that a passport is on the accepted list; the new slug returns 404. Front-matter alt equals the body alt (script). Draft has no "$".

## Gate 1 — Factual QA (claim by claim)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | The Postal Service accepts first-time applications, takes authorized photos, reviews and forwards the application; does NOT issue or create passports; passports are not picked up at a Post Office and are mailed by the State Department | P2 | pass |
| C2 | FAQ: renewals, lost or stolen replacements and name changes go to the State Department's website | P2 | pass |
| C3 | Private "passport expeditors" may submit applications; the FAQ points to the State Department | P2 | pass |
| C4 | USPS.com intro: thousands of Post Offices accept first-time applications; most also take the photo, including digital photos for online renewals | P1 | pass |
| C5 | In-person (DS-11) list of six conditions; otherwise "may be eligible to Renew by Mail using Form DS-82" | P2 | pass |
| C6 | Minors under 16: in person with both parents or guardians, evidence of relationship, identification, consent; 16 and 17: appear in person, parent or guardian ID if the minor has none, consent may be requested | P2 | pass |
| C7 | USPS.com: "children under 16 have special requirements"; a minor's passport cannot be renewed and each expiry needs a new first-time application in person | P1 | pass |
| C8 | Age wording differs: "16 or under" (P1 first-time text) against "under age 16" (P2) | P1; P2 | pass (absence tested) |
| C9 | USPS.com: renew by mail or online if eligible; cannot renew in person; expedited renewals by mail; not eligible by mail means apply in person as a first-time applicant | P1 | pass |
| C10 | Renew by mail conditions (possession, undamaged, issued at 16 or older, within 15 years, current name or documentable change) and renew online conditions (10 years, expiry within 1 year or expired under 5 years, age 25 or older, no personal information change, no travel for at least 6 weeks, U.S. state or territory address, not APO, FPO or DPO, passport in hand and not reported lost or stolen); digital photo needed | P1 | pass |
| C11 | Mailed renewal: the State Department recommends a USPS tracking service (P1); the FAQ names Priority Mail Express and Priority Mail | P1; P2 | pass |
| C12 | Appointments: Step 3 (set hours; need to schedule online or at a lobby kiosk); banner (adds retail counter; limited walk-in hours at select locations; no locations named); FAQ (online, phone IVR for up to six applicants, kiosk; renewals cannot be made with the scheduler or kiosk; employees cannot create appointments online) | P1; P2 | pass |
| C13 | Photos: many Post Offices for a fee; FAQ requirements list and its 2017 State Department source credit; hard copy for Renew by Mail, digital for Renew Online; photo-only appointment | P1; P2 | pass |
| C14 | First-time documents (unsigned form, proof of identity and of citizenship with photocopies, fees); DS-11 completed on the State Department site, printed, "DO NOT SIGN"; FAQ: USPS does not provide the forms; digital IDs not accepted | P1; P2 | pass |
| C15 | Two separate payments (State Department and USPS acceptance); cards not accepted for the State Department; USPS payment methods differ between the pages (FAQ lists cash; USPS.com does not); no amounts | P1; P2 | pass |
| C16 | Processing time starts when the State Department receives the application; passport and citizenship documents may arrive in two mailings; contact NPIC if no second mailing within 10 business days | P2 | pass |
| C17 | Status: Online Passport Status System; may not get a status update for 2 weeks after applying | P1 | pass |
| C18 | REAL ID post: a passport is on TSA's accepted ID list | live REAL ID post | pass |
| C19 | State Department pages not read in full; no rule in the article is attributed to them | method | pass |

## Image checks

800 px wide SVG, 1200 px wide PNG (scale 1.5), render check printed `[]`, viewed in crops. The card texts were corrected after the first render (the "set hours" line was reworded to match the banner and Step 3; "a minor's passport: always a new first-time application" became "a child's passport is not renewable (USPS.com)"). Alt text equals the front-matter alt and describes every card. C2PA metadata stripped on the device and the SHA-256 and sizes equal the originals (PNG 553,373 bytes, `9966b73c…`; SVG 4,426 bytes, `16dd8b9a…`).

## Format

One H1, H2 sections, no table (the sections are prose), a bulleted list only for Sources, meta description 155 characters, focus keyword `usps passport` in the title and the lead.

## Open points for Gate 2

- Confirm the attribution wording: every rule is "what USPS says", with the State Department pages stated as not read.
- Confirm the three differences (age wording, appointments and walk-ins, USPS payment methods) are shown and not resolved.
- Dated rule post: both pages are re-read right before publishing, the State Department pages are tried again, and any conflict is reported before publishing.
