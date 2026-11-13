# Next-article candidates, third survey (2026-11-13)

Prepared by Claude at the user's request ("TSA and airport security and USPS; no overlap with the 25 live posts; find reader questions, check interest and official sources; pick two; draft, diagram, Gate 1; report the commit SHA; the two Thanksgiving posts keep their 2026-notice condition"). Two candidates were chosen and drafted: `tsa-locks-checked-bag-what-tsa-says` and `usps-holiday-shipping-deadlines-2026`.

## What was and was not measured

Google Trends (US, past 12 months to 2026-11-13, weekly values, 0 to 100, scaled to the highest point inside each comparison of up to five phrases) was read through the explore and widget-data endpoints from a Trends page in the built-in browser. Every comparison contained the anchor phrase "can you bring a vape on a plane", so each phrase is also shown as a multiple of the anchor inside the same comparison ("x vape"). These are **relative interest indexes, not search volume**. No tool in this setup gives search volume (no keyword-volume tool, no Search Console data for topics without a page), so **search volume was not checked** for any candidate. For the holiday phrase a daily series for Oct. to Dec. 2025 was also read to see the seasonal shape.

## Trends readings (relative index; x vape = multiple of the anchor in the same comparison)

| Phrase | Reading | Note |
|---|---|---|
| tsa lock | about 7.4 x vape (average); last 8 weeks about 3.5 x | spiky, maximum 100 |
| tsa locks | about 1.6 x | |
| tsa approved lock | about 0.64 x | |
| tsa recognized lock | 0 | official term, not searched |
| tsa lost and found | about 0.47 x | |
| tsa claim | about 0.69 x | spiky; last 8 weeks low |
| tsa pets; tsa baby formula | about 0.25 x; about 0.23 x | |
| tsa stroller; ssss on boarding pass | about 0.45 x; about 0.5 x | ssss overlaps health-adjacent and ID topics; left out |
| tsa pat down; can you bring a knife on a plane | about 0.07 x; about 0.05 x | |
| can you bring a cooler / a drone on a plane; tsa wrapped gifts; tsa snow globe | 0 or near zero | |
| how to address an envelope | about 6.2 x (average 57.6 against 9.3; no zero week) | highest evergreen reading; see not chosen |
| how to address a package; usps return address | about 3.9 x; about 1.24 x | |
| usps missing mail | about 4.5 x (last 8 weeks 30.8 against 8.6) | see not chosen |
| usps missing mail search; usps lost package claim | about 1.2 x; about 0.7 x | |
| usps free boxes | about 2.0 x (average 46.3 against 23.2; no zero week; rising; last 8 weeks 50.3) | official page not located |
| usps parcel locker; usps redelivery; usps return receipt; usps general delivery; usps mail theft | about 1.5 x; 1.3 x; 0.87 x; 0.56 x; 0.37 x | |
| usps holiday shipping deadlines | average about 0.28 x over 12 months; 45 zero weeks; maximum 59 to 100 | seasonal; last 8 weeks about 0.3 in absolute index |
| usps shipping deadlines | about 0.39 x average, maximum 100 | seasonal |
| usps last day to ship christmas; usps christmas shipping deadline | average 1.2; 0.4 | |

Seasonal shape of the holiday phrases (daily series, Oct. to Dec. 2025): little interest until about Nov. 17, then a ramp and a peak from Dec. 13 to 19 (about 40 to 55 for "holiday shipping deadlines" and up to 100 for "usps shipping deadlines", against an anchor of 0 to 28). The 2026 curve is not known; this is last year's shape.

## Why these two

- **TSA locks and checked bags.** "tsa lock" is about 7.4 times the anchor on average and the question is practical and tied to holiday travel. All three TSA pages are official and plain (Security Screening, Travel Tips, Claims). No overlap with a live post (repo grep for recognized lock, Travel Sentry, Safe Skies, master key and luggage lock found nothing). The pages show a real wording tension ("may not have to be cut" against "will be forced to remove"), shown without being resolved. Claims pages bring the airline-or-TSA split. No prices needed.
- **USPS 2026 holiday shipping deadlines.** The average is the weakest of the candidates, but the interest is seasonal and the 2025 daily series ramps from mid-November, so a post published now can be indexed before the peak. Three official sources agree on every date (USPS.com page, Sept. 22 release, Oct. 14 FAQ) and differ only in footnotes (refund wording, a Priority Mail Express 1-Day note, "customs delays"); no prices. The USPS Thanksgiving brief lists holiday deadlines as out of scope, so the two do not overlap. Dated content: re-read right before publishing.

## Considered and not chosen now

- **How to address an envelope or package** (about 6.2 x and 3.9 x; highest evergreen interest). The USPS FAQ "Addressing Mailpieces" is partly mailer-oriented (automation barcode area) and was read only partly; a good next candidate once the consumer-relevant parts are separated.
- **USPS missing mail** (about 4.5 x). Official process pages (Missing Mail search, claims) were not read; likely next candidate; may overlap price-driven claim questions.
- **USPS free boxes** (about 2.0 x, rising). The official page was not located (the guessed URL returned 404); the topic is likely tied to a promotion page that may change.
- **USPS parcel locker** (about 1.5 x). Needs the Smart Locker pages; not read.
- **TSA claim and TSA lost and found** (about 0.69 x and 0.47 x). Partly covered by the locks article's claims section; lost and found could be a separate short post.
- Low or near-zero readings (TSA pets, baby formula, stroller, knife, pat down, cooler, drone, wrapped gifts, snow globe) and health-adjacent or ID topics (ssss on boarding pass) were left out.
- Thanksgiving posts: unchanged. TSA holiday food stays held until a 2026 TSA food notice is read. USPS Thanksgiving waits for the 2026 USPS operating notice (scheduled check 2026-11-14 09:00 KST).
