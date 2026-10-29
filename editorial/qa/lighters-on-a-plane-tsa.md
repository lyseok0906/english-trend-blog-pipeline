# QA record — lighters-on-a-plane-tsa

Article: `content/drafts/lighters-on-a-plane-tsa.md` (draft, 2026-10-29, about 1,540 words).
Brief: `research/briefs/lighters-on-a-plane-tsa.md`. Sources: `research/sources/lighters-on-a-plane-tsa.md` (S1 to S4 the five TSA pages, S5 FAA PackSafe Lighters, S6 FAA printable chart, S7 eCFR 49 CFR 175.10; S8 FAA 2013 FAQ and S9 DOT-SP 14415 are **not used in the article body**, see "The 2013 FAQ and the special permit").
Stage: draft. Gate 1 (Claude) run on 2026-10-29. **Gate 2 (ChatGPT, by commit SHA) has not run. Nothing is in `content/ready/`, nothing is uploaded to WordPress, nothing is published.**

Method: before drafting (earlier on 2026-10-29) all pages were opened in the built-in browser and each quoted statement was tested against the page or PDF text (see the source notes, "Verification"). At Gate 1, after the draft existed, the FAA page and chart, the five TSA pages and the eCFR section were opened again (2026-10-29) and the statements the draft relies on were tested again by script: FAA page 11 of 11 plus "does not mention the exemption" confirmed; FAA chart (PDF text layer, 9 pages) 5 of 5; TSA pages 27 of 27 (disposable and Zippo 6 of 6 with "no number limit stated" confirmed, arc and electronic 7 of 7, lithium battery powered 3 of 3, torch 4 of 4 with "the torch page does not use the name butane" confirmed, lighter fluid 3 of 3); eCFR 7 of 7 ("up to date as of 10/27/2026"; title last amended 10/13/2026). The chart's lighter rows and the FAA FAQ's two pages were also checked on screen in the PDF viewer (source notes).

