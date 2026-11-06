# QA record — lighters-on-a-plane-tsa

Article: `content/ready/lighters-on-a-plane-tsa.md` (ready since 2026-11-04; written as a draft, 2026-10-29, about 1,590 words after the Gate 2 FIX round; the Gate 1 table below refers to the first version, commit `e75b3bc`/`50ce2d8`, and the FIX round section at the end re-checks every changed statement).
Brief: `research/briefs/lighters-on-a-plane-tsa.md`. Sources: `research/sources/lighters-on-a-plane-tsa.md` (S1 to S4 the five TSA pages, S5 FAA PackSafe Lighters, S6 FAA printable chart, S7 eCFR 49 CFR 175.10; S8 FAA 2013 FAQ and S9 DOT-SP 14415 are **not used in the article body**, see "The 2013 FAQ and the special permit").
Stage: **ready** (moved from `content/drafts/` on 2026-11-04 with the user's approval; status in the front matter set to `ready`). The earlier stage notes below are kept as history. Gate 1 (Claude) run on 2026-10-29. **Gate 2 round 1 (ChatGPT, base commit `50ce2d8`): FIX (5 items), applied. Gate 2 round 2 (base commit `aa72f32`): FIX (diagram files and checkpoint wording), applied; both are recorded in the last sections. Gate 2 round 3 (base `6415385`) = FIX, one item, applied 2026-11-04 (section "Gate 2 FIX round 3"); **Gate 2 round 4 (ChatGPT, base `51e6a1d`, user-reported 2026-11-04): PASS** (section "Gate 2 round 4 result"). Still not in ready; the mandatory TSA/FAA re-check and the existing ready and publication steps still apply. Nothing is in `content/ready/`, nothing is uploaded to WordPress, nothing is published.**

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

## Image and alt text (first version; superseded by the FIX round table below)

| # | Check | Result |
|---|---|---|
| I1 | Diagram cards compared with the article: disposable and Zippo-type (carry-on allowed per TSA, FAA one per passenger in carry-on or on the person; checked bag TSA yes with special instructions, FAA chart not allowed); arc, electronic, lithium battery (carry-on only, checked bag no, prevent unintentional activation, no recharging on board, up to 100 Wh or 2 g lithium metal); torch lighters (not allowed in carry-on or checked bags, TSA and FAA); unabsorbed liquid fuel and lighter fluid or refills (not allowed; FAA, 49 CFR 175.10, TSA for lighter fluid) | pass |
| I2 | Footer: "The TSA officer makes the final decision." "One-lighter limit: FAA page and chart" "Source: TSA, FAA and eCFR pages, read Oct. 29, 2026" (the one-lighter line does not attribute the limit to TSA or the regulation) | pass |
| I3 | Image viewed after export (1200 x 2319, PNG8 with 64 colors, 96,820 bytes): no clipped text, no logo, no photo, no brand name other than the word "Zippo-type" used by the FAA; source SVG (`assets/raw/lighters-on-a-plane-tsa.svg`) has a title element and no embedded metadata | pass |
| I4 | Alt text, 462 characters, matches the diagram cards and the front matter; states the TSA and FAA differences for checked bags and ends with the TSA officer line | pass |
| I5 | Meta description, 129 characters (<160): "TSA and the FAA list lighters by type: disposable, Zippo-type, arc and torch. See what each says about carry-on and checked bags." | pass |
| I6 | Front matter: title, slug, meta description, category, focus keyword, status, date, internal-link candidates, image, image alt present; one H1, eight H2 sections plus Sources | pass |

## Gate 2 — English + SEO QA

Round 1 (base `50ce2d8`): **FIX**, five items (F1 to F5), applied. Round 2 (base `aa72f32`): **FIX**, the diagram files in the repository and the checkpoint wording (L1 to L4), applied. Round 3 on the revised version: not run. Request from ChatGPT by commit SHA after the user pushes.

## Gate 2 FIX round (applied 2026-10-29)

### Instructions and what was changed

| # | Gate 2 instruction | Change made |
|---|---|---|
| F1 | In the diagram and alt, show TSA's checked-bag guidance as a conditional exception (without fuel / with fuel) and mark the difference from the FAA chart | Diagram card 1 now has four labelled lines: "Carry-on bag" (FAA first, then TSA), "Checked bag, TSA" (allowed without fuel; with fuel prohibited unless a DOT exemption applies, up to two, in a DOT approved case), "Checked bag, FAA chart" (not allowed; "The two sources differ."), "Current DOT permit: not confirmed here." Alt text rewritten to say the same |
| F2 | Keep the limit that no current DOT permit was confirmed; do not state that the checked-bag exception applies today | Kept in four places: lead ("could not confirm a current DOT permit, so it does not say whether that exemption applies today"), table row 2 ("A current DOT permit was not confirmed"), the bold "What this article could not confirm" paragraph (now also says it does not say whether the exemption applies today), and the diagram and alt. The body still does not explain how the exemption works |
| F3 | Scope the TSA officer final-decision wording to the security checkpoint | Diagram footer: "The TSA officer decides at the checkpoint whether an item is allowed through." Alt ends "The TSA officer decides at the checkpoint." Body section: "...whether an item is allowed through the checkpoint. That statement is about screening at the security checkpoint." |
| F4 | Make the first answer and the table concise; show the common disposable and Zippo-type FAA carry-on guidance first; make the source difference for checked bags clear | Lead rewritten: the FAA carry-on guidance first, then TSA carry-on, then the checked-bag difference in one sentence. Table columns reordered to FAA first, TSA second; the disposable and Zippo-type row is split into "carry-on" and "checked bags" so the difference is visible row by row. The "Disposable and Zippo-type lighters" section now opens with the FAA. The checked-bags section says TSA's answer is conditional and the FAA's chart does not allow them, and that the article does not choose between them |
| F5 | Keep the 2013 FAA FAQ out of the body; keep it in the source notes and QA | Not mentioned in the body or the diagram or alt. Source note S8 and the section "The 2013 FAQ and the special permit" above are unchanged. User decision 2026-10-29: the optional one-sentence addition is **not** adopted |

### Re-check against the official pages (2026-10-29, after the edits)

All eight pages were opened again in the built-in browser after the edits and the statements below were tested against their text: TSA disposable and Zippo (Last Updated July 14, 2026), arc and electronic (Nov 4, 2024), lithium battery powered (Oct 10, 2024), torch (Oct 10, 2024), lighter fluid (Oct 10, 2024), each with the line "The final decision rests with the TSA officer on whether an item is allowed through the checkpoint"; FAA PackSafe Lighters (Last updated April 13, 2026); FAA printable chart (opened directly as a PDF, "Updated: 11/14/25", text layer read page by page, lighters row and torch row read); eCFR 49 CFR 175.10 ("up to date as of 10/27/2026", paragraph (a)(2) read). No page changed since Gate 1.

| # | Revised statement | Source | Result |
|---|---|---|---|
| R1 | FAA: disposable and Zippo-type (absorbed liquid and butane) lighters limited to one per passenger in carry-on or on one's person | FAA page; chart | pass |
| R2 | TSA lists "Carry On Bags: Yes" for Disposable and Zippo | TSA page | pass |
| R3 | TSA: checked bags "Yes (Special Instructions)"; lighters without fuel allowed; lighters with fuel prohibited unless they adhere to the DOT exemption, which allows up to two fueled lighters if properly enclosed in a DOT approved case | TSA page | pass |
| R4 | FAA chart lighters row ends with "Not allowed in Checked Bags" | FAA chart (text layer; row also checked on screen in the viewer at Gate 1) | pass |
| R5 | The article could not confirm a current DOT permit | Source note S9 (DOT-SP 14415, third revision April 26, 2013, expiration Feb 28, 2017); no current permit found; TSA and FAA pages do not name one | pass (a stated limit, not a rule claim) |
| R6 | Both list torch lighters as not allowed in carry-on or checked bags | TSA torch page No / No; FAA page "not allowed in the cabin or in checked baggage"; chart "Not allowed in Carry-On or Checked Bags" | pass |
| R7 | Table row 1: FAA one per passenger, carry-on or person; regulation "on one's person or in carry-on baggage only"; TSA carry-on Yes | FAA; eCFR (a)(2); TSA | pass |
| R8 | Table row 2: chart "Not allowed in Checked Bags"; TSA "Yes (Special Instructions)", without fuel allowed, with fuel prohibited unless a DOT exemption applies | FAA chart; TSA | pass |
| R9 | Table row 3 (arc, electronic, other lithium battery): FAA carry-on only, measures against unintentional activation, no recharging; TSA arc page carry-on "Yes (Special Instructions)" / checked No; TSA lithium page carry-on Yes / checked No | FAA; TSA x2 | pass |
| R10 | Table row 4: torch, FAA not allowed in the cabin or in checked baggage; TSA No / No | FAA; TSA | pass |
| R11 | Table row 5: unabsorbed liquid fuel lighters "forbidden" (FAA); regulation: lighters containing unabsorbed liquid fuel (other than liquefied gas) not permitted on one's person, in carry-on or in checked baggage; no TSA page read for this type | FAA; eCFR | pass |
| R12 | Table row 6: regulation: lighter fuel and lighter refills not permitted on one's person, in carry-on or checked baggage; TSA lighter fluid carry-on No, checked No | eCFR; TSA lighter fluid | pass |
| R13 | FAA: when a carry-on bag is checked at the gate or at planeside, any lighter in the carry-on must be removed and kept with the passenger in the cabin | FAA page; chart | pass |
| R14 | FAA's pages do not mention the exemption (web page text and the chart's lighters row contain no mention of an exemption, permit or special instructions) | FAA page; chart | pass |
| R15 | "The final decision rests with the TSA officer on whether an item is allowed through the checkpoint" appears on the TSA pages; the article says this concerns screening at the checkpoint and does not extend it to checked bags or airlines | five TSA pages | pass |
| R16 | TSA's disposable and Zippo page says questions about regulations can be taken to the FAA website | TSA page | pass |
| R17 | TSA page dates: July 14, 2026; Nov 4, 2024; Oct 10, 2024 (three pages) | five TSA pages | pass |
| R18 | Unchanged sections (how many lighters; arc, electronic and lithium battery details; torch description and naming note; unabsorbed liquid fuel and lighter fluid; Sources list) | Gate 1 claims C-series, re-read today | pass |

