# QA record — tsa-holiday-food-carry-on

Article: `content/drafts/tsa-holiday-food-carry-on.md` (draft, 2026-11-04, about 1,375 words in the body, one H1, seven H2 sections including Sources).
Brief: `research/briefs/tsa-thanksgiving-food-carry-on.md` (backlog row 8; the slug changed from `tsa-thanksgiving-food-carry-on` to `tsa-holiday-food-carry-on` because the article is framed as holiday food, as the user's scope approval of 2026-11-04 asked). Sources: `research/sources/tsa-thanksgiving-food-carry-on.md`.
Stage: draft. Gate 1 (Claude) run on 2026-11-04. Gate 2 not run. **Not for publication until a TSA 2026 Thanksgiving notice that contains food guidance has been read, compared with this draft and the draft revised and re-reviewed (user rule, 2026-11-04).** Not in `content/ready/`, not uploaded to WordPress.

## Scope as approved by the user (2026-11-04)

- Holiday-food framing. The 2025 local release is always labeled with its year and region (Harrisburg International Airport, Nov. 24, 2025) in the lead, body, table, diagram and alt.
- The Food page and the local release are kept apart by source; the "Where the two TSA sources differ" section shows the differences and does not merge them or decide which applies (C20 to C24).
- No search volume or Trends figure appears in the article (Trends stay relative and are only in the source notes).
- No airline rules, import rules, alcohol, food safety or packing advice (stated in the article).

## Method

After drafting, the TSA pages were opened in the built-in browser on 2026-11-04 and every statement was tested by script:

- Food page: all six list pages fetched (59 rows, "Total: 59 items"), every row used in the table matched for name, carry-on value and checked value; searches for cranberry, stuffing, casserole, turkey and mashed returned no rows; the footer sentence "The final decision rests with the TSA officer on whether an item is allowed through the checkpoint." matched.
- Harrisburg release (`.../2025/11/24/tsa-prepared-for-busy-thanksgiving-travel-harrisburg-offers-special`): title, dateline ("Monday, November 24, 2025", "HARRISBURG, P.A."), all example lists and the quoted fragment "as it is spreadable" matched. Four strings failed a first strict test only because of wording and punctuation: the page dates the release "Monday, November 24, 2025" (not the abbreviated form tested), writes "spill, spread, spray, pump, or pour" and "(frozen, cooked, or uncooked)" with a serial comma, and writes "jar/can". The article paraphrases these without quotation marks, and the page text was read in context to confirm the meaning.
- National release of Nov. 21, 2025: date and title matched; no occurrence of turkey, pie, stuffing, cranberry, gravy, casserole or food.
- Press-release list: newest item Oct 28 2026; no item mentions Thanksgiving.

## Gate 1 — Factual QA (claim by claim)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | Lead: the Food page lists pies, cakes, cookies and cooked meat as Yes in carry-on and checked bags | Food page | pass |
| C2 | Lead: the page limits gravy, jam, maple syrup and sauces to 3.4 ounces in a carry-on ("Yes (Less than or equal to 3.4oz/100 ml allowed)") | Food page | pass |
| C3 | Lead: a TSA local release from Harrisburg International Airport, dated Nov. 24, 2025, gives a holiday list and says to pack gravy, cranberry sauce, jams and maple syrup in checked bags | Release | pass |
| C4 | Both sources read on Nov. 4, 2026; the Food page shows no date | Reads | pass |
| C5 | On Nov. 4, 2026 TSA's press-release list showed no 2026 Thanksgiving release and the newest item was Oct. 28, 2026 | List | pass |
| C6 | The Food page lists 59 items, each with a carry-on and a checked value | Food page | pass |
| C7 | No item is named cranberry sauce, stuffing, casserole or turkey | Food page (search of all 59 rows) | pass (absence check) |
| C8 | Table: Pies and Cakes, Cookies, Cooked Meat Seafood and Vegetable (No Liquid), Bread, Candy and Spices (dry): Yes / Yes | Food page | pass |
| C9 | Table: Fresh Fruits and Vegetables, Fresh Meat and Seafood, Frozen Food, Canned Foods: "Yes (Special Instructions)" / Yes | Food page | pass |
| C10 | Table: Gravy, Jam and Jelly, Maple Syrup, Salsa and Sauces, Soups: "Yes (Less than or equal to 3.4oz/100 ml allowed)" / Yes | Food page | pass |
| C11 | Several rows say solid food items (not liquids or gels) can be transported in carry-on or checked bags | Food page (Bread, Candy, Spices, Solid Foods) | pass |
| C12 | The Fresh Fruits and Vegetables row limits this to the continental United States and says passengers flying from Hawaii, Puerto Rico or the U.S. Virgin Islands to the mainland cannot take most fresh fruits and vegetables | Food page | pass |
| C13 | Fresh meat and frozen food: ice or ice packs must be completely frozen; partially melted ice or ice packs with liquid at the bottom are not permitted | Food page | pass |
| C14 | Canned foods: could require additional screening that might result in the item not being allowed through; TSA suggests a checked bag, shipping or leaving it at home | Food page | pass |
| C15 | Release: titled "TSA prepared for busy Thanksgiving travel in Harrisburg, offers special packing tips"; published Nov. 24, 2025; TSA at Harrisburg International Airport (MDT) | Release | pass |
| C16 | Release: most foods can be carried through a checkpoint, some items must be in checked baggage; items that can spill, spread, spray, pump or pour and are larger than 3.4 ounces go in checked luggage | Release | pass |
| C17 | Release carry-through examples: baked goods (homemade or store-bought pies, cakes, cookies, brownies, sweet treats); meats (turkey, chicken, ham, steak; frozen, cooked or uncooked); stuffing (cooked or uncooked, box or bag); solid casseroles (carry-on or checked); mac and cheese (solid, cooked in a pan, or ingredients); fresh vegetables; fresh fruit (cranberries among the examples); candy; spices | Release | pass |
| C18 | Release: casseroles with liquid or semi-liquid components (soups, sauces, gravy) must comply with the 3-1-1 liquids rule | Release | pass |
| C19 | Release checked-bag examples: cranberry sauce (homemade or canned, "as it is spreadable"); gravy (homemade or in a jar/can); canned fruits or vegetables in liquid-filled cans or jars; preserves, jams and jellies (spreadable items must be checked); maple syrup. Ice packs permitted if frozen solid | Release | pass |
| C20 | Differences table: gravy, jam and jelly, maple syrup (Food page carry-on up to 3.4 oz and checked Yes; release lists them for checked bags) | Food page; release | pass |
| C21 | Cranberry sauce: no Food-page row; release names it for checked bags | Food page; release | pass |
| C22 | "Both sources point to checked bags for larger amounts"; the Food page also shows the 3.4-ounce carry-on allowance and the release's list does not mention one | Food page; release | pass (the release's general rule names items larger than 3.4 ounces; the lists for gravy, jams and maple syrup carry no size) |
| C23 | The release names items the Food page has no row for (turkey, stuffing, casseroles, mac and cheese); the article does not match them to rows (Cooked Meat (No Liquid) Yes/Yes; Soups up to 3.4 oz) | Food page; release | pass |
| C24 | The article does not decide which wording applies to a particular trip | Draft statement | pass |
| C25 | Food page footer: the final decision rests with the TSA officer on whether an item is allowed through the checkpoint | Food page | pass |
| C26 | Pies and cakes and cookies rows: TSA officers may instruct travelers to separate items such as foods and powders from carry-on bags so they do not obstruct clear X-ray images | Food page | pass |
| C27 | Other TSA airports published local releases with similar titles on Nov. 24 and 25, 2025; only Harrisburg was read; not compared | Source notes (list read 2026-11-04, at least ten releases; Miami's title differs) | pass |
| C28 | National release of Nov. 21, 2025 gave general holiday travel tips and had no food examples | National release | pass (absence check) |
| C29 | 2026: no Thanksgiving release in the list; if TSA publishes one its examples may differ | List | pass (conditional statement) |
| C30 | Link to the published 3-1-1 article (`/tsa-3-1-1-liquids-rule/`) with its exact title | Live post (title recorded in the source notes) | pass |
| C31 | Sources: four TSA URLs, each opened on 2026-11-04 | Reads | pass |

Result: 31 of 31 claims pass as attributed statements, stated limits or absence checks.

## Open points reported

- **P1 — 2026 notice (blocks publication).** The user's rule: not published until a TSA 2026 Thanksgiving notice that contains food guidance has been read. Not yet issued as of 2026-11-04. Past timing: Nov. 24 and 25 in 2025 (local), Nov. 19 to 21 in 2024; an estimate, not a TSA statement. When it appears: compare each example with the draft, rewrite the section "What TSA had published for the 2026 holiday" (or remove it), re-test every statement, update diagram footer and alt if the footer line changes, and run Gate 2.
- **P2 — Which wording applies.** The Food page and the release word gravy, jam and jelly and maple syrup differently; the article reports both and does not decide (as the user asked).
- **P3 — Only Harrisburg read.** Other airports' releases of Nov. 24 and 25, 2025 were not compared; the article says so.
- **P4 — Focus keyword.** `can you bring holiday food through tsa` is Claude's choice for the new framing; it is not a measured search term (Trends for exact food phrases were near zero, relative values only, source notes). Needs the user's or Gate 2's view.
- **P5 — Release dateline.** The release's dateline reads "HARRISBURG, P.A."; the article and diagram say "Harrisburg International Airport" and do not add a state name.
- **P6 — Dates on the Food page.** The page shows no update date; the article says so.

## Image and alt text

| # | Check | Result |
|---|---|---|
| I1 | Diagram cards compared with the body and the sources: card "TSA Food page" (carry-on and checked: pies, cakes, cookies, cooked meat; carry-on up to 3.4 oz (100 ml): gravy, jam and jelly, maple syrup, sauces, soups; special instructions: canned foods, fresh meat and seafood, frozen food, fresh fruits and vegetables); card "TSA local release (2025)" (Harrisburg International Airport, Nov. 24, 2025; through the checkpoint list; checked-bags list); card "Where the two differ" (gravy, jam and jelly, maple syrup; cranberry sauce named in the release only); footer lines (officer decides; no 2026 release found Nov. 4, 2026; sources; pages read Nov. 4, 2026) | pass |
| I2 | The diagram labels the 2025 release by year and airport in the card title and first line, and keeps the Food-page and release lists in separate cards | pass |
| I3 | **File checked as committed.** The PNG and SVG were staged back from the repository working tree after the write: PNG 1200 x 2724, 112,676 bytes at the source (118,328 bytes after transfer, which adds a C2PA block), pixel-identical to the local build; SVG 31 text elements identical to the local build (the transfer adds a `<metadata>` block). The PNG was opened and viewed from the repository copy | pass |
| I4 | Alt text 455 characters, the same string in the front matter and in the body image; matches the three cards and the footer line (the officer decides) | pass |
| I5 | Meta description 133 characters | pass |
| I6 | Front matter complete (title, slug, meta, category, focus keyword, status draft, date, internal link candidate, image, alt); one H1; internal link to the 3-1-1 post | pass |
| I7 | Diagram history: a first build showed a clipped card title ("TSA local release, Harrisburg, Nov. 24, 2025" ran past the card); fixed by shortening the title and moving the airport and date to the first line; a second build removed a "Pennsylvania" label (not stated on the release page) and kept "Nov. 24, 2025" together with non-breaking spaces | fixed |

## Next

Gate 2 on the SHA of this commit only after the user decides on P1 and P4; the draft stays blocked from `ready` and WordPress until the 2026 notice is read.
