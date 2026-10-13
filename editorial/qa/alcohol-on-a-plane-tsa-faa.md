# QA record — alcohol-on-a-plane-tsa-faa

Article: `content/drafts/alcohol-on-a-plane-tsa-faa.md`
Brief: `research/briefs/alcohol-on-a-plane-tsa-faa.md`. Sources: `research/sources/alcohol-on-a-plane-tsa-faa.md` (S1 TSA "Alcoholic beverages", S2 FAA PackSafe "Alcoholic Beverages", S3 eCFR 49 CFR 175.10).
Stage: draft written 2026-10-13; Gate 1 done by Claude on 2026-10-13. **Not sent to Gate 2, not approved, not on WordPress, not published.** Post-pilot article: not counted in the pilot 12.

Method: three official pages opened in the built-in browser on 2026-10-13 and read; the quoted statements were tested by script against each page's text (TSA 11 of 11, FAA 9 of 9, eCFR 6 of 6): all present. The FAA page DOM was checked for images or icons under "Alcoholic Beverages Over 140 Proof": none, and no text other than the definition and the regulation link. This is the drafting and factual-QA re-check for a rule-type post; the re-check right before the user approves moving to `ready` and again right before publishing is still **mandatory**; if a page cannot be opened, do not publish.

## Gate 1 — Factual QA (claim by claim)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | TSA says alcoholic beverages are allowed in checked bags and in carry-on bags, carry-on amounts limited to 3.4 oz (100 ml) | S1-1, S1-2 | pass (attributed) |
| C2 | Checked bags: more than 24% but not more than 70% alcohol limited to 5 liters (1.3 gallons) per passenger, unopened retail packaging (TSA) | S1-3 | pass (attributed) |
| C3 | Checked bags: 24% alcohol or less not subject to limitations (TSA) | S1-4 | pass (attributed) |
| C4 | Wording as of October 13, 2026; three pages; describes the rules, no packing advice | Browser reads; scope | pass |
| C5 | Table rows: carry-on 3.4 oz (100 ml) or less; checked 24% or less not subject to limitations; checked more than 24% up to 70% limited to 5 liters (1.3 gallons) per passenger in unopened retail packaging | S1-1, S1-3, S1-4 | pass (attributed) |
| C6 | TSA's page adds that mini bottles of alcohol must be able to comfortably fit into a single quart-sized bag | S1-5 | pass (attributed) |
| C7 | Internal link to the published TSA 3-1-1 liquids article (https://statesideexplained.com/tsa-3-1-1-liquids-rule/), for the general carry-on liquids rule | Published article exists (live) | pass |
| C8 | FAA: same figures for more than 24% but not more than 70% alcohol by volume (up to 140 proof); unopened retail packaging; 5 liters per packaging and 5 liters in total per passenger | S2-1 | pass (attributed) |
| C9 | FAA footnote: liquids, gels and aerosols in carry-on baggage are further limited to 100-ml (3.4 oz) containers at the TSA checkpoint | S2-2 | pass (attributed) |
| C10 | Both TSA and the FAA point to 49 CFR 175.10(a)(4) | S1-8, S2-4 | pass |
| C11 | The regulation lists alcoholic beverages among hazardous materials the subchapter's rules do not apply to for passengers when the section's requirements are met | S3-1 | pass (attributed) |
| C12 | The regulation covers not more than 24% alcohol by volume, and more than 24% and not more than 70% in unopened retail packagings not exceeding 5 liters, carry-on or checked, 5 liters per person in total | S3-2, S3-3 | pass (attributed) |
| C13 | The FAA page and the regulation use alcohol by volume; TSA's page says only "alcohol" | S1-3, S2-1, S3-2 | pass |
| C14 | TSA's page does not address beverages above 70% | S1 full text read | pass (absence checked in the page text) |
| C15 | FAA heading "Alcoholic Beverages Over 140 Proof" defines them as greater than 70% alcohol by volume, including grain alcohol and 151 proof rum, and refers to the regulation; the page text under it states no rule | S2-4 | pass (absence checked in the page DOM) |
| C16 | The regulation's exception, as written, covers beverages up to 70% alcohol by volume; the article states no rule for stronger beverages | S3-2, S3-3; scope | pass (scope; no inference stated as fact) |
| C17 | TSA: FAA regulations prohibit consuming alcohol on board unless served by a flight attendant; FAA's page: unless served by the air carrier; TSA: flight attendants may not serve an intoxicated passenger | S1-7, S2-3 | pass (attributed) |
| C18 | TSA says to check with your airline before bringing any alcoholic beverages on board; the final decision rests with the TSA officer | S1-6, S1-8 | pass (attributed) |
| C19 | Scope: no duty-free or inbound international, airline policy, state or foreign laws, alcohol for sale, packing, quantity advice, no rule over 70% | Scope statement | pass (scope) |
| C20 | Sources: three pages checked October 13, 2026, with the page dates shown (TSA Feb 20, 2025; FAA Apr 13, 2026; eCFR up to date as of 10/08/2026) | Browser reads | pass |

Result: 20 of 20 pass; no unsupported claim. Wording watch for Gate 2: "alcohol" versus "alcohol by volume" (C13) is stated once on purpose; the "over 70%" section states what is not said rather than a rule.

## Gate 2 — English + SEO QA

Not done. To be sent to ChatGPT by commit SHA when the user decides.

## Not done yet

- Diagram and image alt text (front matter says `pending`).
- Mandatory pre-approval re-check of the three pages.
- Search demand and competition not measured.
