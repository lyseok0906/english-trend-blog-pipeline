# QA record — alcohol-on-a-plane-tsa-faa

Article: `content/drafts/alcohol-on-a-plane-tsa-faa.md`
Brief: `research/briefs/alcohol-on-a-plane-tsa-faa.md`. Sources: `research/sources/alcohol-on-a-plane-tsa-faa.md` (S1 TSA "Alcoholic beverages", S2 FAA PackSafe "Alcoholic Beverages", S3 eCFR 49 CFR 175.10, S4 TSA "Alcoholic beverages over 140 proof", S5 FAA PackSafe printable chart PDF).
Stage: draft. First Gate 1 on 2026-10-13 (commit `27955a4`, 20 claims, no rule stated over 70%). **Second pass 2026-10-13 on the user's request:** over-70% prohibition added, 5-liter per-passenger total confirmed, 24%-or-less wording scoped, airline-check line kept, diagram and alt text made, Gate 1 re-run (below). **Not sent to Gate 2, not approved, not on WordPress, not published.** Post-pilot article: not counted in the pilot 12.

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
| C12 | The regulation covers not more than 24% alcohol by volume without a quantity limit; and more than 24% and not more than 70% in unopened retail packagings not exceeding 5 liters, carry-on or checked | S3-2, S3-3 | pass |
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
| I1 | Diagram cards compared with the article: carry-on 3.4 oz (100 ml) or less, mini bottles in a single quart-sized bag (TSA); checked 24% or less not subject to limitations in checked bags (TSA); checked over 24% to 70% unopened retail packaging only, 5 L (1.3 gal) total per passenger (TSA and FAA); over 70% (over 140 proof) not allowed in carry-on or checked bags (TSA; FAA chart), includes grain alcohol and 151 proof rum; on board: FAA, no drinking alcohol on board unless the air carrier serves it | pass (each card's attribution matches S1-S5) |
| I2 | Footer: "TSA: check with your airline." "The TSA officer makes the final decision." "% = alcohol by volume (FAA, 49 CFR 175.10)" "Source: TSA, FAA and eCFR pages, read Oct. 13, 2026" | pass (the "% = alcohol by volume" note matches the FAA/regulation wording; TSA says only "alcohol") |
| I3 | Image viewed after export (1200 x 2286, PNG8, 115,044 bytes): no clipped text, no logo, no photo, no brand name; source SVG has no embedded metadata | pass |
| I4 | Alt text, 313 characters: states carry-on, checked 24% or less, over 24% up to 70% (unopened retail packaging, 5 liters total per passenger) and over 70% not allowed; no keyword stuffing | pass |
| I5 | Meta description, 134 characters (<160): "TSA lists alcohol as allowed in carry-on (3.4 oz max) and checked bags, with limits, and not allowed above 70% alcohol. See the rules." | pass |

Result: 23 of 23 claims and 5 of 5 image checks pass. **One caveat is open and travels with the record: C17 (and the FAA-chart part of C8) rests on a document-reader read of the FAA PDF, not on a direct open.** The over-70% rule itself is also stated by TSA's own entry (C14-C16), tested on the page text. Wording watch for Gate 2: "alcohol" (TSA) versus "alcohol by volume" (FAA, regulation) is stated once on purpose; the over-70% section says what each source states and notes that the FAA web page text is silent.

## Gate 2 — English + SEO QA

Not done. To be sent to ChatGPT by commit SHA when the user decides.

## Not done yet

- Direct open of the FAA printable chart PDF (S5) at the mandatory pre-approval re-check.
- Mandatory pre-approval re-check of all five pages.
- Search demand and competition not measured.
