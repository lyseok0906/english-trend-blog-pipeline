# QA record — forever-stamp-how-it-works

Article: `content/ready/forever-stamp-how-it-works.md` (moved from `content/drafts/` on 2026-10-07)
Sources: `research/sources/forever-stamp-how-it-works.md` (S1–S4, section "Re-read in a real browser (2026-10-07)")
Stage: draft written 2026-10-07; Gate 1 done by Claude on 2026-10-07; Gate 2 (English + SEO, ChatGPT) passed 2026-10-07 after three wording fixes. Pre-approval USPS re-check done 2026-10-07 (no change). Moved to `content/ready/` 2026-10-07 after the user's approval. Publishing is a separate step by the user.

Method: all four USPS pages were read in the built-in browser on 2026-10-07. The quoted sentences and the page titles were tested again by script after the draft was written (S2 and S1). USPS is the only source used. No price number is in the article text (brief rule).

## Gate 1 — Factual QA (claim by claim)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | USPS says a Forever stamp is "always valid for the First-Class Mail 1 oz rate, even if postage rates increase" (quote, 14 words) | S2: "Value: Always valid for the First-Class Mail 1 oz rate, even if postage rates increase." Only the capital A differs, because the quote starts mid-sentence | pass (attributed) |
| C2 | USPS describes it as a stamp for domestic mail weighing up to 1 ounce | S2: "A Forever® stamp is for sending domestic mail weighing up to 1 oz via First-Class Mail®." | pass (attributed) |
| C3 | The wording is as of October 7, 2026 and comes from four USPS pages | Browser reads 2026-10-07 | pass |
| C4 | None of the four pages shows an update date; the price list shows its effective date, October 4, 2026 | S3 header "Notice 123 • Effective October 04, 2026". S2 shows a stamp issue date (6/9/2026), which is not a page update date; S1 shows a modified date only in page metadata, not on the page; S4 shows none | pass (absence, wording limited to dates the pages show) |
| C5 | "In other words, USPS says the stamp keeps its value for the 1-ounce rate when that rate changes" | Paraphrase of S2 value sentence | pass |
| C6 | The first Forever stamp was issued on April 12, 2007 | S1 visible text: "issued April 12, 2007, at Philadelphia's Independence Hall" | pass |
| C7 | A Forever stamp is for domestic mail up to 1 oz via First-Class Mail | S2 | pass (attributed) |
| C8 | Purpose: letters and cards up to 1 ounce within the U.S., including U.S. territories and military bases overseas | S2 "Purpose" line | pass (attributed) |
| C9 | 1 ounce is approximately 4 sheets of regular 8-1/2" x 11" paper in a rectangular envelope | S2 "Purpose" line | pass (attributed: "the same page says") |
| C10 | A Forever stamp is for mail up to 1 ounce | S2 | pass |
| C11 | USPS's price list charges more for heavier letters: a stamped letter up to 2 oz and one up to 3 oz each cost more than one up to 1 oz | S3 Retail—Single Piece, Letters (Stamped): 1 oz, 2 oz and 3 oz rows, each higher than the last. Numbers not given in the text | pass |
| C12 | USPS's store page describes a Forever stamp as being for domestic mail | S2 | pass (attributed) |
| C13 | USPS's international page describes the Global Forever stamp for sending 1-ounce letters or postcards to other countries | S4: "Send 1 oz letters or postcards around the world with one Global Forever® stamp". After Gate 2 the draft no longer says "separate", which S4 does not use | pass (attributed) |
| C14 | USPS says the Global Forever never expires, even if the postage price goes up | S4 | pass (attributed) |
| C15 | First-Class Mail International reaches more than 180 countries | S4 | pass (attributed) |
| C16 | The USPS pages used here do not say whether a regular Forever stamp can be used on international mail | S2 and S4 full text searched for "Forever": no such statement | pass (absence) |
| C17 | Scope paragraph (no prices, where to buy, designs, postcard rates, packages; prices change; current price is on USPS's pages) | Scope statement, no factual claim about the rule | pass (scope) |
| C18 | Source titles and URLs | S1 page title "2007 - First Forever stamps issued - U.S. Postal Facts", H1 "2007 – First Forever stamps issued"; S2 "U.S. Flag 2026 Stamps"; S3 "Notice 123" ("Price List"); S4 "First-Class Mail International" | pass |

Note on C13: Gate 2 asked to drop "separate" (USPS does not use the word). Fixed in the article, the diagram and the alt text; see Gate 2.

### Image (`assets/optimized/forever-stamp-how-it-works.png`, original SVG in `assets/raw/`)

- Own flowchart, no photos, no stamp artwork, no USPS logo (brief rule). 1200x2280.
- Every sentence in the diagram traces to C1, C7, C8, C11, C13: "always valid for the First-Class Mail 1 oz rate, even if postage rates increase"; "The stamp pays the 1 oz rate"; "USPS: for letters and cards sent within the U.S."; "USPS price list: letters up to 2 oz and 3 oz cost more than letters up to 1 oz"; "USPS describes the Global Forever stamp for international mail."
- Source line: "Source: USPS websites, read Oct. 7, 2026".
- Alt text in the front matter describes the diagram's content and does not repeat the keyword.
- File check on the device: pixel hash matches the cloud render.

### Handled by wording

- No price number anywhere (brief rule); the price list is described only as "higher".
- No instruction on how to add postage (not verified; stated in the article as out of scope).
- Costco and retailers, postcard rates and stamp designs are out of scope and not mentioned except in the scope list.

### Not verified

- Whether a regular Forever stamp works on international mail (no official page read says so; the article says it does not say).
- Whether a Forever stamp works on postcards (the article does not claim it).
- Search volume and competition for the focus keyword.
- FAQ pages on faq.usps.com (404 or empty earlier); not needed for any claim.

### Re-check obligations

Mandatory re-check of S1–S4 right before the user approves moving the article to `ready` (brief rule). If any page differs, return to draft.

## Gate 2 — English + SEO QA

ChatGPT reviewed commit `e0aee2b` on 2026-10-07. Title kept as is (57 characters, shows search intent and the limit). Body, meta description, structure and diagram readability passed. One fix was requested, in three places, because USPS does not use the word "separate":

1. Body: "a separate stamp, the Global Forever" became "the Global Forever stamp".
2. Diagram: "USPS describes a separate stamp for it, called the Global Forever." became "USPS describes the Global Forever stamp for international mail." (the new PNG was checked on the device by pixel hash; the first write came through stale, so it was re-written and checked again).
3. Alt text: "a separate stamp called the Global Forever" became "the Global Forever stamp".

ChatGPT said Gate 2 counts as PASS once these three changes are made. Done in the commit that follows `e0aee2b`. The word "separate" no longer appears in the article, the diagram or the alt text.

Result: **PASS** (2026-10-07). Next: mandatory USPS re-check right before the user approves moving the article to `ready` (done below).

## Pre-approval USPS re-check (2026-10-07)

All four USPS pages were opened again in the built-in browser and the draft's quoted and paraphrased wording was tested by script (details in the source notes, section "Re-check before approval"). No difference: S1 April 12, 2007; S2 validity, domestic, 1 oz, territories and "approximately 4 sheets" wording; S3 effective October 4, 2026 and rising stamped-letter rows, no "Forever" line; S4 Global Forever wording, 180 countries, no statement about a regular Forever stamp. Result: unchanged, article may move to `ready`.

## Gate 3 — Approval

The user approved moving this article to `content/ready/` on 2026-10-07, on condition that Claude re-checks the USPS pages first and the content is the same. It was. Order set by the user: publish the TSA article first, run live QA on it, then Claude uploads this article to WordPress as a draft and the user previews and publishes it.

## WordPress hand-off (for the upload step)

Title, slug, category (new category "Postal service and stamps" to be created), meta description and focus keyword are in the front matter. Body starts at the bold sentence (the title is the post title). Upload the PNG with the `image_alt` text and do not also set it as the featured image. Preview on phone width before publishing. If more than a day passes before publishing, tell Claude so the USPS pages are re-read. After publishing, send the live URL for live QA.

## WordPress draft (2026-10-07)

Claude created the draft through the logged-in browser after the TSA article went live and passed live QA: post id 22, status draft, slug `forever-stamp-how-it-works`, new category "Postal service and stamps", diagram uploaded (1200x2280, not scaled; file hash matches the repository PNG) with the `image_alt` text, Rank Math meta description (125 characters, equals the front matter) and focus keyword set, comments closed, no featured image. Body text checked against `content/ready/forever-stamp-how-it-works.md` (lowercase letters and digits, same 2254 characters and same SHA-256). Four USPS source links present. The draft returns 404 to anonymous visitors, as it should.

Remaining: the user previews on a phone width and publishes (Publish is the user's step). If more than a day passes before publishing, tell Claude so the four USPS pages are re-read. After publishing, send the live URL for live QA, then Claude moves the article to `content/published/`.
