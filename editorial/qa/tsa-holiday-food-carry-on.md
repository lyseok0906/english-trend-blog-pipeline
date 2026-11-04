# QA record — tsa-holiday-food-carry-on

Article: `content/drafts/tsa-holiday-food-carry-on.md` (draft, 2026-11-04, about 1,375 words in the body, one H1, seven H2 sections including Sources).
Brief: `research/briefs/tsa-thanksgiving-food-carry-on.md` (backlog row 8; the slug changed from `tsa-thanksgiving-food-carry-on` to `tsa-holiday-food-carry-on` because the article is framed as holiday food, as the user's scope approval of 2026-11-04 asked). Sources: `research/sources/tsa-thanksgiving-food-carry-on.md`.
Stage: draft. Gate 1 (Claude) run on 2026-11-04. Gate 2 round 1 (ChatGPT, base `a6de32c`, user-reported 2026-11-04): FIX, applied 2026-11-04 (section "Gate 2 FIX round 1"); **Gate 2 round 2 (base `0336d6b`, user-reported 2026-11-04): FIX, one item, applied 2026-11-04** (section "Gate 2 FIX round 2"); round 3 has not run. **Not for publication until a TSA 2026 Thanksgiving notice that contains food guidance has been read, compared with this draft and the draft revised and re-reviewed (user rule, 2026-11-04).** Not in `content/ready/`, not uploaded to WordPress.

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

## Gate 2 FIX round 1 (base a6de32c, 2026-11-04)

Gate 2 result (ChatGPT, user-reported): FIX. Requests: (1) make clear in the body, diagram and alt that 3.4 oz is a per-container limit, checked against TSA's text; (2) make the display title of the link to the TSA 3-1-1 article match its real title. The hold on publication until a 2026 TSA food notice is read stays.

| # | Change | Result |
|---|---|---|
| F1 | Lead: "...and allows gravy, jam, maple syrup and sauces in a carry-on at 3.4 ounces (100 ml) or less" followed by "TSA's liquids page says that limit applies to each container, not to a total." | applied |
| F2 | New paragraph at the end of "What TSA's Food page says": the Food page's value reads "Yes (Less than or equal to 3.4oz/100 ml allowed)" and does not say what the 3.4 ounces is measured against; TSA's "Liquids, Aerosols, and Gels Rule" page limits items to travel-sized containers of 3.4 ounces (100 ml) or less per item in a quart-sized bag and sends larger containers to checked baggage; so the 3.4 ounces is the size of each container, not a total for the trip; the pages do not go further (for example a larger container only partly filled) and the article does not either | applied |
| F3 | Release section: for casseroles with liquid components the release adds that each liquid or semi-liquid item must be in a container of 3.4 ounces or less and fit into a single quart-sized, clear, resealable plastic bag | applied |
| F4 | Differences table: "Carry-on: Yes, 3.4 oz or less (container size, see above)"; the paragraph below it says "(the size of each container)" and "for those items"; the Soups sentence says "3.4 ounces (100 ml) or less" | applied |
| F5 | Link text: "What Is the TSA 3-1-1 Liquids Rule? What's Exempt?", the live post's H1 (opened 2026-11-04; the earlier long title was wrong); front-matter link note updated | applied |
| F6 | Alt (514 characters, front matter and body identical): "gravy, jam, maple syrup and sauces at 3.4 oz or less in carry-on, a limit TSA's liquids page applies to each container" | applied |
| F7 | Diagram: card 1 says "Carry-on, 3.4 oz (100 ml) or less" and adds the line "TSA liquids page: the 3.4 oz limit is per container."; card 3 says "the Food page allows 3.4 oz or less in carry-on bags"; footer source line now "Source: tsa.gov Food, liquids pages, Harrisburg release" | applied |

**Official pages re-opened 2026-11-04 (built-in browser).**

| Page | Checked | Result |
|---|---|---|
| TSA, Liquids, Aerosols, and Gels Rule | "limited to travel-sized containers that are 3.4 ounces (100 milliliters) or less per item"; quart-sized bag; "Pack items that are in containers larger than 3.4 ounces or 100 milliliters in checked baggage" | present |
| TSA Harrisburg release (Nov. 24, 2025) | "Each liquid or semi-liquid item must be in a container of 3.4 ounces or less and fit into a single quart-sized, clear, resealable plastic bag." (in the casserole paragraph) | present |
| TSA Food page | 59 rows and value strings as in Gate 1 (read earlier the same day) | unchanged |
| Live 3-1-1 post | H1 "What Is the TSA 3-1-1 Liquids Rule? What's Exempt?"; its text uses "each container holds 3.4 ounces ... or less" | matches |

**Image files checked as committed (new transfer names; staged back from the repository).** PNG 1200 x 2946, pixel-identical to the local build (126,485 bytes in the repository after the transfer added a C2PA block); SVG 34 text elements identical to the build; the PNG was opened and viewed from the repository copy; the diagram, body and alt agree on the per-container wording and the year and airport label.

Open points P1 to P6 above are unchanged (P1, the 2026 notice, still blocks publication). Not in ready, not on WordPress. Next: Gate 2 round 2 on the new SHA.

## Gate 2 FIX round 2 (base 0336d6b, 2026-11-04)

Gate 2 result (ChatGPT, user-reported): FIX, one item. The body and diagram rely on TSA's "Liquids, Aerosols, and Gels Rule" page, so it must be listed under Sources with its actual check date, and the introduction ("what TSA says in two places") must reflect the added source. The hold on publication until a 2026 TSA food notice is read stays. The rest of the article, the 3.4-ounce per-container wording, the link text, the diagram and the alt were not questioned.

| # | Change | Result |
|---|---|---|
| J1 | Sources list: new entry "TSA, 'Liquids, Aerosols, and Gels Rule' (used for what the 3.4-ounce limit refers to; the page shows no update date)" with the URL `https://www.tsa.gov/travel/security-screening/liquids-aerosols-gels-rule` | applied |
| J2 | Sources paragraph: "The Food page, the Liquids, Aerosols, and Gels Rule page and the press-release list were read on November 4, 2026, and both press releases were read the same day. The Food page and the Liquids page show no update date." | applied |
| J3 | Introduction: the article covers what TSA says about holiday food in two places (Food list; Harrisburg release) and "also uses a third TSA page, 'Liquids, Aerosols, and Gels Rule,' only to explain what the 3.4-ounce limit refers to. All three were read on November 4, 2026. The Food page and the Liquids page show no date." | applied |
| J4 | "What this article does not cover": "what two TSA sources state" became "what the TSA pages and the release listed under Sources state" | applied |
| J5 | Sections "Where the two TSA sources differ" and the alt ("two TSA sources") unchanged: they compare the Food page and the release; the Liquids page is a supporting definition, not a third side of the comparison | kept |

**Check date of the Liquids page.** First opened 2026-11-04 for Gate 2 FIX round 1 (the page's own first read) and opened again the same day for this round: title "Liquids, Aerosols, and Gels Rule | Transportation Security Administration"; no update or year date anywhere on the page (script search for "updated", "last modified" and month-day-year dates found none); the three strings the article relies on are present: "3.4 ounces (100 milliliters) or less per item", "quart-sized bag" and "Pack items that are in containers larger than 3.4 ounces or 100 milliliters in checked baggage". The article therefore states 2026-11-04 as the read date and says the page shows none of its own.

Additional claims for the Gate 1 table (numbering continues):

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C32 | The Liquids page is used only to explain what the 3.4-ounce limit refers to; items in travel-sized containers of 3.4 ounces (100 ml) or less per item, in a quart-sized bag; larger containers in checked baggage | Liquids page | pass |
| C33 | The Liquids page shows no update date; read on November 4, 2026 | Liquids page | pass (absence check) |
| C34 | Sources: five TSA pages (Food page, Harrisburg release, national release, Liquids page, press-release list), each opened on 2026-11-04 | Reads | pass |

Result after this round: 34 of 34 claims pass. The body text is about 1,626 words by the same count as before (the earlier counts omitted nothing; the additions are the per-container paragraph and the source lines). The diagram and alt were not changed in this round (PNG and SVG in the repository are the files committed in `0336d6b`). Open points unchanged; P1 (the 2026 notice) still blocks publication. Next: Gate 2 round 3 on the new SHA.
