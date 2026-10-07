# QA record — forever-stamp-how-it-works

Article: `content/drafts/forever-stamp-how-it-works.md`
Sources: `research/sources/forever-stamp-how-it-works.md` (S1–S4, section "Re-read in a real browser (2026-10-07)")
Stage: draft written 2026-10-07; Gate 1 done by Claude on 2026-10-07; Gate 2 (English + SEO, ChatGPT) not yet done.

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
| C13 | USPS's international page describes a separate stamp, the Global Forever, for sending 1-ounce letters or postcards to other countries | S4: "Send 1 oz letters or postcards around the world with one Global Forever® stamp". "Separate" rests on the page naming it a different stamp ("Global Forever stamp available") and S2 calling the flag Forever domestic. S4 does not use the word "separate" | pass (attributed; see note below) |
| C14 | USPS says the Global Forever never expires, even if the postage price goes up | S4 | pass (attributed) |
| C15 | First-Class Mail International reaches more than 180 countries | S4 | pass (attributed) |
| C16 | The USPS pages used here do not say whether a regular Forever stamp can be used on international mail | S2 and S4 full text searched for "Forever": no such statement | pass (absence) |
| C17 | Scope paragraph (no prices, where to buy, designs, postcard rates, packages; prices change; current price is on USPS's pages) | Scope statement, no factual claim about the rule | pass (scope) |
| C18 | Source titles and URLs | S1 page title "2007 - First Forever stamps issued - U.S. Postal Facts", H1 "2007 – First Forever stamps issued"; S2 "U.S. Flag 2026 Stamps"; S3 "Notice 123" ("Price List"); S4 "First-Class Mail International" | pass |

Note on C13: "separate stamp" is Claude's reading of USPS's wording, not a USPS word. If ChatGPT or the user wants the claim closer to the page, change "a separate stamp, the Global Forever" to "the Global Forever stamp". Not changed yet.

### Image (`assets/optimized/forever-stamp-how-it-works.png`, original SVG in `assets/raw/`)

- Own flowchart, no photos, no stamp artwork, no USPS logo (brief rule). 1200x2280.
- Every sentence in the diagram traces to C1, C7, C8, C11, C13: "always valid for the First-Class Mail 1 oz rate, even if postage rates increase"; "The stamp pays the 1 oz rate"; "USPS: for letters and cards sent within the U.S."; "USPS price list: letters up to 2 oz and 3 oz cost more than letters up to 1 oz"; "USPS describes a separate stamp for it, called the Global Forever."
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

Not yet done. To be sent to ChatGPT by commit SHA with the article path and this QA path.
