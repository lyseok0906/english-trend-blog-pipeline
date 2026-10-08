# QA record — usps-mail-forwarding-how-long

Article: `content/drafts/usps-mail-forwarding-how-long.md`
Brief: `research/briefs/usps-mail-forwarding-how-long.md`. Sources: `research/sources/usps-mail-forwarding-how-long.md` (S1 USPS "Standard Forward Mail & Change of Address", S2 USPS FAQ "Mail Forwarding Options", S3 USPS FAQ "Extended Mail Forwarding").
Stage: draft written 2026-10-07; Gate 1 done by Claude on 2026-10-07. Not sent to Gate 2, not approved, not on WordPress, not published.

Method: the three USPS pages were opened again in the built-in browser on 2026-10-07; their text was read and the quoted statements tested by script against the page text (S1 18 phrases, S2 the FAQ sentence, S3 12 phrases): all present. This is the drafting and factual-QA re-check required for rule posts; the re-check right before the user approves moving to `ready` and again right before publishing is still **mandatory**; if a page cannot be opened, do not publish.

## Gate 1 — Factual QA (claim by claim)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | USPS says standard mail forwarding lasts 12 months | S1-1 | pass (attributed) |
| C2 | When forwarding ends, USPS returns mail to the sender for 6 months with a label that has the new address | S1-12 | pass (attributed) |
| C3 | A paid extension is possible for a permanent change of address | S1-2, S3-2 | pass |
| C4 | Wording as of October 7, 2026; three USPS pages; no prices, no advice | Browser reads; scope | pass |
| C5 | Forwarding may begin within 3 business days; best to allow up to 2 weeks | S1-3 | pass (attributed) |
| C6 | USPS says identity must be verified to submit a change of address | S1-13 | pass (attributed; no fee mentioned) |
| C7 | The FAQ separates permanent (12 months) from temporary (a specified period of time) | S2-1, S2-2 | pass (attributed) |
| C8 | The forwarding page says a temporary change of address is for relocating 15 days up to 1 year | S1-10 | pass (attributed) |
| C9 | Mail is forwarded piece by piece | S1-4 | pass (attributed) |
| C10 | Free: First-Class Mail and periodicals (newsletters and magazines); Priority Mail Express, Priority Mail and USPS Ground Advantage | S1-5, S1-6 | pass (attributed) |
| C11 | Media Mail is forwarded, customer pays shipping from the local Post Office | S1-7 | pass (attributed) |
| C12 | USPS Marketing Mail is not forwarded | S1-8 | pass (attributed) |
| C13 | The pages differ on periodicals: page says free, no separate limit; FAQ says "primarily First-Class Mail service for 12 months and Periodicals for 60 days" | S1-5, S2-1 | pass (each attributed; the one quote is USPS's words minus the registered mark; "gives no separate time limit" reflects the page text read) |
| C14 | The FAQ adds that it generally does not forward Marketing Mail or Package Services Mail | S2-1 | pass (attributed, "generally" kept) |
| C15 | Extra time in 6-, 12- or 18-month increments, not to exceed 18 months of extended time, in addition to the initial 12 months | S3-1, S1-2 | pass (attributed) |
| C16 | "Up to 30 months in all" is the article's arithmetic (12 + 18), labeled as not a USPS statement | S1-1 + S3-1 | pass (computed, labeled) |
| C17 | Only for a permanent change of address, and a permanent, domestic request | S3-2 | pass (attributed) |
| C18 | Can be bought with the initial request, or later with the confirmation code and the new ZIP Code | S3-3 | pass (attributed) |
| C19 | A reminder email at the 11th month | S3-4 | pass (attributed) |
| C20 | After 6 months, another 6-month interval can be added until 18 months | S3-6 | pass (attributed) |
| C21 | Once the request has expired, the extension can no longer be bought | S3-7 | pass (attributed) |
| C22 | The extension request cannot be changed; canceling the change of address cancels it; no refund; the forwarding page says it cannot be canceled or refunded | S3-5, S1-11 | pass (attributed) |
| C23 | Classes forwarded during the extension: First-Class Mail, USPS Ground Advantage Commercial items, Priority Mail | S3-8 | pass (attributed) |
| C24 | A change of address order only changes the address with the Post Office; the customer must still update government agencies and companies | S1-9 | pass (attributed) |
| C25 | For an absence of 3 to 30 days, the page points to Hold Mail | S1-14 | pass (attributed) |
| C26 | Internal link to the Hold Mail draft (https://statesideexplained.com/usps-hold-mail-how-it-works/) | Pipeline | **link works only after that article is published** |
| C27 | Scope: no prices or fees, Premium Forwarding Service, business or military, deceased, international, identity problems | Scope statement | pass (scope) |
| C28 | Sources: all three checked October 7, 2026; FAQ dates Aug 26, 2026 and Jul 11, 2026; forwarding page no date | Browser reads | pass |

### Image (`assets/optimized/usps-mail-forwarding-how-long.png`, original SVG in `assets/raw/`)

- Own timeline (three steps plus one dashed optional card), no photos, no USPS logo. 1200x2697. Every line traces to the claims above: C5, C9, C1, C10 (the card says only that First-Class Mail is forwarded for free, to avoid the periodicals discrepancy), C12, C3, C15, C17, C22, C2, C28. Visual check of the render: no text overflow.
- Alt text in the front matter and the body is identical (356 characters).
- File check on the device: pixel hash of the PNG should match the cloud render (md5 of RGB bytes 09b531c7...); checked at commit.

### Handled by wording

- Every rule statement is attributed to USPS; the periodicals difference is reported from each page, not resolved; "up to 30 months" is labeled as arithmetic.
- No prices, no fee, no advice on which option to choose.

### Not verified

- Which of the two USPS statements on periodicals is current in practice (USPS does not reconcile them).
- Whether the "Change of Address - The Basics" FAQ adds conditions (not read).
- Whether durations or the extension terms change after today (the mandatory re-check covers this).
- Search volume and competition for the focus keyword (not measured; third-party pages rank ahead of USPS's).
- Diagram text size on a real phone (to be checked in the WordPress preview).
- The internal link to the Hold Mail article is dead until that article is published.

### Re-check obligations

**Mandatory**: re-read S1, S2 and S3 right before the user approves moving the article to `ready`, and again right before publishing. Compare 12 months, 6/12/18-month increments and the 18-month maximum, 3 business days / 2 weeks, 6 months of return-to-sender, the periodicals wording on both pages, and the FAQ page dates. If a page differs or cannot be opened, return to draft or do not publish.

## Gate 2 (ChatGPT, 2026-10-07, result reported by the user)

**FIX REQUIRED, applied.** The 12 months is now tied to a permanent change of address in the first answer, the meta description and the diagram, and the temporary-change wording no longer conflicts with the first answer.

| Change | Before | After |
|---|---|---|
| `meta_description` (144 characters) | "USPS standard mail forwarding lasts 12 months, with paid extensions for permanent moves. See what is forwarded and what happens when it ends." | "For a permanent change of address, USPS mail forwarding lasts 12 months. See what is forwarded, extension options and what happens when it ends." |
| First three sentences | "USPS says standard mail forwarding lasts 12 months. After that, USPS says it returns mail to the sender for 6 months ... A paid extension is possible for a permanent change of address." | "For a permanent change of address, USPS says standard mail forwarding lasts 12 months. For a temporary change, USPS says mail is forwarded for the period you specify. A paid extension is possible for a permanent change of address." |
| Diagram, step 2 title | "2. Standard forwarding: 12 months" | "2. Permanent forwarding: 12 months" |
| Alt text (front matter and body, identical, 357 characters) | "Standard forwarding: 12 months." | "Permanent forwarding: 12 months." |
| `internal_link_candidates` | Hold Mail (drafted) | Hold Mail (drafted; keep the link only if Hold Mail is published first, otherwise remove it) |

Claim check: "for a permanent change of address ... 12 months" is S2-1 (the FAQ ties 12 months to a permanent change of address) together with S1-1 (the forwarding page's 12 months); "for a temporary change ... the period you specify" is S2-2 ("a specified period of time"); the extension sentence is S3-2. The sentence about the 6 months of return-to-sender is no longer in the introduction; it stays in the section "When forwarding ends" (S1-12). The diagram was re-rendered (1200x2697, no text overflow; pixel hash md5 of RGB 676147eb...); the PNG and SVG on the device match the cloud render. Result: pass.

**Publish-order condition (Gate 2).** The internal link to the Hold Mail article (C26) may stay only after the Hold Mail article is live. Publish Hold Mail first; if this article must go first, remove the link. Check this at the `ready` move and before publishing.

## Gate 2 final (ChatGPT, 2026-10-07, result reported by the user)

The fixed version (commit `4746e4a`) was re-reviewed: **Gate 2 final PASS**. No further changes requested. The publish-order condition stands: keep the internal link to the Hold Mail article only if Hold Mail is published first; otherwise remove it.


## Mandatory pre-approval re-check (2026-10-08): DIFFERENCE FOUND on S1

The three USPS pages were opened again in the built-in browser and tested by script (strings normalized for case, quotes, dashes, registered marks and spacing).

| Page | Result |
|---|---|
| S2 USPS FAQ "Mail Forwarding Options" (Aug 26, 2026) | the permanent-change sentence (12 months, Periodicals 60 days, Marketing Mail and Package Services Mail generally not forwarded) and "a specified period of time" present; **unchanged** |
| S3 USPS FAQ "Extended Mail Forwarding" (Jul 11, 2026) | all 7 quoted statements present; **unchanged** |
| S1 USPS "Standard Forward Mail" (no date shown) | the 12 months and 6/12/18-month extension sentence, "can't cancel or request a refund", the 6-month return-to-sender note, piece by piece, Priority Mail Express / Ground Advantage / Media Mail, 15 days up to 1 year, 3-30 days Hold Mail and the change-of-address-only-changes-the-Post-Office note: present. **Three statements the article relies on changed** (see below) |

What changed on S1 (current wording, quoted from the page):

1. Start timing. The sentence "Although mail forwarding may begin within 3 business days of your submitted request, it's best to allow up to 2 weeks" is no longer on the page. The page now says: "Once your request is approved, allow at least 7-10 business days for it to go into effect."
2. Periodicals. The page now says: "Periodicals (newsletters and magazines) are forwarded for free for 60 days if fully prepaid by the sender." (before: forwarded for free, no time limit). This now agrees with the FAQ's 60 days, so the article's paragraph about the two pages describing periodicals differently is no longer true.
3. Marketing Mail. The page now says: "USPS Marketing Mail is not forwarded unless the sender has paid forwarding postage." (before: not forwarded).

Still stated as before: First-Class Mail, Priority Mail Express, Priority Mail and USPS Ground Advantage forwarded for free; Media Mail forwarded with the customer paying shipping from the local Post Office; "piece by piece"; the reminder email (S1 now says when 1 month is left, S3 says the 11th month mark, which agree for a 12-month period).

**Result: the article is affected in the lead-in section ("The 12 months and how it starts"), in "What gets forwarded" (the periodicals discrepancy paragraph and the Marketing Mail sentence) and in the diagram text and its alt text ("forwarding may begin within 3 business days; allow up to 2 weeks").** The 12-month answer, the meta description and the Extended Mail Forwarding section are not affected. The article was not changed in this step and the ready-move approval is not requested; the user decides how to fix it (proposed fixes in the decision log). Because the text and the diagram change after Gate 2 final PASS, a new Gate 2 check of the changed parts is needed before the move to `ready`.


## Fix after the USPS change (2026-10-08), sent to Gate 2 again

At the user's instruction (2026-10-08) the article was changed to match the current USPS forwarding page (S1):

| Place | Before | After |
|---|---|---|
| "The 12 months and how it starts" | forwarding "may begin within 3 business days of your request, but it is best to allow up to 2 weeks" | "once your request is approved, you should allow at least 7-10 business days for it to go into effect" (S1: "Once your request is approved, allow at least 7-10 business days for it to go into effect.") |
| "What gets forwarded", first paragraph | periodicals listed among the mail forwarded for free; Marketing Mail "is not forwarded" | periodicals described as forwarded for free for 60 days if fully prepaid by the sender (S1); Marketing Mail "is not forwarded unless the sender has paid forwarding postage" (S1); First-Class Mail, Priority Mail Express, Priority Mail and USPS Ground Advantage still free; Media Mail unchanged |
| "What gets forwarded", second paragraph | "The two USPS pages do not describe periodicals the same way ..." | "The USPS FAQ on forwarding options gives the same 60-day figure for periodicals" (S2 unchanged: "Periodicals for 60 days"); the FAQ's Marketing Mail and Package Services sentence and "This article reports each page's wording as it stands" stay |
| Diagram, card 1 | "Forwarding may begin within 3 business days. USPS says it is best to allow up to 2 weeks." | "Once the request is approved, USPS says to allow at least 7-10 business days to go into effect." |
| Diagram, card 2 | "USPS Marketing Mail is not forwarded." | "USPS Marketing Mail is not forwarded unless the sender paid forwarding postage." |
| Diagram footer | "read Oct. 7, 2026" | "read Oct. 8, 2026" |
| Alt text (front matter and body, 366 characters) | "forwarding may begin within 3 business days; allow up to 2 weeks" | "once approved, allow at least 7-10 business days for it to go into effect" |
| As-of dates | October 7, 2026 | October 8, 2026 (intro and Sources) |

Unchanged and still supported: the 12-month answer in the first sentence, the meta description (144 characters), the temporary-change sentence (S2), the Extended Mail Forwarding section (S3 unchanged), the return-to-sender note, the Hold Mail pointer and its internal link (Hold Mail is published), the "no prices" scope. Front matter and body alt text are identical; the diagram was rendered again (1200x2697) and viewed. **Gate 2: not yet done for the changed parts; sent after the commit.**


## Gate 2 result after the USPS fix (2026-10-08)

**Gate 2: PASS** (ChatGPT, on commit `e323977`, as reported by the user). The changed parts (start timing, periodicals, Marketing Mail, diagram, alt text, as-of dates) were reviewed; no further change requested. Body, diagram and alt text stay as committed.

## Mandatory pre-approval re-check: the 2026-10-08 USPS re-check is used

By the user's decision (2026-10-08), the USPS re-check recorded above ("Mandatory pre-approval re-check (2026-10-08)": S2 and S3 unchanged, S1 changed) counts as the mandatory re-check before the ready-move approval. The article was then fixed to the S1 wording read in that re-check, and the fixed version passed Gate 2. Result for the approval: the article matches the three USPS pages as read on 2026-10-08. Note: the re-check was run before the fix, not after it; no USPS page was re-read between the re-check and the Gate 2 PASS. Still mandatory: a fresh read of the three USPS pages right before Publish (on the user's request).

Ready-move approval has not been given yet.