Result: 18 of 18 revised statements pass as attributed statements. The limits P1 to P4 above remain open and are stated in the article.

### Image and alt text (revised in FIX round 1; superseded by FIX round 2 below: the file checked here was not the file in the repository)

| # | Check | Result |
|---|---|---|
| I1 | Diagram card 1 compared with R1 to R4: FAA one per passenger in carry-on or on one's person; TSA carry-on allowed; TSA checked bag allowed without fuel, with fuel prohibited unless a DOT exemption applies (up to two, in a DOT approved case); FAA chart not allowed; the two sources differ; current DOT permit not confirmed here. Cards 2 to 4 unchanged and match R9, R10, R11 and R12 | pass |
| I2 | Footer: "The TSA officer decides at the checkpoint whether an item is allowed through." matches R15; "One-lighter limit: FAA page and chart"; "Source: TSA, FAA and eCFR pages, read Oct. 29, 2026" | pass |
| I3 | Image viewed after export (1200 x 2901, PNG8, 64 colors, 119,568 bytes): no clipped text, no logo, no photo; the footer line wraps to three lines with a one-word last line ("through."), accepted. Source SVG updated (`assets/raw/lighters-on-a-plane-tsa.svg`, with title element) | pass |
| I4 | Alt text, 497 characters, matches the diagram and the front matter and the in-body image text (same string). It is longer than the first version (462) because it now carries the conditional TSA checked-bag answer and the unconfirmed permit; it can be shortened if Gate 2 asks | pass (note) |
| I5 | Meta description unchanged, 129 characters | pass |
| I6 | Front matter complete; one H1, nine H2 sections plus Sources (the table section is now headed "What the FAA and TSA say, by type of lighter") | pass |

