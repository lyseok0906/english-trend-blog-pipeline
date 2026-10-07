# QA record — tsa-3-1-1-liquids-rule

Article: `content/published/tsa-3-1-1-liquids-rule.md` (moved from `content/ready/` on 2026-10-07 after publishing)
Sources: `research/sources/tsa-3-1-1-liquids-rule.md` (T1 and T2, read in a real browser on 2026-10-07; the earlier S1–S3 reads used a summarizing tool)
Stage: draft written 2026-10-07; Gate 1 done by Claude on 2026-10-07; Gate 2 (English + SEO, ChatGPT) passed 2026-10-07. Pre-approval TSA re-check done 2026-10-07 (no change). Moved to `content/ready/` on 2026-10-07 after the user's approval. Publishing is a separate step by the user.

Method: the full text of both TSA pages was read in the built-in browser and compared with every claim in the draft. The pages were opened a second time after the draft was written, and the key sentences were tested by script (see the re-check section in the source notes). TSA is the only source used.

## Gate 1 — Factual QA (claim by claim)

Result values: `pass` = matches the recorded source text; `pass (attributed)` = true only as attributed to TSA in the text; `pass (absence)` = a statement that something is not on the page, checked against the full page text.

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | You may bring liquids, aerosols, gels, creams and pastes in your carry-on bag if each container holds 3.4 oz (100 ml) or less and they go in a quart-sized bag | T1 first paragraph | pass (attributed to TSA in the second sentence of the intro and in "What the rule says") |
| C2 | TSA says to pack anything in a larger container in checked baggage | T1: "Pack items that are in containers larger than 3.4 ounces or 100 milliliters in checked baggage." | pass |
| C3 | The wording is as of October 7, 2026 and comes from two TSA pages | Browser read 2026-10-07 | pass |
| C4 | Neither page shows an update date or a notice of change | Full text of T1 and T2 read; no date words, no notice | pass (absence) |
| C5 | TSA says you may bring a quart-sized bag of these items in carry-on "and through the checkpoint" (draft: "in your carry-on bag and through the checkpoint") | T1 | pass |
| C6 | Travel-sized containers of 3.4 oz (100 ml) or less per item | T1 | pass |
| C7 | TSA's FAQ refers to this as the 3-1-1 liquids rule | T2 page title and heading | pass |
| C8 | TSA says placing the items in the small bag and separating it from your carry-on baggage "facilitates the screening process" | T1 (one short direct quote) | pass (attributed) |
| C9 | The page does not say you must take the bag out at every checkpoint | T1 full text: no such instruction | pass (absence) |
| C10 | Any liquid, aerosol, gel, cream or paste that alarms during screening requires additional screening | T1 | pass |
| C11 | The rule page links to three exemptions: medications, infant and child nourishments, inbound international flights | T1 "Exemptions" list | pass |
| C12 | The article covers the last two and not medications | Scope statement | pass (scope) |
| C13 | Formula, breast milk and juice over 3.4 oz (100 ml) are allowed in carry-on baggage and do not need to fit in a quart-sized bag | T2 | pass (attributed) |
| C14 | TSA says to remove these items from the carry-on bag so they are screened separately from the rest of your belongings | T2 | pass (attributed) |
| C15 | Duty-free liquids over 3.4 oz may be carried in a secure, tamper-evident bag if three conditions are true | T1 | pass (attributed) |
| C16 | Condition 1: bought internationally and flying to the United States on a connecting flight | T1 | pass |
| C17 | Condition 2: retailer packed them in a transparent, secure, tamper-evident bag with no sign of tampering | T1 ("do not show signs of tampering when presented to TSA") | pass |
| C18 | Condition 3: original receipt is with the items and the purchase was made within 48 hours | T1 | pass |
| C19 | The items must still be screened and cleared; an item that alarms or cannot be screened is not permitted in the carry-on | T1 | pass (attributed) |
| C20 | TSA recommends packing all liquids over 3.4 oz in checked baggage even if in a tamper-evident bag | T1 ("liquids, gels, and aerosols") | pass (attributed) |
| C21 | Liquids over 3.4 oz not in a secure, tamper-evident bag must be packed in checked baggage | T1 last sentence | pass (attributed) |
| C22 | Out-of-scope list: medications, specific airports, other countries, PreCheck; the article does not track announcements | Scope statement, no factual claim | pass (scope) |
| C23 | "TSA's pages are the place to confirm the current wording before you fly" | Pointer to the primary source, no factual claim about the rule | pass |
| C24 | Source titles and URLs in the Sources section | Page titles and addresses opened in the browser | pass |

