# QA record — tsa-precheck-what-it-changes

Article: `content/drafts/tsa-precheck-what-it-changes.md`
Brief: `research/briefs/tsa-precheck-what-it-changes.md`. Sources: `research/sources/tsa-precheck-what-it-changes.md` (S1 TSA "TSA PreCheck", S2 TSA "TSA PreCheck FAQ", S3 TSA "How to use TSA PreCheck benefits").
Stage: draft written 2026-10-07; Gate 1 done by Claude on 2026-10-07. Not sent to Gate 2, not approved, not on WordPress, not published.

Method: three TSA pages were opened in the built-in browser on 2026-10-07. The brief had read only S1; S2 and S3 were opened now because S1 alone did not describe how the lane is reached. Their full text was read, and after the draft was written the quoted statements were tested by script against the page text (9 phrases on S1, 15 on S2, 6 on S3): all present. This is the drafting and factual-QA re-check required for rule posts; the re-check right before the user approves moving to `ready` and again right before publishing is still **mandatory**; if a page cannot be opened, do not publish. Prices, offers, location counts and the "99% wait less than 10 minutes" statement on S1 are not used (promotional, changing; the brief's open question 2 had no answer, so the conservative choice was made).

## Gate 1 — Factual QA (claim by claim)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | In TSA's words, PreCheck gives trusted travelers a speedier security experience in dedicated lanes across the U.S. | S1-1 | pass (attributed) |
| C2 | In a PreCheck lane you leave electronics and 3-1-1 liquids in your bag and leave on belts, light jackets and shoes (TSA says) | S1-2 | pass (attributed) |
| C3 | TSA also says no individual is guaranteed expedited screening | S1-3 | pass |
| C4 | Wording as of October 7, 2026; three TSA pages; the article describes the program and does not recommend enrolling | Browser reads; scope | pass |
| C5 | Table: electronics: leave in your bag; liquids in 3-1-1 bags: leave in your bag; belts, light jackets and shoes: leave on | S1-2 | pass (attributed) |
| C6 | Internal link to the published TSA 3-1-1 liquids article (https://statesideexplained.com/tsa-3-1-1-liquids-rule/) | Published article exists (post 19) | pass |
| C7 | TSA's FAQ: if a PreCheck lane is not available, a traveler with a PreCheck boarding pass may be able to keep 3-1-1 liquids and laptops in the bag and shoes and light jackets on in the standard lane; eligible passengers should check with the TSA officer on duty | S2-7 | pass (attributed) |
| C8 | TSA says it uses unpredictable security measures, both seen and unseen; all travelers will be screened; no individual is guaranteed expedited screening; the FAQ answers "no" to whether an eligible traveler is guaranteed | S1-3, S2-8 | pass (attributed) |
| C9 | PreCheck benefits are not automatic; the KTN goes in the KTN field of the airline reservation; the name must match the enrollment name and the date of birth must be correct | S3-1, S3-2 | pass (attributed) |
| C10 | The PreCheck indicator must be displayed on the boarding pass before a traveler can use the lane | S2-2 | pass (attributed) |
| C11 | Showing a Global Entry, NEXUS or SENTRI card or a PreCheck approval notification does not give access to the lane | S2-1 | pass (attributed) |
| C12 | Global Entry, NEXUS and SENTRI members use their PASS ID as the KTN, and it still has to be in the airline reservation | S3-3, S2-1 | pass (attributed) |
| C13 | Children 17 and under can join an adult in the PreCheck lane; the FAQ gives conditions | S1-5, S2-4 | pass (attributed) |
| C14 | Anyone 18 and older needs their own KTN; children 12 and under can join an adult and the indicator does not have to be on their own boarding pass; children 13 to 17 only when the indicator appears on their own boarding pass, which requires the same reservation as an adult whose boarding pass has it | S2-4, S2-5 | pass (attributed) |
| C15 | A parent who escorts a child through security with a gate pass is directed to standard screening | S2-6 | pass (attributed) |
| C16 | PreCheck memberships last five years | S2-3 | pass (attributed) |
| C17 | TSA has three authorized enrollment providers: CLEAR, IDEMIA and Telos | S1-6 | pass (attributed) |
| C18 | Scope: no prices, offers, enrollment steps, eligibility, worth-it judgment, comparisons, Touchless ID, flights to other countries, standard-lane rules for those without PreCheck | Scope statement | pass (scope) |
| C19 | Sources: all three checked October 7, 2026; none shows an update date | Browser reads | pass |
| C20 | Source titles and URLs | Page titles: "TSA PreCheck", "TSA PreCheck FAQ", "How to use TSA PreCheck benefits" | pass |

### Image (`assets/optimized/tsa-precheck-what-it-changes.png`, original SVG in `assets/raw/`)

- Own three-step card diagram, no photos, no provider logos, no boarding pass or PreCheck mark. 1200x1947. Every line traces to the claims above: "Known Traveler Number in the airline reservation. The PreCheck indicator must show on the boarding pass. It is not automatic." (C9, C10); "In a PreCheck lane, TSA says: stays in your bag: electronics and 3-1-1 liquids; stays on you: belts, light jackets and shoes" (C2, C5); "No guarantee (TSA): All travelers will be screened. No individual is guaranteed expedited screening." (C8); "Source: TSA pages, read Oct. 7, 2026" (C19).
- Alt text in the front matter and the body is identical (465 characters).
- File check on the device: pixel hash of the PNG matches the cloud render (md5 of RGB bytes fd4adaa1...). Visual check of the render: no text overflow (a first render had one line overflowing the first card; the card was made taller and re-rendered).

### Handled by wording

- Every program statement is attributed to TSA with "TSA says", in TSA's words where quoted; the one direct quotation is a short phrase from S1 in the lead.
- The shoes statement is attributed to the PreCheck page only; the standard lane without PreCheck is not described (the TSA/DHS shoe-policy release of July 8, 2025 was not opened and is not used).
- No prices, offers, wait-time statistic or sign-up steps; no recommendation.

### Not verified

- The FAQ sections not read (applying, renewal, enrollment providers, military, medical conditions), including who is eligible; the article does not describe them.
- The "participating airlines" list (TSA's airports and airlines map was not opened); the article does not claim every airline takes part.
- Whether the shoes statement on the PreCheck page matches current standard-lane practice (see above; not described).
- Search volume and competition for the focus keyword (not measured; promotional pages dominate).
- The exact diagram text size on a real phone (to be checked in the WordPress preview).

### Re-check obligations

**Mandatory**: re-read S1, S2 and S3 right before the user approves moving the article to `ready`, and again right before publishing. Compare the benefits sentence, the "not guaranteed" caveat, the indicator and KTN wording, the children's conditions, the five-year statement and the provider names. If a page differs or cannot be opened, return to draft or do not publish.

## Gate 2 (ChatGPT, 2026-10-07, result reported by the user)

**FIX REQUIRED, applied.**

| Change | Before | After |
|---|---|---|
| Bold first sentence | "TSA PreCheck is a TSA program that, in TSA's words, gives trusted travelers a speedier security experience in dedicated lanes across the U.S." | "TSA PreCheck is a TSA program that offers eligible travelers a speedier security experience in dedicated lanes across the U.S." |
| Diagram, step 2 label | "Stays on you:" | "You can keep on:" |
| Alt text (front matter and body, identical, 469 characters) | "belts, light jackets and shoes stay on you" | "you can keep belts, light jackets and shoes on" |

Claim check: the new first sentence is a paraphrase of S1-1 ("gives trusted travelers a speedier security experience in dedicated lanes across the U.S."); "eligible travelers" follows TSA's use of "PreCheck eligible" in the FAQ (S2-8) and drops the quotation attribution, which the next sentence ("TSA says ...") carries. "You can keep on" matches TSA's "leave on belts, light jackets, and shoes" (S1). The diagram was re-rendered (1200x1947, no text overflow; pixel hash md5 of RGB e91371ac...); the PNG and SVG on the device match the cloud render. Result: pass.

Not sent back to Gate 2 yet. For the changed articles, ChatGPT will re-review the fix commit.
