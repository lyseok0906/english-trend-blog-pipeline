# QA record — real-id-to-fly-what-tsa-accepts

Article: `content/drafts/real-id-to-fly-what-tsa-accepts.md`
Brief: `research/briefs/real-id-to-fly-what-tsa-accepts.md`. Sources: `research/sources/real-id-to-fly-what-tsa-accepts.md` (S1 TSA "Acceptable Identification at the TSA Checkpoint", S2 TSA "REAL ID", S3 TSA "About TSA ConfirmID").
Stage: draft written 2026-10-07; Gate 1 done by Claude on 2026-10-07. Not sent to Gate 2, not approved, not on WordPress, not published.

Method: all three TSA pages were opened again in the built-in browser on 2026-10-07; their text was read in full, and after the draft was written the quoted statements were tested against the page text by script (25 phrases on S1, 4 on S2, 5 on S3): all present. The ConfirmID fee amount is on the pages and is not used (user decision 2026-10-07). This is the drafting and factual-QA re-check required for rule posts; the re-check right before the user approves moving to `ready` and again right before publishing is still **mandatory**; if a page cannot be opened, do not publish.

## Gate 1 — Factual QA (claim by claim)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | Lead: you need an ID that is on TSA's list, a REAL ID is one of them; TSA says adults 18 and older must show valid identification at the airport checkpoint; a state license or ID card must be REAL ID compliant to be on the list; a U.S. passport is also on the list | S1-1, S1-3, S1-6 | pass (attributed; the "must be REAL ID compliant" sentence restates S1-6 and S2-2) |
| C2 | Wording as of October 7, 2026; three TSA pages; TSA says its list "is subject to change without notice" and encourages checking it again before traveling | Browser reads; S1-2 | pass (quote 6 words) |
| C3 | TSA says REAL ID enforcement began on May 7, 2025; as of that date non-compliant state licenses and IDs are no longer accepted as valid identification at airports | S2-1, S1-6 | pass |
| C4 | (revised after Gate 2, see the Gate 2 final section) TSA's REAL ID page says that a traveler using a state-issued driver's license or ID card for a domestic flight must use one that is REAL ID compliant. TSA's identification page also lists other acceptable forms of ID, including a U.S. passport | S2-2, S1-6, S1-3 | pass (see note) |
| C5 | Passengers should either travel with an acceptable alternative form of ID, like a passport, or enroll for a state-issued REAL ID through their state DMV | S1-6 | pass (attributed) |
| C6 | If unsure whether an ID complies with REAL ID, check with your state DMV; a temporary driver's license is not acceptable | S1-4 | pass (attributed) |
| C7 | Table: REAL ID-compliant license or ID, Enhanced Driver's License or Enhanced ID, passport, passport card, DHS trusted traveler cards (Global Entry, NEXUS, SENTRI, FAST), U.S. Department of Defense ID including dependents, permanent resident card and Tribal Nation photo ID are on the list | S1-3 | pass |
| C8 | Table: a non-REAL ID state license or ID is no longer accepted at airports as of May 7, 2025; a temporary license is not acceptable | S1-6, S1-4 | pass |
| C9 | Table: TSA accepts certain mobile driver's licenses issued by states approved for federal use; the mDL must be based on a REAL ID, EDL or EID | S1-5 | pass |
| C10 | "TSA's list has many more entries than these" | S1-3 (the page lists 17 forms, plus digital IDs in testing) | pass |
| C11 | TSA currently accepts expired ID up to two years after expiration, for the forms on its list | S1-8 | pass (attributed; "currently" kept) |
| C12 | Children under 18 are not required to show ID for travel within the United States; unaccompanied minors eligible for TSA PreCheck must show an acceptable ID for expedited screening; contact the airline about its own requirements | S1-9 | pass (attributed) |
| C13 | From February 1, 2026 a traveler without an acceptable ID has the option to pay a fee to use TSA ConfirmID; TSA then attempts to verify identity; ConfirmID is a fee-based service | S1-7, S3-1 | pass (no amount) |
| C14 | The process takes an average of 10 to 15 minutes but could take 30 minutes or more | S3-2 | pass (attributed) |
| C15 | If identity cannot be verified, the traveler will not be allowed to enter the screening checkpoint | S1-10 | pass (attributed) |
| C16 | Scope: no how-to for REAL ID (TSA's page links each state's plan), no international travel, airline rules, federal-facility access, immigration status, fee amount, full list, digital ID programs beyond the mobile license condition, no advice | S2-4; scope statement | pass (scope) |
| C17 | Sources: all three checked October 7, 2026; none shows an update date | Browser reads | pass |
| C18 | Source titles and URLs | Page titles: "Acceptable Identification at the TSA Checkpoint", "REAL ID", "About TSA ConfirmID" | pass |