### Image (`assets/optimized/tsa-3-1-1-liquids-rule.png`, original SVG in `assets/raw/`)

Own flowchart, no photos, logos or third-party artwork. 800 px wide source, 1200 x 2634 PNG, portrait, text 28 px or larger in the source (30 px or larger except the source line), made for phone reading as with the first article. Checked against the draft:

- "Liquids, aerosols, gels, creams and pastes" → C1.
- "Is the container 3.4 oz (100 ml) or less?" → C6.
- "Yes … Carry-on, in a quart-sized bag" → C1; "TSA: keeping the bag separate from your carry-on baggage helps screening" → C8 (paraphrase, no "must").
- "No … Pack it in checked baggage, unless an exception applies" → C2 and the exemptions.
- "Breast milk, formula, juice … allowed in carry-on … no quart bag needed … removed and screened separately" → C13, C14.
- "Qualifying duty-free liquids … bought internationally, flying to the U.S. on a connecting flight … tamper-evident bag and a receipt dated within 48 hours" → C16–C18 (revised after Gate 2, see below: "Tamper-evident bag, original receipt, and a purchase within 48 hours"). This is a shortened version: the image does not say that the retailer packs the bag or that the bag is transparent. The full conditions are in the article text.
- "Any liquid, aerosol, gel, cream or paste that alarms needs additional screening" → C10 (revised after Gate 2, see below).
- "Source: TSA website, read Oct. 7, 2026" → C3.

Rendered and viewed (current version 1200 x 2763 after the Gate 2 revision); no clipped or overlapping text. The image does not state that the rule is unchanged.

Note on the file in the repo: files written to the connected folder get a provenance (C2PA) block added by the file tool. The SVG is larger than the generated file for that reason (11,832 vs 4,058 bytes). The pixels of the PNG were compared with the generated PNG and are identical.

### Handled by wording

- The brief's risk about whether the traveler must remove the liquids bag is closed: T1 says only that separating the bag "facilitates the screening process", and the article says that and says the page does not state a requirement. It does not add one.
- The article says nothing about whether the rule is new or changed. It says the pages show no update date or change notice.
- The word "exempt" in headings follows TSA's own "Exemptions" list on the rule page.
- The rule page says the duty-free exemption applies to a traveler "traveling to the United States with a connecting flight"; the article uses the same scope and does not extend it to other trips.
- Not repeated from the pages, on purpose: the TSA FAQ statements about ice packs, teethers, baby food and breast milk pumping equipment, and the "medically necessary" wording. They are outside the one question this article answers.

### Not verified (and kept out of the article)

- Whether the rule changed in 2026 or will change. A limited search on 2026-10-06 found no TSA announcement; that is not proof.
- Medication and other medical-liquid rules (the Medications page was not read in full).
- The TSA PreCheck line on the TSA Cares page (not read in context).
- What the name "3-1-1" stands for beyond what TSA's pages state. The article does not explain the name.
- Search volume and competition.

### Re-check before publish approval (mandatory)

Open T1 and T2 in a browser again right before approval. Compare with this record: 3.4 oz / 100 ml, quart-sized bag, the separating sentence, the checked-baggage sentence, the three duty-free conditions, the breast milk, formula and juice sentence. If any wording differs or a date or change notice appears, return the draft for revision. If a TSA page cannot be opened, the article is not published.

### Gate 1 verdict

Pass. No claim in the draft lacks a recorded source. The draft can go to English + SEO QA (ChatGPT, by commit SHA).