### Still open (reported as is)

- **P1 and P2 remain.** The pages do not reconcile TSA's conditional checked-bag answer with the FAA chart's "Not allowed in Checked Bags", and no current DOT permit was confirmed. The article states both and does not say the exemption applies today.
- Whether TSA's "Special Instructions" for fueled lighters can be met by a traveler today is not something the pages used here establish.

## Gate 2 FIX round 2 (applied 2026-10-29, base `aa72f32`)

| # | Gate 2 instruction | Result |
|---|---|---|
| L1 | The SVG and PNG on GitHub are both the previous diagram; put the corrected files in | **Confirmed.** In commits `318b5b2` and `aa72f32` the repository files were the first diagram (PNG 1200 x 2319, 102,590 bytes; SVG 11,588 bytes; card text "Carry-on: allowed (TSA)..." and footer "The TSA officer makes the final decision."). Cause: the file transfer into the repository folder delivered the earlier version under the reused file name, and round 1's image check (I3, I4) looked at the build folder, not at the repository file, so it described a file that was not the one committed. This was a process error on Claude's side. Fix: the corrected files were written again under new transfer names and read back from the repository (L4) |
| L2 | Show the conditional checked-bag answer (without fuel / with fuel), the difference from the FAA chart, and the unconfirmed current DOT permit in the diagram | Card 1 now reads: "Carry-on bag: FAA: one per passenger, in carry-on or on your person. TSA: allowed." "Checked bag, TSA: allowed without fuel. With fuel, prohibited unless a DOT exemption applies (up to two, in a DOT approved case)." "Checked bag, FAA chart: not allowed. The two sources differ." "Current DOT permit: not confirmed here." Matches R1 to R4 above (re-tested against the pages in round 1; no page changed) |
| L3 | Limit the TSA officer wording to the security checkpoint | Diagram footer: "At the security checkpoint, the TSA officer decides whether an item is allowed through." Alt text ends with the same limit. Body section "The TSA officer" already says the statement is about screening at the security checkpoint. Matches R15 |
| L4 | Open the PNG and SVG as the files that will go to GitHub and compare them with the in-body alt text | Done after the final write, on the repository files: PNG 1200 x 2901, 125,762 bytes, pixel-identical to the rendered image (difference box empty) and viewed; SVG height 1934, 12,980 bytes, 33 text elements, text matches the diagram above. Both carry an embedded provenance manifest added by the transfer (a `caBX` chunk of 5,758 bytes in the PNG, a `<metadata>` block in the SVG); the round 1 line "no embedded metadata" is withdrawn |