### Image (`assets/optimized/real-id-to-fly-what-tsa-accepts.png`, original SVG in `assets/raw/`)

- Own flowchart, no photos, no license, passport or REAL ID star, no TSA logo. 1200x2607. Every line traces to the claims above: "Adult 18 or older at the TSA checkpoint" (C1); "Is your ID on TSA's list? The list can change without notice (TSA)" (C2); the example IDs (C7); "Not accepted since May 7, 2025: a state license or ID that is not REAL ID compliant" (C3); "Fee-based identity check", "Average 10-15 minutes; could take 30 minutes or more", "If identity cannot be verified: no entry to the checkpoint" (C13 to C15); "Source: TSA pages, read Oct. 7, 2026" (C17). No fee amount.
- The vertical layout puts the "if no" card after the "if yes" card; the arrow between them is labeled "ID is not on the list".
- Alt text in the front matter and the body is identical (540 characters; the example list in the alt is shorter than the diagram's).
- File check on the device: pixel hash of the PNG matches the cloud render (md5 of RGB bytes c4e1f3ca...). Visual check of the render: no text overflow.

### Handled by wording

- All rule statements are attributed to TSA with "TSA says"; the article names the as-of date and says the list can change without notice.
- The ConfirmID purpose wording on the page is not quoted. The fee amount is left out; "fee-based" only.
- "Currently" is kept for the expired-ID statement, as TSA words it.
- No advice such as "get a REAL ID now"; the passport alternative is TSA's own statement.

### Not verified

- Whether TSA's list changes after today (it can change without notice; the mandatory re-check covers this).
- The mobile driver's license state approvals (TSA's linked page was not opened).
- The 17-entry count behind "many more entries" was read from the page text, not recounted on a second pass.
- Search volume and competition for the focus keyword (not measured).
- The exact diagram text size on a real phone (to be checked in the WordPress preview).

### Re-check obligations

**Mandatory**: re-read S1, S2 and S3 right before the user approves moving the article to `ready`, and again right before publishing. Compare the acceptable-ID list, the May 7, 2025 wording, the expired-ID and children statements and the ConfirmID description. If a page differs or cannot be opened, return to draft or do not publish.

## Gate 2 (ChatGPT, 2026-10-07, result reported by the user)

**FIX REQUIRED, applied.** The first answer and the meta description now answer directly whether a REAL ID is required.

| Change | Before | After |
|---|---|---|
| `meta_description` (138 characters) | "TSA says adults need an ID on its list, and a state license must be REAL ID compliant. See what else TSA accepts and what happens without one." | "No. Adults need an ID on TSA's list; a REAL ID-compliant state license or ID is one option. See alternatives and what happens without one." |
| Bold first sentence | "You need an ID that is on TSA's list, and a REAL ID is one of them." | "No—not necessarily. You need an ID on TSA's list, and a REAL ID-compliant state license or ID is one option." |
| Next sentences | "TSA says adults 18 and older ... checkpoint. A state license or ID card must be REAL ID compliant to be on the list. A U.S. passport is also on the list." | "TSA says adults 18 and older must show valid identification at the airport checkpoint. A U.S. passport is also on the list." then "A state license or ID card must be REAL ID compliant to be on the list." |