## Gate 1 — Factual QA (claim by claim)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | Lead: TSA's page for disposable and Zippo lighters lists them as allowed in carry-on bags | S1-1 | pass (attributed) |
| C2 | Lead: the FAA says disposable (butane) and Zippo-type lighters are limited to one per passenger, in a carry-on bag or on the person | S5-2, S6-1 | pass (attributed) |
| C3 | Lead: TSA lists torch lighters as not allowed in carry-on or checked bags | S4-1 | pass (attributed) |
| C4 | Lead: the FAA says torch lighters are not allowed in the cabin or in checked baggage | S5-5, S6-3 | pass (attributed) |
| C5 | Lead: for checked bags, TSA's and the FAA's wording about disposable and Zippo lighters differs, and the article shows both | S1-2, S1-4 against S5-2, S6-2, S7-1 | pass (comparison of dated sources; see open point P1) |
| C6 | Wording as of October 29, 2026, from eight pages; TSA update dates July 14, 2026 (disposable and Zippo), November 4, 2024 (arc and electronic), October 10, 2024 (torch, lighter fluid, lithium battery powered) | Browser reads; S1 to S4 page dates | pass |
| C7 | The article describes the rules and gives no advice on what to pack | Scope | pass (no recommendation sentence in the body; the "agree" sentence reports what four sources say) |
| C8 | Table row 1: disposable and Zippo-type; TSA carry-on Yes, checked "Yes (Special Instructions)"; FAA one per passenger in carry-on or on one's person; the FAA chart says not allowed in checked bags; 49 CFR 175.10 on one's person or in carry-on only | S1-1, S1-2, S5-2, S6-2, S7-1 | pass |
| C9 | Row 2: arc/electronic page carry-on "Yes (Special Instructions)", checked No; lithium battery powered page carry-on Yes, checked No; FAA carry-on only with measures against unintentional activation and no recharging on board | S2-1, S3-1, S5-4 | pass |
| C10 | Row 3: torch lighters TSA No / No; FAA not allowed in the cabin or in checked baggage | S4-1, S5-5 | pass |
| C11 | Row 4: unabsorbed liquid fuel (desk, table, antique wick lighters): no separate TSA page read; FAA forbidden; 49 CFR 175.10 lighters containing unabsorbed liquid fuel (other than liquefied gas) not permitted on one's person, in carry-on or in checked baggage | S5-1, S7-2 | pass (the "no separate TSA page was read" is a statement about this work) |
| C12 | Row 5: lighter fluid TSA No / No; 49 CFR 175.10 lighter fuel and refills not permitted on one's person, in carry-on or in checked baggage | S4-3, S7-2 | pass |
| C13 | "Disposable and Zippo": TSA lists them as allowed in carry-on; the FAA groups absorbed-liquid and butane lighters with Zippo-type and disposable lighters as examples, one per passenger in carry-on or on one's person | S1-1, S5-2 | pass |
| C14 | FAA: a carry-on bag checked at the gate or at planeside, any lighter in it must be removed and kept with the passenger in the cabin | S5-3, S6 (same sentence) | pass |
| C15 | Regulation 49 CFR 175.10(a)(2) covers a lighter intended for use by an individual when carried on one's person or in carry-on baggage only | S7-1 | pass |
| C16 | How many: the FAA page and chart (updated November 14, 2025) say one per passenger for absorbed-liquid and butane lighters; the regulation says "a lighter" (singular); TSA's disposable and Zippo page states no number | S5-2, S6-1, S7-1, S1-5 | pass (absence confirmed by script) |
| C17 | TSA checked bags "Yes (Special Instructions)"; without fuel allowed; with fuel prohibited unless the DOT exemption, which TSA says allows up to two fueled lighters if properly enclosed in a DOT approved case | S1-2 to S1-4 | pass (attributed, wording kept close to the page) |
| C18 | The FAA describes these lighters as carried in carry-on or on the person; the regulation says the same; the chart's lighter row says "Not allowed in Checked Bags"; the FAA's web page does not mention the exemption | S5-2, S7-1, S6-2, S5-6 | pass (chart row also checked on screen; absence confirmed by script) |
| C19 | "What the pages used here do not settle": TSA's page does not name the exemption, the approval or the cases that qualify; the FAA's pages do not mention it; no permit document could be confirmed as current | S1-4 (the page's one sentence), S5-6, S9 | pass as a limitation statement; see open point P2 |
| C20 | TSA's page, the FAA's page and chart, and the regulation all allow a disposable or Zippo-type lighter in a carry-on bag | S1-1, S5-2, S6-1, S7-1 | pass |
| C21 | TSA's two pages for arc, electronic and lithium battery powered lighters, as described (the lithium page has no further text) | S2-1, S3-1 | pass |
| C22 | TSA's arc and electronic page: prevent unintentional activation of the heating element; the three examples; each lithium ion battery not to exceed 100 Wh; lithium metal 2 grams; recharging on board not permitted | S2-2 to S2-4 | pass |
| C23 | FAA page: lithium battery powered lighters (Tesla coil, flux, arc, double arc) carry-on only, with the same measures, limits and no recharging | S5-4 | pass |
| C24 | Regulation: batteries must meet the UN Manual of Tests and Criteria, Part III, Subsection 38.3; the lighters must have a safety cap or similar protection against unintentional activation | S7-3 | pass |
| C25 | Internal link to the published power-bank article for the rules on power banks | Published article exists (`https://statesideexplained.com/power-bank-on-a-plane-tsa-faa/`, live since 2026-10-07) | pass (the link text claims nothing about its content beyond "rules for power banks") |
| C26 | TSA torch page: No / No; describes a thin, needle-like flame, hotter (reaching 2,500 F) and more intense than common lighters | S4-1, S4-2 | pass |
| C27 | FAA page: torch lighters not allowed in the cabin or in checked baggage under both the Hazardous Materials Regulations and TSA security rules; the chart lists torch lighters as not allowed in carry-on or checked bags | S5-5, S6-3 | pass |
| C28 | Naming detail: the FAA page lists "butane lighters" among the other names for torch lighters, while its entry for butane lighters (disposable lighters as an example) allows one per passenger; TSA's torch page does not use that name | S5 (both statements on the page), S4 | pass (absence on TSA's torch page confirmed by script) |
| C29 | FAA page: liquid-fuel lighters without an absorbent lining, such as desk and table lighters and antique wick lighters, are forbidden; regulation: lighter fuel, refills and lighters containing unabsorbed liquid fuel (other than liquefied gas) not permitted on one's person, in carry-on or in checked baggage; TSA lighter fluid No / No | S5-1, S7-2, S4-3 | pass |
| C30 | TSA's pages: the final decision rests with the TSA officer; TSA's disposable and Zippo page says to see the FAA website for questions about regulations | S1-6 (and the footer on every TSA page read) | pass |
| C31 | Scope list (matches, e-cigarettes and vaping devices, camping stoves, butane canisters, mailing, other countries, airline policy, how to pack) and "does not track changes" | Scope | pass |
| C32 | Sources list: eight pages with the dates shown (TSA July 14, 2026; Nov 4, 2024; Oct 10, 2024 three times; FAA web Apr 13, 2026; FAA chart "Updated: 11/14/25", a PDF; eCFR "up to date as of 10/27/2026") | Reads | pass |

Result: 32 of 32 claims pass as attributed statements of the eight pages. Two things are **not** passes in the sense of a rule the article could state; they are reported as open points below.

## Open points reported (rules the article cannot state as one clear rule)

