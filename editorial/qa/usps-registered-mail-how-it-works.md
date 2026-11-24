# QA — USPS Registered Mail

Article: `content/drafts/usps-registered-mail-how-it-works.md` (draft, 2026-11-24, about 1750 words in the body, one H1, Sources included; meta description 141 characters; alt text 1,530 characters after Gate 2 rounds 1 and 2).

Stage: draft. Gate 1 (Claude) run on 2026-11-24 on the rewritten article. **Gate 2 round 1 (ChatGPT, base `d955818`, user-reported 2026-11-25): FIX, two items, applied 2026-11-25** (section "Gate 2 FIX round 1"); **Gate 2 round 2 (base `0f54285`, user-reported 2026-11-25): FIX, one item, applied 2026-11-25** (section "Gate 2 FIX round 2"); Gate 2 round 3 (changed part only) not yet run. Backlog row 46.

## Handed-over draft
The first draft came in a bundle (commit `6e09600`, another environment). Its brief and QA said factual QA was incomplete. The article here was rewritten after Claude read the live pages; every claim below was tested against them.

## Gate 1 — claim groups
- FAQ 000006061 (May 14, 2025): 35 of 37 phrases, 2 table-spacing artifacts.
- DMM 503.2.1 to 2.5: 43 of 44 phrases, 1 my typo.
- FAQ 000007968 (May 19, 2026), Domestic Registered Mail row: 5 of 5.
- Dollar limits, fees and the cash threshold amount are in the sources and deliberately left out.
- Return Receipt post (WP 174) was a 404 on 2026-11-24 (scheduled for 2026-11-25 15:00 KST): confirm it is public before this post is published; otherwise remove that one link. The other four internal links returned 200.
- Certified Mail post says it does not compare Certified Mail with Registered Mail; this article does not compare either.

## Where the pages differ (shown in the article, not resolved)
- The word "receipt": mailing receipt (PS Form 3806) against the internal system of receipts, which the FAQ says is not readily available.
- Eligible classes: four in the FAQ text; the DMM points to exhibit 1.4 (not read).
- How soon to ask about a missing item: 14 or more days (Missing Mail FAQ) against 15 days (DMM, no declared value); different procedures, relation not stated.

## Image checks
After round 2: PNG 1200 x 3441 px, 671,183 bytes, SHA-256 prefix `1ba07d759a80a7b5`; SVG 6,814 bytes, `2b144bbc91c54d3c`; md 14,991 bytes, `b94cefdaef84a040` (after round 1: PNG 3303 px, `4ea85c7c66d71268`; SVG `566fb9637d0d2dd0`; md `ba1e436d199c255b`; alt 1,435; first version: PNG 3165 px, `19deb80b13b60f6f`; SVG `ac99f8c26c64fc38`; md `1d10c1707fbfc58e`; alt 1,237); C2PA chunk and metadata stripped on the device (hashes equal the originals). The rendering script printed no text past the right margin; the PNG was viewed. Diagram text only repeats facts from the article; alt text matches the front matter and the Markdown alt text. No dollar sign or percent sign in the article.

## Not checked
Search volume; any page not listed in the source notes; WordPress (no draft or schedule exists); mobile and editor checks (after Gate 2 PASS).

## Gate 2 FIX round 1 (2026-11-25, base `d955818`): applied
Findings: (1) the diagram card and alt text said "no scans from facility to facility", which can read as USPS itself having no scans; the FAQ says only that updated scans are not provided to the customer as the piece is processed from facility to facility (the body already limits this to "Registered Mail alone"). (2) The diagram's bottom card set 14 or more days against 15 days without saying they are different procedures: the Missing Mail FAQ's 14 or more days is for a search request and/or a claim; the DMM's 15 days is the mailer's own inquiry for Registered Mail with no declared value; the article must not say the claim filing period equals the search time.

Applied: (1) diagram card 3 now reads "No facility-to-facility updates for customers" and the alt text says "USPS gives customers no facility-to-facility updates for Registered Mail alone". (2) diagram card 4 says the DMM has "a separate mailer inquiry after 15 days from mailing"; the dashed card says 14 or more days (Missing Mail FAQ: search request and/or claim) and 15 days (DMM: mailer inquiry, no declared value) are different procedures and the pages do not tie them together; the alt text says the same; the body bullet in "Where the USPS pages differ" now names each procedure and says neither page relates the two numbers to each other or to the claim filing period (covered in our claims article), so the article does not say they are the same. The rest of the article is unchanged. The FAQ and DMM wording was re-checked against the earlier read (FAQ: "Updated scans are not provided as the piece is processed from facility to facility"; Missing Mail FAQ: "allow fourteen (14) or more days ... submit a search request ... and/or file a claim"; DMM 2.5.1: after 15 days from the mailing date, mailer only, no declared value). Image checks: the rendering script printed no text past the right margin; the PNG was viewed; no dollar sign or percent sign. Nothing is published; Gate 2 round 2 (changed part only) is needed.

## Gate 2 FIX round 2 (2026-11-25, base `0f54285`): applied
Finding: the diagram still set the Missing Mail FAQ's 14 days beside the DMM's 15 days without clearly separating both from the insurance claim filing period. Three different things: (a) the Missing Mail FAQ's guidance to allow 14 or more days before a search request (it also names a claim); (b) the DMM's mailer inquiry after 15 days from mailing for Registered Mail with no declared value; (c) the claim filing period, a separate rule that the pages read for this article do not give (our claims article covers it).

Applied: diagram card 4 says the claim filing period is a separate rule, not given here, and that the DMM has a separate mailer inquiry after 15 days; the dashed card names the three separate things and says the pages do not tie them together; the alt text says the same; the body bullet in "Where the USPS pages differ" lists the three and says the article does not say they are the same; the "If it is lost" section adds one sentence that the period for filing the claim is a separate rule this article does not give. No new factual claim and no number added. The rest of the article is unchanged. Image checks: the rendering script printed no text past the right margin; the PNG was viewed; no dollar sign or percent sign; converted content hash recomputed. Nothing is published; Gate 2 round 3 (changed part only) is needed.