## Gate 2 — English + SEO QA

Reviewer: ChatGPT, on commit `6db909d` (article, QA record and diagram). Result received from the user on 2026-10-07: **text and SEO pass; diagram needs two wording changes.**

Passed as written (per the reviewer): title, meta description, first-sentence answer, heading structure; not stating that the bag must be removed at every checkpoint; the portrait diagram is not cut off and explains the exceptions without photos.

Revisions requested and applied (Claude, 2026-10-07):

| # | Finding | Change made |
|---|---|---|
| 1 | The line "Anything that alarms needs additional screening." reads wider than the TSA liquids rule | Diagram bottom line and the matching sentence in the alt text (front matter and body image) changed to "Any liquid, aerosol, gel, cream or paste that alarms needs additional screening." This follows T1: "Any liquid, aerosol, gel, cream or paste that alarms during screening will require additional screening." |
| 2 | "Tamper-evident bag and a receipt dated within 48 hours needed." did not match the TSA conditions closely | Diagram line changed to "Tamper-evident bag, original receipt, and a purchase within 48 hours." This follows T1: "The original receipt for the liquids is present and the purchase was made within 48 hours." |

The article text did not change. The diagram was redrawn (same layout, three lines at the bottom, five lines in the duty-free card; the PNG is now 1200 x 2763). It was viewed after rendering; no clipped or overlapping text. Pixels of the file in the repository were compared with the rendered file.

Per the reviewer's rule, this revised diagram needs only a wording check by the reviewer, not a full review. After that check, Gate 2 counts as passed.

Diagram wording check: done by ChatGPT on commit `df5d08c` (user report, 2026-10-07). Both wording changes are reflected exactly (the "Any liquid, aerosol, gel, cream or paste that alarms needs additional screening." line and the "Tamper-evident bag, original receipt, and a purchase within 48 hours." line); the alt text in the article matches the new bottom line; no clipped or overlapping text.

**Gate 2: PASS (2026-10-07).**

Points the reviewer was given:

- Title is 50 characters ("What Is the TSA 3-1-1 Liquids Rule? What's Exempt?"); the focus keyword is `what is the tsa liquids rule`.
- Meta description is 152 characters (limit 160).
- One short quote only ("facilitates the screening process").

## Pre-approval source re-check (2026-10-07, after Gate 2)

Both TSA pages were opened again in the built-in browser and their text was tested by script against the draft's wording (rule page read in the browser pane; the FAQ page fetched from the same site and parsed).

| Check | Result |
|---|---|
| T1: quart-sized bag sentence; "3.4 ounces (100 milliliters) or less per item"; "separating from your carry-on baggage facilitates the screening process"; checked-baggage sentence; "alarms during screening will require additional screening" | all found, wording unchanged |
| T1: three exemption links (Medications, Infant and child nourishments, Inbound International Flights) | found |
| T1: duty-free conditions (purchased internationally and flying to the U.S. on a connecting flight; transparent, secure, tamper-evident bag packed by the retailer; original receipt and purchase within 48 hours); "must be screened and cleared"; the recommendation to pack liquids over 3.4 oz in checked baggage; last sentence on liquids not in a tamper-evident bag | all found, wording unchanged |
| T1: any instruction to remove or take out the bag | none |
| T2: breast milk, formula and juice over 3.4 oz allowed in carry-on and not needed in a quart-sized bag; remove them to be screened separately | both found, wording unchanged |
| Update date or change notice on either page | none found |

Result: no TSA wording changed since the first read. Method note: the character counts differ slightly from the earlier reads (T1 1,673 vs 1,686; the FAQ was parsed from fetched HTML, so its count is not comparable) because spacing was normalized and the FAQ was read a different way; the tested sentences are what matters and all matched.

Because the user will approve, Claude will read both pages once more immediately before the WordPress publish step if more than a day passes between this check and publishing.

## Gate 3 — Approval to move to ready

Approval: given by the user in chat on 2026-10-07 for this article only ("TSA 글을 `content/ready/`로 옮겨도 좋습니다"). It is not approval of any other article and not approval to publish automatically. The user uploads a WordPress draft, checks the preview and publishes.