Claim check for the new wording (Gate 1 re-run on the changed sentences): "You need an ID on TSA's list" and "adults 18 and older must show valid identification" are TSA statements already in the Gate 1 table; "a REAL ID-compliant state license or ID is one option" and "a U.S. passport is also on the list" are on TSA's list (the ID table in the article); "not necessarily" follows from the TSA identification page, which tells passengers to travel with an acceptable alternative ID such as a passport or to enroll for a REAL ID. Result: pass. No diagram change (the flowchart already starts from "is the ID on TSA's list"). Alt text unchanged (540 characters; Gate 2 did not ask to shorten it).

Left as it was, for the re-review: the section "What TSA says about REAL ID" still reports, attributed to TSA's REAL ID page, that U.S. travelers must be REAL ID compliant to board domestic flights, followed by the identification page's alternatives. The two statements are both TSA's and are shown together.

Not sent back to Gate 2 yet. For the changed articles, ChatGPT will re-review the fix commit.

## Gate 2 final (ChatGPT, 2026-10-07, result reported by the user)

One more sentence fix was requested for this article and applied. In the section "What TSA says about REAL ID", the sentence

- Before: "TSA's REAL ID page says U.S. travelers must be REAL ID compliant to board domestic flights and to access certain federal facilities."
- After: "TSA's REAL ID page says that a traveler using a state-issued driver's license or ID card for a domestic flight must use one that is REAL ID compliant. TSA's identification page also lists other acceptable forms of ID, including a U.S. passport."

Claim check: the REAL ID page's own words (S2-2) are "U.S. travelers must be REAL ID compliant to board domestic flights and access certain federal facilities"; the identification page (S1-6) says non-compliant state licenses and IDs are no longer accepted at airports and that passengers should bring an acceptable alternative like a passport or enroll for a REAL ID; and the list on that page includes a U.S. passport (S1-3). The new sentence 2 is S1-3 and S1-6. The new sentence 1 narrows the REAL ID page's wording to travelers who use a state license or ID card, which is the reading S1-6 supports; the narrowing is therefore a combination of S2-2 and S1-6, although the sentence attributes it to the REAL ID page. Result: pass, with this note for the record. The federal-facilities clause is no longer in the body; the scope section still says the article does not cover access to federal facilities.

**Gate 2 final result: PASS** for this article (after this fix), as reported by the user.

## Mandatory pre-approval re-check (2026-10-08)

Before asking for the ready-move approval, the TSA pages were opened again in the built-in browser and their text tested by script (strings normalized for case, quotes, registered marks, asterisks and spacing):

| Page | Strings tested | Present |
|---|---|---|
| S1 TSA "Acceptable Identification at the TSA Checkpoint" (https://www.tsa.gov/travel/security-screening/identification) | 25 (18+ must show ID; list subject to change; REAL ID-compliant license, EDL/EID, mobile driver's license condition, passport, passport card, DHS trusted traveler cards, DoD ID, permanent resident card, Tribal Nation photo ID; temporary license not acceptable; May 7, 2025 wording and the alternative-ID sentence; ConfirmID option from February 1, 2026; expired ID up to two years; children; unaccompanied minors; identity not verified means no entry) | 25 of 25 |
| S2 TSA "REAL ID" (https://www.tsa.gov/realid) | 4 (enforcement began May 7, 2025; "must be REAL ID compliant to board domestic flights and access certain federal facilities"; REAL ID Act 2005; state selector) | 4 of 4 |
| S3 TSA "About TSA ConfirmID" (https://www.tsa.gov/tsaconfirm-id/about-confirmid) | 3 (fee-based service; lost ID or no REAL ID; average 10-15 minutes, could take 30 minutes or more) | 3 of 3 |

The ConfirmID fee amount, which the pages show, remains unused in the article. The two sentences changed after Gate 2 (the REAL ID page sentence and the identification page's list of alternatives) rest on S2 and S1 strings that are all still present.
**Result: no difference from the source notes; no article change.** The check is dated 2026-10-08; the as-of date in the text is October 7, 2026 (the day the pages were first read for this article, and no wording changed in between). Ready-move approval has not been given yet; a fresh read right before publishing is still **mandatory**.