Alt text, 521 characters, same string in the front matter and in the body image: "Disposable and Zippo-type: carry-on allowed, one per passenger (FAA)" matches card 1 line 1; "Checked bags: TSA allows lighters without fuel and prohibits fueled ones unless a DOT exemption applies; the FAA chart says not allowed; a current DOT permit was not confirmed" matches card 1 lines 2 to 4; "Arc, electronic and lithium battery lighters: carry-on only" matches card 2; "Torch lighters, liquid-fuel lighters and lighter fluid: not allowed" matches cards 3 and 4; "At the security checkpoint, the TSA officer decides whether an item goes through" matches the footer. The alt is longer than round 1's 462 characters and can be cut if Gate 3 asks.

Process change: every image is now read back from the repository file (size, dimensions, pixel comparison with the render, text of the SVG) before it is committed, and the QA states which file was checked.

## Gate 2 FIX round 3 (base 6415385, 2026-11-04)

Gate 2 result (ChatGPT, user-reported): FIX, one item. Request: in the front matter and body alt, replace `liquid-fuel lighters` with `lighters with unabsorbed liquid fuel`; keep the TSA/FAA checked-bag difference and the "current DOT permit not confirmed" state.

| # | Change | Result |
|---|---|---|
| M1 | Alt text, front matter and body: "Torch lighters, liquid-fuel lighters and lighter fluid: not allowed." became "Torch lighters, lighters with unabsorbed liquid fuel and lighter fluid: not allowed." The string is identical in both places (537 characters; it was 521, so it is longer; flagged for Gate 2 as before). | done |
| M2 | SVG `<title>` (not rendered) also said "liquid-fuel lighters"; reworded to "...torch lighters, and lighters with unabsorbed liquid fuel." The picture itself is unchanged: card 4 already read "Lighters with unabsorbed liquid fuel, and lighter fluid or refills: not allowed (FAA, 49 CFR 175.10; TSA for lighter fluid)." | done |
| M3 | Not changed, as asked: the checked-bag clause ("TSA allows lighters without fuel and prohibits fueled ones unless a DOT exemption applies; the FAA chart says not allowed; a current DOT permit was not confirmed") and the checkpoint sentence. | kept |

