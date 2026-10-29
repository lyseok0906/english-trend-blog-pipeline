# QA record — alcohol-on-a-plane-tsa-faa

Article: `content/ready/alcohol-on-a-plane-tsa-faa.md`
Brief: `research/briefs/alcohol-on-a-plane-tsa-faa.md`. Sources: `research/sources/alcohol-on-a-plane-tsa-faa.md` (S1 TSA "Alcoholic beverages", S2 FAA PackSafe "Alcoholic Beverages", S3 eCFR 49 CFR 175.10, S4 TSA "Alcoholic beverages over 140 proof", S5 FAA PackSafe printable chart PDF).
Stage: draft. Latest revision after commit `6ff8034`: three wording fixes from the writer's pre-Gate-2 self-check (below). First Gate 1 on 2026-10-13 (commit `27955a4`, 20 claims, no rule stated over 70%). **Second pass 2026-10-13 on the user's request:** over-70% prohibition added, 5-liter per-passenger total confirmed, 24%-or-less wording scoped, airline-check line kept, diagram and alt text made, Gate 1 re-run (below). **Gate 2 (independent, ChatGPT) PASS on commit `33aea2b`, reported by the user 2026-10-13. Stage stays `draft`: not approved for `ready`, not on WordPress, not published.** Post-pilot article: not counted in the pilot 12.

Method: S1, S2, S3 and S4 were opened in the built-in browser on 2026-10-13 and the quoted statements were tested by script against each page's text (S1 11 of 11, S2 9 of 9, S3 6 of 6, S4 7 of 7): all present. **S5 (FAA printable chart, PDF) was not opened directly and not script-tested**; it was read twice through a document-reader tool and the reads agree (over 140 proof: "Not allowed in Carry-On or Checked Bags"; under 140 proof: unopened retail packaging, 5 L per packaging and 5 L total per passenger, 100-ml carry-on footnote; "Updated: 11/14/25"). Every claim that rests on S5 alone is marked below. The over-70% prohibition does not rest on S5 alone: TSA's own entry (S4) says "No" for both carry-on and checked bags. The diagram was viewed after export and its text compared with the article (see I1-I3). This is the drafting and factual-QA re-check for a rule-type post; the re-check right before the user approves moving to `ready` and again right before publishing is still **mandatory**, **including a direct open of the FAA chart PDF**; if a page cannot be opened, do not publish.

