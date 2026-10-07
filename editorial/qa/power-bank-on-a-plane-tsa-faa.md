# QA record — power-bank-on-a-plane-tsa-faa

Article: `content/ready/power-bank-on-a-plane-tsa-faa.md` (moved from `content/drafts/` on 2026-10-07)
Brief: `research/briefs/power-bank-on-a-plane-tsa-faa.md`. Sources: `research/sources/power-bank-on-a-plane-tsa-faa.md` (S1 TSA Power Banks, S2 TSA batteries over 100 Wh, S3 FAA PackSafe batteries).
Stage: draft written 2026-10-07; Gate 1 done by Claude on 2026-10-07. Gate 2 (English + SEO, ChatGPT): PASS on commit `2edbc32`, 2026-10-07, no changes. Not approved, not on WordPress, not published.

Method: all three pages were opened in the built-in browser on 2026-10-07, once for the source notes and again after the draft was written. After the draft, 6 phrases (S1), 6 phrases (S2) and 17 phrases (S3), including every number, were tested by script against each page's text: all true. This second read is the drafting and factual-QA re-check required for airport-rule posts. The re-check right before the user approves publishing is still **mandatory**; if a page cannot be opened, do not publish.

## Gate 1 — Factual QA (claim by claim)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | TSA says power banks are not allowed in checked luggage; "Yes, but only in a carry-on bag" | S1-1, S1-2 (header "Carry On Bags: Yes", "Checked Bags: No") | pass |
| C2 | The FAA limits a spare battery or power bank to 100 Wh per battery | S3-1 | pass (attributed) |
| C3 | The FAA says larger batteries of 101 to 160 Wh need airline approval | S3-2 | pass (attributed) |
| C4 | The wording is as of October 7, 2026 and comes from three pages | Browser reads 2026-10-07 | pass |
| C5 | TSA says portable chargers and power banks containing a lithium ion battery must be packed in carry-on bags | S1-1 | pass (attributed) |
| C6 | TSA adds that spare lithium batteries, which include both power banks and phone chargers, are prohibited in checked luggage | S1-2 | pass (attributed) |
| C7 | The FAA's table agrees: carry-on yes, checked bags no; the battery must be protected from damage and short circuit | S3-1 (row "Spare Battery or Power Bank": YES / NO; "Must be carry-on only and protected from damage and short circuit") | pass |
| C8 | With airline approval a passenger may also carry up to two spare larger lithium-ion batteries of 101 to 160 Wh | S3-1/S3-2 | pass (attributed) |
| C9 | TSA's page on batteries over 100 Wh says the same thing, and says the limit is two of those larger batteries per person | S2-2 ("With airline approval ... up to two spare larger lithium ion batteries (101–160 Wh)"; "limit of two spare batteries per person") | pass (attributed) |
| C10 | Table: up to 100 Wh allowed in carry-on; 101 to 160 Wh needs airline approval, two spare batteries per person at most; over 160 Wh forbidden | S3-1, S3-2: "0-100 Wh are allowed on passenger aircraft ... 101-160 Wh require approval from the air carrier ... exceeding 160 Wh are forbidden"; two per person | pass (attributed in the column header "What the FAA says") |
| C11 | The FAQ says there is no limit on the number of rechargeable batteries under 100 Wh carried for personal use; batteries carried for sale or distribution are prohibited | S3-3. The wording "under 100 Wh" is kept exactly; no claim for exactly 100 Wh | pass (attributed) |
| C12 | The FAA says a battery's Wh should be marked on the battery; if not, multiply volts by amp hours | S3-4 | pass (attributed) |
| C13 | For mAh, divide by 1000 to get amp hours first, then multiply by the volts | S3-4 | pass (attributed) |
| C14 | The FAA's example is a 12-volt battery rated at 8 Ah, which is 96 Wh (12 x 8 = 96) | S3-4 | pass |
| C15 | The FAA says TSA, individual airline and international rules may at times be more restrictive than its own | S3-5 ("Transportation Security Administration (TSA) security, individual airline, and international rules may, at times, be more restrictive") | pass (attributed) |
| C16 | It adds that many airlines may have stricter limits on how many power banks a passenger can carry, regardless of Wh capacity, and tells passengers to check with their airline before traveling | S3-5 | pass (attributed) |
| C17 | At the checkpoint, TSA says the final decision rests with the TSA officer on whether an item is allowed through | S1-3 | pass (attributed) |
| C18 | The FAA says damaged or recalled batteries must not be carried aboard an aircraft unless the battery has been removed or otherwise made safe | S3-6 | pass (attributed). The FAA's full sentence also says "likely to create sparks or generate a dangerous evolution of heat"; the draft shortens it without changing the meaning |
| C19 | Scope paragraph (no in-flight use, airline policy, international, other battery types, wheelchairs, product recommendations; link to the TSA 3-1-1 article; no tracking of changes) | Scope statement; the link target is the published article at https://statesideexplained.com/tsa-3-1-1-liquids-rule/ | pass (scope; link target exists) |
| C20 | Sources: all three checked October 7, 2026; page dates May 14, 2025; March 29, 2023; October 2, 2026 | Visible "Last Updated on" lines on each page, tested by script | pass |
| C21 | Source titles and URLs | TSA page titles "Power Banks" and "Lithium batteries with more than 100 watt hours"; FAA page title "Airline Passengers and Batteries" (site PackSafe section) | pass |