**Official pages re-opened 2026-11-04 for the changed clause (built-in browser, page loads).**

| Page | Checked | Result |
|---|---|---|
| FAA PackSafe, Lighters (page shows April 13, 2026) | heading "Unabsorbed liquid (desk/table lighters, antique wick lighters), absorbed liquids, butane (Zippo-type lighters, disposable lighters)"; "Lighters that use liquid fuel, but do not have an absorbent lining, are forbidden."; one-lighter sentence for absorbed liquid and butane lighters | all present, unchanged |
| eCFR 49 CFR 175.10(a)(2) | "Lighter fuel, lighter refills, and lighters containing unabsorbed liquid fuel (other than liquefied gas) are not permitted on one's person or in carry-on or checked baggage." and the one-lighter sentence | both present, unchanged |
| TSA, Lighters (Torch) (Last Updated October 10, 2024) | Carry On Bags: No; Checked Bags: No | unchanged |
| TSA, Lighter (Fluid) (Last Updated October 10, 2024) | Carry On Bags: No; Checked Bags: No | unchanged |

The wording "lighters with unabsorbed liquid fuel" follows the regulation's own phrase; the FAA page says "lighters that use liquid fuel, but do not have an absorbent lining" and its heading says "Unabsorbed liquid". Not re-opened today: the other five pages (TSA disposable/Zippo, arc, lithium; FAA chart), because those statements were not changed.

**Image checks, repository files read back (not the build folder).** `assets/optimized/lighters-on-a-plane-tsa.png` in the repository: 125,762 bytes, 1200 x 2901, opened and read; unchanged since the previous round (the PNG was not regenerated because only the SVG title changed). The repository SVG (13,024 bytes, 33 text elements) was rendered at 1.5x and compared with the repository PNG: same size, largest per-pixel difference 30 of 255, no pixel differing by more than 40. Card text read from the repository PNG: card 1 (carry-on, TSA checked-bag conditional, FAA chart, DOT permit not confirmed), card 2 (arc/electronic/lithium), card 3 (torch), card 4 ("Lighters with unabsorbed liquid fuel, and lighter fluid or refills"), footer (security checkpoint). Each alt clause matches a card. Both files still carry an embedded C2PA provenance block from the file transfer.

## Gate 2 round 4 result (base `51e6a1d`, reported by the user 2026-11-04)

**PASS.** ChatGPT checked the alt text, which now separates lighters with unabsorbed liquid fuel from the other lighter types, and the committed PNG. No change to the article, diagram or alt was requested or made.