- **P1 — Checked bags for disposable and Zippo-type lighters.** TSA says "Yes (Special Instructions)" (fuel-free lighters allowed; fueled lighters only under a DOT exemption, up to two in an approved case). The FAA page, the FAA chart and the regulation describe carry-on or person only, and the chart says "Not allowed in Checked Bags". The sources do not reconcile these. The article shows both side by side and does not choose. A reader still cannot get one plain checked-bag answer from the pages, and the article says so ("where TSA's and the FAA's wording differs").
- **P2 — The DOT exemption.** The article repeats TSA's one sentence and says it cannot explain the exemption. Why it cannot: TSA's page does not name the permit, the case or the quantity conditions beyond one sentence; the FAA pages do not mention it; the only permit document found (DOT-SP 14415, third revision, April 26, 2013, Prometheus International) shows an expiration date of February 28, 2017, and no current permit was found. Whether the exemption is still in force, in what form, and for which cases could not be confirmed.
- **P3 — Number of lighters.** TSA states no number; the FAA page, chart and regulation point to one. Attributed, not reconciled.
- **P4 — Torch lighter label.** The FAA page lists "butane lighters" among names for torch lighters while allowing butane lighters elsewhere on the same page. The article notes this and uses the description from TSA's torch page.

## The 2013 FAQ and the special permit (recorded, not used in the body)

User instruction 2026-10-29: record the older FAQ in the source notes and QA first; propose before putting it in the body.

- **What it is:** FAA "Airline Passengers and Lighters FAQ's", November 18, 2013, opened directly in the PDF viewer (2 pages). It says torch lighters and up to two additional lighters may be carried in checked baggage in DOT-approved airtight travel containers (U.S. domestic travel only), and its table marks that case "Yes (In the U.S.)". It also says one lighter in the cabin, and its table marks disposable and Zippo-type lighters "No" for checked baggage.
- **How it differs from the current pages:** the torch statement conflicts with TSA's torch page (No / No, Oct 10, 2024) and with the FAA's page (Apr 13, 2026) and chart (11/14/25). On disposable and Zippo-type lighters in checked bags, it is closer to the FAA's current wording than to TSA's page, except for the permit-container case that TSA's exemption sentence appears to correspond to (this is a reading, not something any page states).
- **Why the body does not use it:** it is more than twelve years old, the permit mechanism it relies on could not be confirmed as current (P2), and quoting it would put a possibly superseded statement next to current pages.
- **Proposal for the user (not applied):** the reader need is real but small. A reader who finds the FAQ on the FAA site may see torch lighters allowed in checked bags and wonder. If the user wants it addressed, one dated sentence could say that an older FAA FAQ (November 2013) describes DOT-approved travel containers for torch lighters in checked baggage in U.S. domestic travel, and that the FAA's current web page and chart and TSA's torch page say torch lighters are not allowed in either place, so the article follows the current pages. Claude's judgment: leave it out of the body now, and add the sentence only if Gate 2 or the user asks.

## Image and alt text

| # | Check | Result |
|---|---|---|
| I1 | Diagram cards compared with the article: disposable and Zippo-type (carry-on allowed per TSA, FAA one per passenger in carry-on or on the person; checked bag TSA yes with special instructions, FAA chart not allowed); arc, electronic, lithium battery (carry-on only, checked bag no, prevent unintentional activation, no recharging on board, up to 100 Wh or 2 g lithium metal); torch lighters (not allowed in carry-on or checked bags, TSA and FAA); unabsorbed liquid fuel and lighter fluid or refills (not allowed; FAA, 49 CFR 175.10, TSA for lighter fluid) | pass |
| I2 | Footer: "The TSA officer makes the final decision." "One-lighter limit: FAA page and chart" "Source: TSA, FAA and eCFR pages, read Oct. 29, 2026" (the one-lighter line does not attribute the limit to TSA or the regulation) | pass |
| I3 | Image viewed after export (1200 x 2319, PNG8 with 64 colors, 96,820 bytes): no clipped text, no logo, no photo, no brand name other than the word "Zippo-type" used by the FAA; source SVG (`assets/raw/lighters-on-a-plane-tsa.svg`) has a title element and no embedded metadata | pass |
| I4 | Alt text, 462 characters, matches the diagram cards and the front matter; states the TSA and FAA differences for checked bags and ends with the TSA officer line | pass |
| I5 | Meta description, 129 characters (<160): "TSA and the FAA list lighters by type: disposable, Zippo-type, arc and torch. See what each says about carry-on and checked bags." | pass |
| I6 | Front matter: title, slug, meta description, category, focus keyword, status, date, internal-link candidates, image, image alt present; one H1, eight H2 sections plus Sources | pass |

## Gate 2 — English + SEO QA

Not run. Requested from ChatGPT by commit SHA after the user pushes. Points for the reviewer: the checked-bag section (P1, P2), the table's wording, whether the lead gives the answer early enough, and whether the 2013 FAQ proposal above should be adopted.

## Not done yet

- Gate 2 (independent).
- Fresh re-check of all eight pages before approval and again right before publishing (FAA chart PDF opened directly).
- User approval to move to `content/ready/`; WordPress draft; publishing.
