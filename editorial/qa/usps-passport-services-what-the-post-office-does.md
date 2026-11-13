# QA record — usps-passport-services-what-the-post-office-does

Article: `content/drafts/usps-passport-services-what-the-post-office-does.md` (draft, 2026-11-13; about 1,470 body words without the alt text; one H1, eight H2 sections; no table).
Brief: `research/briefs/usps-passport-services-what-the-post-office-does.md`. Sources: `research/sources/usps-passport-services-what-the-post-office-does.md` (P1 USPS.com "Passports", no update date; P2 USPS FAQ 000007488, Nov 5, 2026).
Stage: **ready, held (not published)**: Gate 1 done 2026-11-13; Gate 2 PASS on `17a6018` after two FIX rounds; revised 2026-11-13 after the State Department pages were opened (translated view, English not verified); changed parts await a new Gate 2. **Rule-type post: re-read both pages (and try the State Department pages again) before any publish or republish.**

## Scope

What two USPS pages say about passport services: the Post Office's role, who applies in person, minors, renewing as USPS.com describes it, appointments and walk-in hours, photos and documents, the two payments without amounts, what happens after applying. **The State Department pages were opened on 2026-11-13 only in a browser translation; their English wording was not verified** (see the revision section below); the article attributes every rule to USPS and does not quote or interpret the State Department sentences. No prices, expedited detail, processing times, lost or stolen passports or international travel rules.

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

## Gate 2 FIX on `27cde5e` (applied 2026-11-13)

1. **Which Post Offices, which services.** The lead, meta description, diagram and alt read as if every Post Office accepts applications and takes photos. USPS.com's wording is "Thousands of Post Offices accept first-time passport applications ... Most of those locations can also take your passport photo" (tested again, found). Fixed everywhere: the lead and the meta description (156 characters) now say thousands of Post Offices accept applications and most of those also take photos; the "What the Post Office does" section says the FAQ's role list applies to the Post Offices that offer passport services; the first diagram card is retitled "What passport Post Offices do" and says "Thousands of Post Offices accept first-time applications; most of those also take photos"; the alt matches.
2. **Expedited renewal wording.** USPS.com says "If you need expedited service for your renewal, you must renew by mail" and labels the mail option "Available with Expedited Service" (found). It describes urgent cases separately: a life-or-death emergency (the State Department processes these by appointment only; visit the Life-or-Death Emergencies page on travel.state.gov) and urgent travel (call the State Department Passport Agency to schedule an appointment) (all found). The diagram card now says "Expedited renewal service: by mail. Urgent travel: a State Department appointment", and the body has a new section, "Expedited service and urgent travel", that separates the two and gives **no time thresholds** on purpose (see the open point below). The alt and the diagram footer say the State Department pages were not read here.
3. **State Department links.** The body now links the State Department's [apply in person as an adult](https://travel.state.gov/en/passports/apply/adults.html) and [renew by mail](https://travel.state.gov/en/passports/renew-replace/mail.html) pages (scope paragraph, the in-person section, the expedited section, and the Sources list as "pointer only; not read in full"). **Access record:** in the built-in browser both pages returned the Cloudflare challenge (HTTP 403) again and it was not bypassed. A summarizing web fetch returned `renew-replace/mail.html` as a paraphrase (not verbatim, no update date shown) and failed for `apply/adults.html` (client error). The paraphrase is **not used for any claim** and no eligibility detail is attributed to those pages; the article says it could not read them and does not rely on their text.

**Open point (not resolved, not stated in the article):** the paraphrased State Department page mentions an appointment rule for travel in under 3 weeks (a window of 14 calendar days), while USPS.com's own heading is "Urgent Travel in Less than 10 Weeks". The paraphrase is unverified, so this may be a summarizing error or a real difference between the pages. That is why the article repeats neither threshold. Re-check both State Department pages directly (a person or a browser that passes the challenge) before publishing, and add the comparison to the article if confirmed.

Image: re-rendered (render check `[]`, viewed in crops); C2PA stripped on the device; PNG 596,737 bytes (`ee4591c3…`), SVG 4,683 bytes (`9b330dc1…`), hashes equal the originals. Front-matter alt equals the body alt (script). Changed parts only: the lead, the meta description, the scope paragraph, two sentences in the role and in-person sections, the renewal sentence, the new expedited section, the Sources list, the first and fourth diagram cards, the footer and the alt.

## Gate 2 re-check on `8953bd9` (2026-11-13)

FIX: "A child's passport is not renewable" (diagram card and alt) read as covering every minor. USPS.com's wording is "A minor's passport cannot be 'renewed'. Instead, each time a minor's passport expires, you must submit a new, first-time passport application in person" and it gives no age in that sentence; its minors heading says "Passports for children under 16 have special requirements"; its renew-by-mail conditions require a passport "issued when you were age 16 or older"; the FAQ's in-person list includes a previous passport issued under 16 (all found at Gate 1). Fixed: the diagram card and the alt now say "A passport issued under 16 is not renewable"; the body keeps USPS's words ("a minor's passport"), says the sentence gives no age, and says the article reads it as covering passports issued to children under 16 and does not extend it further. No other body sentence says a child's or minor's passport is not renewable. The reviewer confirmed the participating Post Offices and photos scope, the expedited/urgent split and the State Department links; the urgent travel dates stay out, pointing to the State Department. Image re-rendered (render check `[]`), C2PA stripped; PNG 600,000 bytes (`686f50fc…`), SVG 4,691 bytes (`eea77db5…`), hashes equal the originals; front-matter alt equals the body alt.

