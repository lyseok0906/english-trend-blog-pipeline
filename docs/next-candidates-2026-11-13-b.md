# Next-article candidates, fourth survey (2026-11-13)

Prepared by Claude at the user's request ("find two candidates that do not overlap the existing 27 posts; compare again the envelope addressing, missing mail and free boxes candidates recorded in `docs/next-candidates-2026-11-13.md`; check search interest and official sources before choosing; take the two chosen through brief, draft, diagram and Gate 1 and report the commit SHA; the two Thanksgiving posts keep their official-notice condition"). Two candidates were chosen and drafted: `usps-missing-mail-search-how-it-works` and `how-to-address-an-envelope-usps`.

## What was and was not measured

Google Trends (US, past 12 months to 2026-11-13, weekly values, 0 to 100, scaled to the highest point inside each comparison of up to five phrases) was read through the explore and widget-data endpoints from a Trends page in the built-in browser. Every comparison contained an anchor phrase ("can you bring a vape on a plane" or a phrase tied to it), so each phrase is shown as a multiple of the anchor inside the same comparison; multiples from different comparisons are only roughly comparable. These are **relative indexes, not search volume. Search volume was not checked** (no keyword tool or Search Console data was available); nothing here estimates monthly searches. Official sources were read in the built-in browser on 2026-11-13 and tested again by script at Gate 1.

## Trends readings (relative index; x vape = multiple of the anchor in the same comparison)

| Phrase | Reading | Note |
|---|---|---|
| how to address an envelope | about 6.2 x (average 57.6 against 9.3; maximum 100; last 8 weeks 50.8; no zero week) | highest evergreen reading; chosen |
| how to address a package | about 3.9 x (average 36.0; maximum 79; last 8 weeks 25.5) | covered inside the envelope post (packages section) |
| usps return address | about 1.2 x | covered inside the envelope post |
| usps missing mail | about 4.5 x (average 42.2; maximum 65; last 8 weeks 30.8) | chosen |
| usps lost package | about 2.8 x (average 61.2 against 21.8; maximum 100; last 8 weeks 61.8) | folded into the Missing Mail post |
| usps missing mail search | about 1.2 x | same topic |
| usps free boxes | about 2.0 x (average 43.7 against 21.8; last 8 weeks 47.6) | not chosen, see below |
| usps parcel locker | about 1.5 x | Smart Locker pages not read |
| usps tracking status; usps in transit; usps out for delivery; usps label created | about 1.7 x; 2.5 x; 1.7 x; 0.63 x (3 zero weeks) | strong candidate, see below |
| usps arrived at hub; usps notice left | about 0.02 x each (48 zero weeks for "arrived at hub") | near zero |
| usps return to sender; usps return package | about 1.1 x; 1.5 x | returns pages not read |
| tsa expired id; tsa id requirements; tsa child id; tsa lost and found | about 0.52 x; 1.19 x; 0.12 x; 0.46 x | see below |

## Why these two

- **How to address an envelope.** The highest evergreen reading of the surveys (about 6.2 x; no zero week) and a plain reader question. The earlier survey held it back because the FAQ "Addressing Mailpieces" mixes consumer guidance with mailer rules; this time five USPS pages were read (the FAQ, the letters page, the address popup, a video transcript and the package page, step 4) and the mailer parts are left out. The pages show real differences that can be shown without a price: "center" against "bottom center", where the apartment number goes, "always use abbreviated locators" against "writing the words is encouraged", and "always use a return address" against "required on certain types of mail". Caveat: none of the five pages has an update date, which the article says. The letters page lists postage prices; none are used. No overlap with a live post (repo grep for address an envelope, return address and how to address found only incidental mentions).
- **USPS Missing Mail search.** About 4.5 x on average, steady rather than seasonal, with the related "usps lost package" at about 2.8 x. Two official pages are current (the FAQ is dated May 19, 2026) and agree on the core rule (7 to 365 days). They differ in ways worth showing: the FAQ's per-service wait table (7 days for Priority Mail Express, 14 for Registered Mail and Parcel Select) against the application's 7-day minimum, the claim timing (USPS.com gives 60 days only for damaged or missing contents of insured mail; the FAQ says "meeting the appropriate timeframe"), and the handgun note. No overlap with a live post (Package Intercept is a different service and is linked, not repeated).

## Considered and not chosen now

- **USPS free boxes** (about 2.0 x, rising). The official surface is a store listing (https://store.usps.com/store/shipping-supplies/free-shipping-supplies/_/N-alnx4j, a product list of items priced $0.00: Priority Mail envelopes, flat rate boxes and similar). There is no rules page, the catalog changes, and the article would be a product list with prices of zero. Re-compared as asked; not chosen.
- **USPS tracking statuses** (1.7 to 2.5 x). The FAQ "Where is my package? Tracking Status Help" (Article 000006077, dated Sep 29, 2026) is a strong, dated source with a "What It Means / What You Can Do" list. A good next candidate; it was not chosen this time because the two above read higher and the status list is long and would need its own table plan.
- **USPS parcel locker** (about 1.5 x). Smart Locker pages not read.
- **USPS return package and return to sender** (about 1.5 x and 1.1 x). Returns pages not read.
- **TSA expired ID, TSA ID requirements** (0.52 x, 1.19 x). Overlap with the live REAL ID post; left out. **TSA child ID and TSA lost and found** (0.12 x, 0.46 x): low.
- **USPS arrived at hub, notice left** (about zero): left out.
- Thanksgiving posts: unchanged. TSA holiday food stays held until a 2026 TSA food notice is read. USPS Thanksgiving waits for the 2026 USPS operating notice (scheduled check 2026-11-14 09:00 KST).