Kept open, as the user instructed:

- **P1 stays open.** The difference between TSA's checked-bag answer for disposable and Zippo-type lighters (fuel-free allowed; fueled lighters only under conditions) and the FAA chart's "Not allowed in Checked Bags" is not reconciled by the pages read.
- **P2 stays open.** No current DOT permit or exemption was found or confirmed; the article repeats TSA's one sentence and says it cannot explain it.
- P3 and P4 are unchanged.

Before ready and before publication the mandatory official-page re-check (TSA lighters pages, FAA PackSafe, 49 CFR 175.10) is repeated and recorded; PASS does not replace it. Moving to `ready` and every WordPress step still need the user's approval.

## Not done yet

- Gate 2 round 4 on the revised version (by commit SHA, after the user pushes).
- Fresh re-check of all eight pages before approval and again right before publishing (FAA chart PDF opened directly).
- User approval to move to `content/ready/`; WordPress draft; publishing.

## Pre-ready official-source re-check (2026-11-04, built-in browser; user request before the ready request)

**Result: no change found in any source the article relies on.** Method: each page was opened or fetched in the browser and every statement used in the article (the verbatim anchors in the source notes S1 to S7) was tested by script after whitespace, apostrophe and quotation-mark normalization; page dates were compared with the dates recorded on 2026-10-29. The two TSA checkpoint lines "Carry On Bags: Yes" and "Checked Bags: Yes (Special Instructions)" matched when the colon after the label was allowed for (the first script version omitted it).