## Gate 2 PASS on `17a6018` (2026-11-13)

The reviewer passed the changed parts. Condition kept by the user: before publishing, read the State Department pages directly; if they cannot be opened and the needed content cannot be checked, report the limit and ask about publishing first. Stage moved to ready (not published).

## Pre-publication State Department check (2026-11-13): publication held

The user's condition was to read the State Department pages directly before publishing. They opened in the user's Chrome (translated to Korean by the browser; details in the source notes). Findings: the in-person list on the adult page is consistent with the FAQ list, and children under 16 cannot renew; the timing rules differ from USPS.com: State Department says life-or-death travel within 14 days, urgent travel in 2 to 3 weeks with an appointment within 14 days of travel (28 days if a visa is needed), expedited service for travel within 6 weeks (acceptance facility or mail renewal), routine for 6 weeks or more; USPS.com says "Less than 10 Weeks" and 72 hours (3 business days). **Important conflict; the article was not published.** The user was informed. The article gives no thresholds, so the numbers are not wrong in it, but two sentences are now inaccurate or incomplete ("could not be read in full"; the pointer-only wording of the two State Department links) and the conflict itself is information a reader needs. Proposed change for a new Gate 2: say the State Department pages were read on Nov. 13, 2026 (with the update dates), show the timing difference between the two sources without resolving it, and keep the State Department links as the place to check. Waiting for the user's decision.

## Revision after the State Department pages were opened (2026-11-13), for a new Gate 2

User decision: keep the post unpublished; reflect what was checked and how; link urgent travel directly to the State Department's latest guidance; explain what the USPS and State Department dates refer to only as far as confirmed; do not quote or assert the meaning of any sentence whose English was not verified.

**How the State Department pages were checked.** The built-in browser still got the Cloudflare 403 (not bypassed). In the user's Chrome the pages showed a security-check interstitial that cleared by itself after about 8 to 10 seconds; no click or other action was taken on it. The text was shown in a Korean machine translation with a few English fragments. Pages: `apply/adults.html` (last updated May 4, 2026 as displayed), `renew-replace/mail.html` (Oct. 1, 2026), `apply/get-fast.html` (Sep. 30, 2026). The English wording was **not** verified, so no State Department sentence is quoted or interpreted in the article.

**Changed parts.**
1. Scope paragraph: no longer says the pages "could not be read in full / pointers only". It says they were opened on Nov. 13, 2026 in a translated view, the English wording was not checked, so everything below is what USPS says and the pages are linked for current rules.
2. In-person section: "did not verify its English wording" in place of "could not read it".
3. "Expedited service and urgent travel" section rewritten. USPS.com part: attributed and quoted (re-tested on the live page today, found verbatim): "The State Department processes these requests by appointment only"; "within 72 hours (3 business days)" (twice: life-or-death travel, and how close to travel the appointment must fall); heading "Urgent Travel in Less than 10 Weeks" (time until travel that leads to the phone call); "you must call the State Department Passport Agency"; Life-or-Death Emergencies page; proof of travel; "If you need expedited service for your renewal, you must renew by mail". State Department part: numbers only, labelled as shown in the translated view (14 days; 2 to 3 weeks; 6 weeks on the get-fast page, 3 weeks and 14 days in an appointment line on the mail page, with the displayed update dates). The article says it did not confirm in English what each number refers to, does not say which source applies or that USPS.com is out of date, and links `get-fast.html` as the place to check directly.
4. "What the pages do not say": the last sentence now says the State Department pages were opened only in a translated view, so agreement with their English text on renewal rules, ages and photos is not checked.
5. Sources: three State Department entries added (adults, renew by mail, get a passport faster), each "opened Nov. 13, 2026 in a translated view, English wording not verified".
6. Diagram: Renew card now reads "Expedited renewal service: by mail. Urgent travel: USPS.com and the State Department give different dates; check the State Dept." and keeps "A passport issued under 16 is not renewable."; footer now says the State Department pages were opened Nov. 13 in a translated view, English not verified. Alt updated to match (front-matter `image_alt` equals the body alt, script check).

**Checks.** Render check `[]`; crops viewed (Renew card six lines, footer four lines, no overflow); C2PA stripped on the device; PNG 632,562 bytes (`74cedff2…`), SVG 4,906 bytes (`a62b57da…`), hashes equal the originals. No `$` or dollar amounts. Meta description unchanged (156 characters). Phrase test on the article text: the five USPS quotes above present. State Department sentences quoted in the article: none.

**Still open (stated in the article or here).** The English wording of the State Department pages is not verified; which of the two sources' dates applies, and whether USPS.com is out of date, is not resolved; search volume was never checked (Trends relative indexes only). Not published. Before any publish: re-read both USPS pages and, if possible, read the State Department pages in English (a person or an English view) and compare again.
