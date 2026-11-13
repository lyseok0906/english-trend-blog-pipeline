# Next-article candidates, fifth survey (2026-11-13)

Prepared by Claude at the user's request ("`2a9fee1` is pushed; continue the next-article candidate survey; review two candidates that do not overlap the existing posts, including USPS tracking status help; check the reasons and official sources; take them through draft, diagram and Gate 1 and report the commit SHA"). Two candidates were chosen and drafted: `usps-tracking-status-what-it-means` and `usps-passport-services-what-the-post-office-does`.

## What was and was not measured

Google Trends (US, past 12 months to 2026-11-13, weekly values, 0 to 100, scaled to the highest point inside each comparison of up to five phrases) was read through the explore and widget-data endpoints from a Trends page in the built-in browser. Each comparison contained an anchor ("can you bring a vape on a plane" or a phrase read against it), so each phrase is shown as a multiple of the anchor inside the same comparison; multiples from different comparisons are only roughly comparable, and a small anchor makes a multiple coarse. These are **relative indexes, not search volume. Search volume was not checked** (no keyword tool or Search Console data was available). Official sources were read in the built-in browser on 2026-11-13 and tested again by script at Gate 1. The State Department's passport pages (travel.state.gov) returned a Cloudflare challenge (HTTP 403) and were not bypassed.

## Trends readings (relative index; x vape = multiple of the anchor in the same comparison)

| Phrase | Reading | Note |
|---|---|---|
| usps tracking status | about 1.7 x (average 33.6 against 19.9) | chosen |
| usps in transit; usps out for delivery | about 1.5 x and 1.04 x the tracking-status phrase | covered inside the tracking post |
| usps label created; usps tracking not updating | about 0.38 x and 0.14 x the tracking-status phrase | covered in part; low |
| usps passport | about 22 x (coarse, tiny anchor); about 13 x the tracking-status phrase (average 69.1; maximum 100; last 8 weeks 44.8; no zero week) | highest reading of the survey; chosen |
| usps passport appointment; usps passport photo; renew passport at post office | about 9 x; 1.5 x; 0.9 x | covered inside the passport post |
| usps redelivery | 1.3 x the vape anchor in one comparison; 0.77 x the tracking-status phrase | covered inside the tracking post (notices section) |
| usps money order | about 3.8 x (another comparison) and 2.2 x the tracking-status phrase | not chosen (financial product, price-heavy) |
| usps general delivery | about 0.56 x; 0.34 x the tracking-status phrase | not chosen: low |
| usps smart locker | about 0.04 x | not chosen: low |
| usps tracking number | very high (about 46 against 1 for most phrases) | navigational (people looking for the tracking page); not used as a demand reading |
| usps signature confirmation; usps registered mail; usps delivery time; usps package left at door | about 4.2 (against 19.9); 0.8; 2.5; 0 | low or unclear; not chosen |
| where is my package usps | about 0.65 x (another comparison) | covered by the tracking post |
| tsa medication; tsa breast milk; tsa disability; tsa liquids medically necessary | about 1.9 x (spiky); 0.36 x; 0.41 x; 0.03 x | not chosen: health-adjacent and spiky, or low |

Earlier readings kept: usps return receipt 0.87 x, usps parcel locker 1.5 x, usps return package 1.5 x, usps return to sender 1.1 x, usps free boxes 2.0 x, tsa expired id 0.52 x, tsa id requirements 1.19 x.

## Why these two

- **USPS tracking status.** About 1.7 x the vape anchor, with the related statuses in the same range ("usps in transit" and "usps out for delivery" are of the same order as the main phrase). Two official FAQs are current (Sep 29 and Sep 17, 2026), with an entry for each of 27 statuses. The pages show differences worth showing without any price: "1 full postal business day" against "24 hours", automatic reattempt against "no automatic second delivery attempt", and "will be delivered by a carrier today" against the non-guarantee lines. No overlap with a live post (repo grep: only incidental mentions).
- **USPS passport services.** The highest reading by a wide margin and a plain reader question (can the Post Office do this, and what do I bring). The USPS pages state the role clearly (accepts first-time applications and photos; does not issue passports) and differ in ways that can be shown: "16 or under" against "under age 16", renewal detail on USPS.com against the FAQ's pointer to the State Department, and the appointment and walk-in wording. Every dollar amount on both pages is left out. Caveat: the rules belong to the State Department, whose pages could not be read, so the article attributes everything to USPS and says so. No overlap with a live post (the REAL ID post mentions a passport only as accepted ID).

## Considered and not chosen now

- **USPS redelivery** (0.77 x the tracking-status phrase). Overlaps the tracking post, which covers the Notice Left options.
- **USPS money order** (2.2 x the tracking-status phrase). A financial product whose pages are mostly limits and fees; left out.
- **USPS general delivery** (0.34 x) and **USPS Smart Locker** (about 0.04 x). Low.
- **USPS tracking number.** Navigational demand; the tracking post answers the status question instead.
- **USPS return package and return to sender** (1.5 x and 1.1 x). Returns pages not read; a possible next candidate.
- **USPS free boxes** (2.0 x). A store listing, as recorded on 2026-11-13.
- **TSA medication** (about 1.9 x, spiky) and other TSA phrases. Health-adjacent or low.
- Thanksgiving posts: unchanged. TSA holiday food stays held until a 2026 TSA food notice is read. USPS Thanksgiving waits for the 2026 USPS operating notice (scheduled check 2026-11-14 09:00 KST).