## Gate 1 — Factual QA (claim by claim), re-run on the revised draft

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | TSA says alcoholic beverages are allowed in checked bags and in carry-on bags, carry-on amounts limited to 3.4 oz (100 ml) | S1-1, S1-2 | pass (attributed) |
| C2 | Checked bags: more than 24% but not more than 70% alcohol limited to 5 liters (1.3 gallons) per passenger, unopened retail packaging (TSA) | S1-3 | pass (attributed) |
| C3 | Checked bags: 24% alcohol or less not subject to limitations (TSA). Scoped in the article: "TSA's statement about checked bags only"; table says "TSA sets no separate alcohol limit for checked bags"; it does not change the carry-on limit and does not speak for any airline | S1-4, S1-1, S1-6 | pass (attributed; scope stated) |
| C4 | Wording as of October 13, 2026; five pages; describes the rules, no packing advice | Browser reads; scope | pass |
| C5 | Table rows: carry-on 3.4 oz (100 ml) or less; checked 24% or less not subject to limitations; checked more than 24% up to 70% limited to 5 liters (1.3 gallons) per passenger in unopened retail packaging; carry-on or checked more than 70% (over 140 proof) not allowed | S1-1, S1-3, S1-4, S4-2 | pass (attributed in the lead and the section text) |
| C6 | TSA's page adds that mini bottles of alcohol must be able to comfortably fit into a single quart-sized bag | S1-5 | pass (attributed) |
| C7 | Internal link to the published TSA 3-1-1 liquids article (https://statesideexplained.com/tsa-3-1-1-liquids-rule/) for the general carry-on liquids rule | Published article exists (live) | pass |
| C8 | Over 24% up to 70% (up to 140 proof): FAA says unopened retail packaging, 5 liters per packaging and 5 liters in total per passenger | S2-1; S5-2 | pass (S2 tested; S5 read via document reader, same figures) |
| C9 | The regulation says the same: unopened retail packagings not exceeding 5 liters, total net quantity per person of 5 liters; so the 5 liters is a total per passenger, not a per-bottle limit | S3-3, S2-1 | pass (the "so ..." sentence is a direct reading of "per packaging" plus "total per passenger" and "total net quantity per person") |
| C10 | TSA words it as 5 liters (1.3 gallons) per passenger for checked bags | S1-3 | pass (attributed) |
| C11 | FAA footnote: liquids, gels and aerosols in carry-on baggage are further limited to 100-ml (3.4 oz) containers at the TSA checkpoint | S2-2 | pass (attributed) |
| C12 | The regulation covers not more than 24% alcohol by volume and the article says the regulation "does not state a quantity limit" for them (no quantity appears in (a)(4)(i); stated as absence, not as a rule); and more than 24% and not more than 70% in unopened retail packagings not exceeding 5 liters, carry-on or checked | S3-2, S3-3 | pass |
| C13 | The regulation lists alcoholic beverages among hazardous materials excepted for passengers when the section's requirements are met; its exception covers beverages up to 70% alcohol by volume | S3-1, S3-3 | pass (attributed; the article does not say the regulation prohibits stronger beverages) |
| C14 | TSA has a separate "What can I bring?" entry for alcoholic beverages over 140 proof, defined as more than 70% alcohol (over 140 proof), including grain alcohol and 151 proof rum | S4-1 | pass (tested on page text) |
| C15 | TSA's entry lists both carry-on bags and checked bags as "No" | S4-2 | pass (tested on page text) |
| C16 | Lead and table: TSA lists beverages over 70% alcohol (over 140 proof) as not allowed in carry-on or checked bags | S4-1, S4-2 | pass (attributed to TSA) |
| C17 | FAA PackSafe chart, updated November 14, 2025: row for alcoholic beverages over 140 proof (greater than 70% alcohol by volume, more than 140 proof), marked not allowed in carry-on or checked bags | S5-1 | **pass with caveat: read via document reader twice, not opened directly; direct check mandatory before approval** |
| C18 | The FAA's separate web page has the same heading and refers to the regulation, but its text does not state a rule | S2-4 | pass (absence checked in the page DOM) |
| C19 | TSA: FAA regulations prohibit consuming alcohol on board unless served by a flight attendant; FAA page: unless served by the air carrier; TSA: flight attendants may not serve an intoxicated passenger | S1-7, S2-3 | pass (attributed) |
| C20 | TSA says to check with your airline before bringing any alcoholic beverages on board (airline-check line kept); TSA's pages say the final decision rests with the TSA officer (S1 and S4) | S1-6, S1-8, S4-3 | pass (attributed) |
| C21 | Scope: no duty-free or inbound international, airline policy, state or foreign laws, alcohol for sale, packing, quantity advice | Scope statement | pass (scope) |
| C22 | Sources: five pages checked October 13, 2026, with the page dates shown (TSA Feb 20, 2025 twice; FAA web Apr 13, 2026; FAA chart "Updated: 11/14/25", a PDF; eCFR up to date as of 10/08/2026) | Reads | pass |
| C23 | Lead: "TSA lists alcoholic beverages with more than 70% alcohol (over 140 proof) as not allowed in either carry-on or checked bags" — does not claim the FAA web page or the regulation says so | S4 | pass |

## Image and alt text

| # | Check | Result |
|---|---|---|
| I1 | Diagram cards compared with the article (third card title now "Checked bag: over 24% up to 70%", matching "not more than 70%" in the body and "up to 70%" in the alt): carry-on 3.4 oz (100 ml) or less, mini bottles in a single quart-sized bag (TSA); checked 24% or less not subject to limitations in checked bags (TSA); checked over 24% to 70% unopened retail packaging only, 5 L (1.3 gal) total per passenger (TSA and FAA); over 70% (over 140 proof) not allowed in carry-on or checked bags (TSA; FAA chart), includes grain alcohol and 151 proof rum; on board: FAA, no drinking alcohol on board unless the air carrier serves it | pass (each card's attribution matches S1-S5) |
| I2 | Footer: "TSA: check with your airline." "The TSA officer makes the final decision." "% = alcohol by volume (FAA, 49 CFR 175.10)" "Source: TSA, FAA and eCFR pages, read Oct. 13, 2026" | pass (the "% = alcohol by volume" note matches the FAA/regulation wording; TSA says only "alcohol") |
| I3 | Image re-exported and viewed again after the title change (1200 x 2286, PNG8, 115,201 bytes; the longer title fits inside its card): no clipped text, no logo, no photo, no brand name; source SVG has no embedded metadata | pass |
| I4 | Alt text, 402 characters: states carry-on, checked 24% or less, over 24% up to 70% (unopened retail packaging, 5 liters total per passenger), over 70% not allowed, on board (no drinking alcohol unless the air carrier serves it) and "Check with your airline"; same text in front matter and in the image embed; no keyword stuffing | pass |
| I5 | Meta description, 134 characters (<160): "TSA lists alcohol as allowed in carry-on (3.4 oz max) and checked bags, with limits, and not allowed above 70% alcohol. See the rules." | pass |

Result (re-run after the three wording fixes): 23 of 23 claims and 5 of 5 image checks pass. **One caveat is open and travels with the record: C17 (and the FAA-chart part of C8) rests on a document-reader read of the FAA PDF, not on a direct open.** The over-70% rule itself is also stated by TSA's own entry (C14-C16), tested on the page text. Wording watch for Gate 2: "alcohol" (TSA) versus "alcohol by volume" (FAA, regulation) is stated once on purpose; the over-70% section says what each source states and notes that the FAA web page text is silent.

## Pre-Gate-2 self-check by the writer (NOT Gate 2)

Done 2026-10-13 by Claude, who wrote the article, on commit `6ff8034`, at the user's request. **This is a writer's self-check, not an independent review, and it is not recorded as a Gate 2 pass.** It checked the four points the user listed (over-70% wording; 5 L as a per-passenger total; 24%-or-less scoped to TSA checked bags; diagram cards and alt text against the body) and found them consistent. Three wording fixes were decided by the user and applied afterwards: (1) diagram card title "over 24% to 70%" changed to "over 24% up to 70%" (SVG and PNG regenerated); (2) body: "without a quantity limit" changed to "does not state a quantity limit for them"; (3) alt text extended with the "On board" card and "Check with your airline" (313 to 402 characters). The user decided not to force the focus keyword into the meta description or first sentence: it is in the title and H1, which is enough.

## Gate 2 — English + SEO QA

**PASS** — independent Gate 2 by ChatGPT, on commit `33aea2b`, as reported by the user on 2026-10-13. No change requested to the body, SEO (title, meta description, focus keyword handling), the diagram SVG or the alt text. This is the result as relayed by the user; the reviewer's own text is not stored in the repository. The writer's pre-Gate-2 self-check above remains a separate item and was never counted as Gate 2.

Gate 2 does not replace the source re-check below. It reviewed the text, not the live pages.

## Pre-approval re-check of the five official pages (2026-10-29, Claude)

Requested by the user on 2026-10-29 as the condition for moving this article to `ready`. Each page was opened as a real page load in the built-in browser (signed-in pane on the user's computer) and compared with the draft and with source notes S1 to S5. Nothing on WordPress was touched; the article stays `draft`.

| # | Source | Page date shown on 2026-10-29 | Compared with the draft | Result |
|---|---|---|---|---|
| 1 | TSA "Alcoholic beverages" | Last Updated Feb 20, 2025 (same) | Carry-on: Yes, 3.4 oz / 100 ml or less; checked: Yes; over 24% to 70%: 5 liters (1.3 gallons) per passenger in unopened retail packaging; 24% or less not subject to limitations in checked bags; mini bottles must fit comfortably in a single quart-sized bag; check with your airline; FAA regulations prohibit drinking on board unless served by a flight attendant; flight attendants may not serve an intoxicated passenger; final decision rests with the TSA officer; refers to 49 CFR 175.10(a)(4) | no difference |
| 2 | TSA "Alcoholic beverages over 140 proof" | Last Updated Feb 20, 2025 (same) | Carry-on: No; checked: No; more than 70% alcohol (over 140 proof), including grain alcohol and 151 proof rum; refers to 49 CFR 175.10(a)(4); final decision rests with the TSA officer | no difference |
| 3 | FAA PackSafe "Alcoholic Beverages" web page | Last updated Monday, April 13, 2026 (same) | More than 24% up to 70% (up to 140 proof), unopened retail packaging: 5 L (1.3 gallons) per packaging and 5 L total per passenger; carry-on liquids further limited to 100-ml (3.4 oz) containers at the TSA checkpoint; no drinking on board unless served by the air carrier; the "Over 140 Proof" heading gives only the strength and the regulation reference, with no rule sentence (as recorded in C18) | no difference |
| 4 | eCFR 49 CFR 175.10 | Page says "up to date as of 10/27/2026" (was 10/08/2026 on 2026-10-13); the page also says Title 49 was last amended 10/13/2026 | Paragraph (a)(4) read word for word: (i) not more than 24% alcohol by volume; (ii) more than 24% and not more than 70% alcohol by volume in unopened retail packagings not exceeding 5 liters (1.3 gallons) in carry-on or checked baggage, with a total net quantity per person of 5 liters (1.3 gallons). Same text as S3 | no difference in (a)(4); only the "up to date as of" date moved |
| 5 | FAA PackSafe printable chart (PDF) | "Updated: 11/14/25" printed at the foot of page 3 (same) | **Opened directly in the browser** (a 9-page PDF rendered in the browser's own PDF viewer; read at 120% zoom, page 3). Row "Alcoholic Beverages under 140 Proof" (more than 24% but not more than 70%): carry-on yes, must be in unopened retail packagings, liquids further limited to 100-ml (3.4 oz) containers at the TSA checkpoint; checked yes, unopened retail packagings, 5 L (1.3 gallons) per packaging and 5 L total per passenger. Row "Alcoholic Beverages over 140 Proof" (greater than 70%, including grain alcohol and 151 proof rum): "Not allowed in Carry-On or Checked Bags" in both columns | no difference |

**Result: no source changed and no statement of the draft is contradicted. The caveat on C17 (and the FAA-chart part of C8) is closed: the FAA PDF was opened directly and the over-70% and 5 L rows match.** The article text was not changed, so Gate 1 and Gate 2 results stand.

Notes and limits: (a) the chart's printed date is the same as on 2026-10-13, but the file itself was served with an HTTP "Last-Modified" of 2026-05-14 (read from the response header); the printed update date and the alcohol rows are unchanged, so this is recorded as an observation only, not as a source change; (b) the eCFR "up to date as of" date in the article's Sources section (10/08/2026) describes the day of the original check on 2026-10-13 and is left as it is; a re-check date is only added to the article if the user decides to (not done); (c) the PDF text could not be extracted by script, so it was read visually; (d) this re-check covers the pages' content on 2026-10-29 only; **the same five-page re-check is required again right before publishing**, and the FAA PDF must be opened directly again then.

## Conditions before the move to `ready` (user decision 2026-10-13)

Before the user approves moving this article to `ready`, **all five pages must be re-read**: (1) TSA "Alcoholic beverages", (2) TSA "Alcoholic beverages over 140 proof", (3) FAA PackSafe "Alcoholic Beverages" web page, (4) eCFR 49 CFR 175.10, (5) FAA PackSafe printable chart (PDF). **The FAA PDF must be opened directly in a browser, not through a document reader.** If the PDF cannot be opened directly, the article is **not** published. If a re-read shows a changed or missing statement, the draft goes back to Gate 1 before anything else. The same re-check is required again right before publishing.

## Move to `ready` (user approval 2026-10-29)

The user approved moving this article to `ready` on 2026-10-29 after the five-page re-check above (no source changed; FAA PDF opened directly). The file was moved from `content/drafts/` to `content/ready/` and the front matter set to `status: ready`; the article text, title, meta description, image and alt text were not changed, so the Gate 1 and Gate 2 results stand. Not on WordPress and not published; the WordPress upload and publishing are separate steps the user will start.

## Not done yet

- WordPress draft and publishing (not started; the user will request them).
- The five-page re-check again right before publishing, with the FAA PDF opened directly again (mandatory).
- Search demand and competition not measured.