Gates passed before the move: Gate 1 (Claude), Gate 2 (ChatGPT, commit `df5d08c`), pre-approval TSA re-check (2026-10-07, no change). Article moved to `content/ready/`, front matter `status: ready`.

### Hand-off for publishing in WordPress (user)

- Title: What Is the TSA 3-1-1 Liquids Rule? What's Exempt?
- Slug (permalink): `tsa-3-1-1-liquids-rule` (stable once published)
- Category: Airport security rules (new category; it does not exist in WordPress yet, create it when you set the category)
- Meta description (152 characters): "TSA lets you carry liquids, gels and aerosols in containers of 3.4 oz (100 ml) or less in a quart-sized bag. See what is exempt and what TSA says to do."
- Focus keyword (Rank Math): what is the tsa liquids rule
- Body: start at the bold first sentence. Do not repeat the `#` title line, because WordPress shows the Title field as the page title.
- Image: upload `assets/optimized/tsa-3-1-1-liquids-rule.png` and use it where the markdown image line is. Alt text: the `image_alt` value in the front matter. Do not also set it as the featured image: the theme shows the featured image above the title and the first article had a duplicate for that reason.
- The Sources section has two links; keep them as written.
- Before pressing Publish: read the preview once on a phone-width screen. If more than a day has passed since 2026-10-07, tell Claude first so it can read both TSA pages again.
- After publishing: send Claude the live URL. Claude then moves the article to `content/published/`, runs the live checks as for the first article, and updates the backlog.

## Live QA (2026-10-07)

Published by the user at https://statesideexplained.com/tsa-3-1-1-liquids-rule/ (WordPress post id 19; the draft was created by Claude through the logged-in browser on 2026-10-07, the user previewed and pressed Publish; published time 2026-10-07 01:08 EDT).
Checked by Claude in the built-in browser, anonymous requests (no login cookies).

| Check | Result |
|---|---|
| HTTP status, canonical URL | 200; canonical equals the live URL |
| Title tag | "What Is the TSA 3-1-1 Liquids Rule? What's Exempt? - Stateside Explained" |
| Meta description | Equals the 152-character text in the front matter (og:description too) |
| robots meta | `index, follow, max-snippet:-1, max-video-preview:-1, max-image-preview:large` |
| Headings | One H1, four H2s plus the Sources H2 (what the rule says, checkpoint, exempt, does not cover, Sources) and two H3s, as in the file |
| Body text | Identical to `content/published/` text: both reduced to lowercase letters and digits give the same 2747 characters and the same SHA-256 (compared programmatically; curly quotes from WordPress texturizing do not count) |
| Lists and links | Numbered list has 3 items; 2 source links, both exactly the TSA URLs in the file; both TSA pages open in the browser and still contain the quoted and checked wording (spot test, 2026-10-07) |
| Diagram | One copy only (no featured image); loads; alt text equals `image_alt`; WordPress scaled the file to 1112x2560 and serves a 667x1536 version in the page |
| Category | "Airport security rules" (new category created for this post); category page lists the post |
| Structured data | Rank Math BlogPosting JSON-LD present; article:section "Airport security rules" |
| Comments | No comment form |
| Home page, feed, sitemap | Home shows both posts; `/feed/` includes the post; `post-sitemap.xml` lists it (lastmod 2026-10-07T05:08:07+00:00); `sitemap_index.xml` 200 |
| Drafts not public | `/about/` and `/privacy-policy/` return 404 anonymously |

Not verified: the exact diagram text size on a real phone (not emulated in this check). The diagram text is 28 px or larger at 800 px width, which is about 12 px on a 343 px wide image column; the user's phone preview before publishing is the check. The `www.` host.

Notes for follow-up (not blocking):

- Byline still shows "admin" (display name not yet set; see the DST record).
- The article date is October 7, 2026, the same day as the as-of date in the text.
- TSA pages should be re-read when the article is revisited; there is no deadline. The article does not track rule changes.