| Source | Date now | Date recorded 2026-10-29 | Result |
|---|---|---|---|
| TSA, Lighters (Disposable and Zippo) | "Last Updated on July 14, 2026" | same | all anchors present (carry-on Yes; checked Yes (Special Instructions); fuel-free allowed in checked bags; fueled lighters prohibited unless the DOT exemption, up to two in a DOT approved case; FAA pointer; officer decides) |
| TSA, Lighters (Arc, Electronic, E-Lighters) | "Last Updated on November 4, 2024" | same | all anchors present (carry-on Yes (Special Instructions); checked No; measures against activation and the three examples; 100 Wh and 2 g; no recharging on board) |
| TSA, Lighters (Lithium Battery Powered) | "Last Updated on October 10, 2024" | same | carry-on Yes; checked No |
| TSA, Lighters (Torch) | "Last Updated on October 10, 2024" | same | carry-on No; checked No; the flame description present |
| TSA, Lighter (Fluid) | "Last Updated on October 10, 2024" | same | carry-on No; checked No |
| FAA PackSafe, Lighters | "Last updated: Monday, April 13, 2026" | same | all six anchors present (liquid fuel without absorbent lining forbidden; one lighter limit; gate-check rule; lithium battery lighters carry-on only; no recharging; torch lighters not allowed in the cabin or checked baggage); the page still does not mention the DOT exemption |
| FAA printable chart (PDF, 9 pages) | "Updated: 11/14/25" | same | text layer read with pdf.js: the one-lighter sentence, "Not allowed in Checked Bags" next to the lighter and lithium rows, and the torch lighter row "Not allowed in Carry-On or Checked Bags" present |
| eCFR 49 CFR 175.10 | "up to date as of 11/02/2026" (was 10/27/2026) | 10/27/2026 | the four relied-on strings present and unchanged (one lighter on one's person or in carry-on only; unabsorbed liquid fuel lighters not permitted anywhere; safety cap; no recharging); only the "up to date as of" date moved |

**Open points unchanged.** P1 (TSA's conditional checked-bag answer against the FAA chart's "Not allowed in Checked Bags"), P2 (no current DOT permit or exemption confirmed; the FAA page does not mention it) and P3 and P4 stay as recorded. **As-of date.** The article still says its facts are as of October 29, 2026; nothing changed since, so no body change was made. The as-of date is refreshed at the final re-check right before publishing, which also needs the user's approval of the text change. The ready request is made to the user; the post stays in draft until the user approves the move. No WordPress step.

## Move to `ready` (user approval 2026-11-04)

The user approved moving this article to `ready` on 2026-11-04 after the official-source re-check of the same day (section above: no source changed). The file was moved from `content/drafts/` to `content/ready/` and the front matter set to `status: ready`; the article text, diagram and alt were not changed by the move. The TSA / FAA checked-bag difference (P1) and the unconfirmed DOT permit (P2) stay open as the user instructed; the article keeps stating them as limits.

**Before publishing (the user's condition):** the official sources are re-read right before publication and the result is recorded here; if anything changed, the change is reported first and the text fixed before any upload. The as-of date in the article is refreshed at that re-check, which needs the user's approval because it changes the text. WordPress upload and publication have not been done and need the user's separate approval.


## WordPress draft and final source re-check (2026-11-06)

**Draft created, not published.** On the user's go-ahead of 2026-11-06 the article was uploaded as a WordPress draft: post 78 (draft; edit `https://statesideexplained.com/wp-admin/post.php?post=78&action=edit`, preview `https://statesideexplained.com/?p=78&preview=true`), diagram media 77. Gate 1 and Gate 2 were not repeated (user instruction). The article text is unchanged; the TSA / FAA checked-bag difference (P1) and "current DOT permit not confirmed" (P2) are kept as written. The as-of date in the article is still "October 29, 2026".

**Checks on the draft.** Body hash of the posted content sha256 `a9b5cd485f724bda3891731b9e6244a51fc7e4e7fa6b7a1a0e4120fb368bba76` (13,670 characters, verified against the typed source before posting); image file sha256 `bd4eb08296c150ebd6a6dce86ae0f29b4fae47cd141d7d570c92c708ad46143a` (1200 x 2901, 125,762 bytes) verified after upload; the original file is used in the post (WordPress also made a scaled copy; the post references the original, as for post 72); alt text 537 characters; Rank Math focus keyword "can you bring a lighter on a plane" and description (129 characters) set and read back; comments and pings closed; 38 blocks parse as valid; logged-out request returns 404 and the draft is not in the sitemap.

**Mobile table fix (same as post 75, no text change).** The table block has automatic column widths (`hasFixedLayout` false) and a fluid font size `clamp(12px, 3.6vw, 18px)`. Checked at 375 and 320 px: no word breaks mid-word, no horizontal page overflow, diagram readable. To undo: turn "Fixed width table cells" back on and clear the font size in the block settings.

**Final official-source re-check (2026-11-06) result: no change found.**

| Source | Date now | Recorded | Result |
|---|---|---|---|
| TSA Lighters (Disposable and Zippo) | "Last Updated on July 14, 2026" | same | anchors present |
| TSA Lighters (Arc, Electronic, E-Lighters) | "Last Updated on November 4, 2024" | same | anchors present |
| TSA Lighters (Lithium Battery Powered) | "Last Updated on October 10, 2024" | same | anchors present |
| TSA Lighters (Torch) | "Last Updated on October 10, 2024" | same | anchors present |
| TSA Lighter (Fluid) | "Last Updated on October 10, 2024" | same | anchors present |
| FAA PackSafe, Lighters | "Last updated: Monday, April 13, 2026" | same | liquid-fuel, one-lighter, gate-check, lithium and torch sentences present; the page still does not mention the DOT exemption |
| FAA printable chart (PDF, 9 pages) | "Updated: 11/14/25" | same | text layer read with pdf.js: one-lighter sentence, "Not allowed in Checked Bags" in the lighter rows, torch row present. The file's server Last-Modified header is May 14, 2026, but its printed date and the relied-on text are unchanged; file hash 6638585a... (758,737 bytes) recorded as the new baseline |
| eCFR 49 CFR 175.10 | "up to date as of 11/04/2026"; Title 49 last amended 10/28/2026 | 11/02/2026; 10/13/2026 | the four relied-on strings present and unchanged; only the dates moved |

The user presses Publish. After publication: live QA and records.


## Pre-publication re-check and publication (2026-11-06)

**Standing instruction (user, 2026-11-06):** for articles that passed review, check the official sources right before publishing and publish if nothing changed, then do live QA and records; report first if official content changed or a significant source conflict appears. Applied here; the user asked specifically that the article be published only if the re-check found no change and the TSA / FAA checked-bag difference and the unconfirmed DOT permit remained stated.

**Re-check (about 07:00 UTC, second check of the day):** no change in any source. TSA five pages: dates July 14, 2026 (disposable and Zippo), Nov 4, 2024 (arc and electronic), Oct 10, 2024 (lithium battery powered, torch, lighter fluid); all anchors present (7 of 7, 7 of 7, 3 of 3, 5 of 5, 3 of 3), the torch page still does not use the word butane. FAA PackSafe Lighters "Last updated: Monday, April 13, 2026", 6 of 6 anchors, still no mention of the exemption. FAA chart PDF: 9 pages, "Updated: 11/14/25", file sha256 6638585a... (758,737 bytes) identical to the 2026-11-06 morning read, one-lighter sentence, "Not allowed in Checked Bags" (11 occurrences) and torch row present. eCFR 49 CFR 175.10: "up to date as of 11/04/2026", Title 49 last amended 10/28/2026, the four relied-on strings present. No source conflict beyond the recorded P1 and P2.

**Draft check:** post 78 still draft and unmodified since 2026-11-05 20:05 (site time); the plain text of the saved content equals the repository article text (9,442 characters, sha256 b269d520...1965); 38 blocks; table block with automatic widths and font size clamp(12px, 3.6vw, 18px); image block id 77 pointing to the original file (sha256 bd4eb082...6143a, 125,762 bytes), alt 537 characters; comments and pings closed; category Airport security rules. The article text contains "For checked bags the two differ" (TSA conditional answer against the FAA chart's "Not allowed in Checked Bags") and "This article could not confirm a current DOT permit, so it does not say whether that exemption applies today"; the as-of date stays "October 29, 2026" (user decision).

**Publication:** published by Claude on 2026-11-06 at 07:12:48 UTC (site local time 02:12) by a REST status change on post 78.

## Live QA after publication (2026-11-06)

| Check | Result |
|---|---|
| URL https://statesideexplained.com/lighters-on-a-plane-tsa/ | 200 |
| Title, H1 | "Can You Bring a Lighter on a Plane? What TSA and the FAA Say" (title tag adds " - Stateside Explained") |
| Canonical, og:url | the post URL |
| Meta description (129 characters), og:description | same text |
| Robots | index, follow, max-snippet:-1, max-video-preview:-1, max-image-preview:large |
| og:image | the diagram file |
| JSON-LD | Person, Organization, WebSite, ImageObject, WebPage, BlogPosting |
| Comment form, pingback link | none |
| Diagram | original file; read back with sha256 bd4eb082...6143a; alt text 537 characters |
| Links | one internal link (/power-bank-on-a-plane-tsa-faa/, opens, 200); eight official links (five TSA, FAA page, FAA chart, eCFR) in new tabs with rel noopener |
| Headings and table | ten H2 including Sources, one table; the TSA / FAA checked-bag sentence, the DOT permit sentence and the as-of date "October 29, 2026" present in the live text |
| Phone width (375 px) | no horizontal overflow, no broken words in the table, diagram loaded and readable |
| Post sitemap | listed, lastmod 2026-11-06T07:12:48+00:00 (17 URLs in the post sitemap) |
| RSS feed and home page | the post is listed in both |

No indexing request was made (user rule). Result: **live QA passed.** Note: the article's as-of date is October 29, 2026 while the sources were re-read on November 6, 2026 (the change would be a text change; the user chose to keep October 29).