### Image (`assets/optimized/power-bank-on-a-plane-tsa-faa.png`, original SVG in `assets/raw/`)

- Own decision diagram, no photos, no battery art, no agency or airline logos. 1200x2367.
- Every sentence traces to the claims above: "A spare lithium battery or power bank"; "Carry-on bag only; TSA: spare lithium batteries are prohibited in checked luggage" (C1, C6); "100 Wh or less: Allowed in carry-on (FAA)" (C10); "101–160 Wh: Airline approval needed. Two spare batteries at most (FAA)" (C8, C10); "Over 160 Wh: Forbidden (FAA)" (C10); "No Wh on the label? FAA: volts x amp hours = Wh. For mAh, divide by 1000 first. FAA example: 12 V x 8 Ah = 96 Wh" (C12–C14); "Your airline may set stricter limits" (C15, C16). Source line: "Source: TSA and FAA websites, read Oct. 7, 2026".
- Alt text in the front matter and the body is identical and describes the diagram's content without repeating the keyword.
- File check on the device: pixel hash of the PNG matches the cloud render (md5 of RGB bytes 674e4d6e...); the SVG on the device contains the diagram title text. Visual check of the render: no text overflow.

### Handled by wording

- Each number is attributed to the agency whose page states it. TSA's "Power Banks" page does not state the 100 Wh number, so the 100 Wh limit is attributed to the FAA, and TSA's over-100 Wh page is cited only for the 101–160 Wh, two-battery rule.
- The FAA's table says "100 Wh per battery" and its FAQ says "under 100 Wh" for the no-limit sentence; the article states the table limit and the FAQ sentence separately, and makes no claim about the number of batteries at exactly 100 Wh.
- No in-flight rule, no airline-specific rule, no safety advice of Claude's own, and no statement about how likely battery fires are.
- No product or brand names.

### Not verified

- Any airline's own power-bank rules (not researched; the article says airlines may be stricter, as the FAA does).
- Search volume and competition for the focus keyword (not measured; see the brief).
- The exact diagram text size on a real phone (to be checked in the WordPress preview).

### Re-check obligations

**Mandatory**: re-read S1, S2 and S3 right before the user approves moving the article to `ready` and again right before publishing. Compare the numbers (100, 101–160, 160, two per person), the carry-on-only wording and the "Last updated" dates. If a page differs or cannot be opened, return to draft or do not publish.

## Gate 2 — English + SEO QA

ChatGPT reviewed commit `2edbc32` on 2026-10-07 (this article's draft is in that commit unchanged from the one recorded under Gate 1). Result: **PASS**, no changes requested. The article stays in `content/drafts/` and is not changed by Gate 2.

Next: Mandatory re-check of the three TSA/FAA pages right before the user approves the move to `ready`, and again right before publishing. Moving to `ready` needs the user's approval for this article alone. Not on WordPress, not published.

## Pre-approval source re-check (2026-10-07, mandatory)

Done by Claude after Gate 2 passed and before asking the user to approve the move to `ready`. All three pages were opened again in the built-in browser and the same phrases as in Gate 1 were tested against the page text: 6 phrases on TSA "Power Banks", 6 on TSA "Lithium batteries with more than 100 watt hours", 17 on the FAA "Airline Passengers and Batteries" page (every number: 100 Wh, 101-160 Wh, 160 Wh, two spare batteries per person, 12 V x 8 Ah = 96 Wh, the carry-on-only rows, the airline caveat and the damaged-or-recalled sentence). All 29 are present, unchanged. The page dates are unchanged: TSA "Last Updated on May 14, 2025", TSA "Last Updated on March 29, 2023", FAA "Last updated: Friday, October 2, 2026". The FAA table row "Spare Battery or Power Bank" is still present.

Result: **no difference**; the draft needs no change. The draft text on the device is the text Gate 2 reviewed (commit `2edbc32`). The user's approval to move this article to `ready` is requested separately; until then the article stays in `content/drafts/`. The mandatory re-check is repeated right before the user publishes, and again if more than a day passes after this one.

## Gate 3 — Approval

The user approved moving this article to `content/ready/` on 2026-10-07, after Gate 2 PASS and the mandatory source re-check above (no difference). The approval covers this article only. Front matter set to `status: ready`. Publishing is a separate step by the user: next, once the user asks, Claude uploads the article to WordPress as a draft (title, slug, category "Airport security rules", diagram with alt text, Rank Math meta description and focus keyword), and the user previews on phone width and presses Publish.

**Mandatory**: re-read the three TSA/FAA pages again right before the user presses Publish (and again before the WordPress upload if more than a day has passed since the re-check above). If a page differs or cannot be opened, do not publish.

