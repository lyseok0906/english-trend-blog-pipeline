# QA record — usps-tracking-status-what-it-means

Article: `content/drafts/usps-tracking-status-what-it-means.md` (draft, 2026-11-13; about 2,090 body words without the alt text; one H1, nine H2 sections; two tables of 3 columns).
Brief: `research/briefs/usps-tracking-status-what-it-means.md`. Sources: `research/sources/usps-tracking-status-what-it-means.md` (S1 USPS FAQ 000006077, Sep 29, 2026; S2 USPS FAQ 000007991, Sep 17, 2026).
Stage: **draft, Gate 1 done 2026-11-13** (waiting for Gate 2). **Rule-type post: re-read both FAQs before any publish or republish.**

## Scope

What two USPS FAQ pages say about tracking and the 27 listed statuses: limits of tracking, pre-shipment, network scans, Arrived at Post Office, Out for Delivery and the 9 pm rule, Held, No Access, Notice Left, Available for Pickup, returns for address problems, Delivered but not found, the waits before a service request, and what the pages do not say. No prices, international tracking, claims, outcomes of service requests or other carriers.

## Method

After drafting, both pages were opened again in the built-in browser (2026-11-13) and tested by script after normalization: S1 73 of 73 phrases (status-guide slice of the page, after the group headings, 12,060 characters; article number and date present); S2 22 of 22 phrases (article slice 10,770 characters; article number and date present). Absence tests on S1: no "$", no "fee", no "price", no "guarantee"; "1 full postal business day" is not defined; "time limit" appears 5 times and no context has a number. Status count: the list on the page was extracted and counted, 27 statuses in five groups (8, 5, 5, 1, 8). Internal links checked from the live site (logged out): Certified Mail, Hold Mail, Missing Mail, address an envelope, mail forwarding and Informed Delivery return 200 and their titles match the link text; the new slug returns 404 (unpublished, no clash). Front-matter alt equals the body alt (script). Draft has no "$" and no "fee".

## Gate 1 — Factual QA (claim by claim)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | Out for Delivery: prepared for delivery and "will be delivered by a carrier today"; may arrive at a different time or later in the day than regular mail; after 1 full postal business day following the scan, use the tracking number to submit a service request | S1 | pass |
| C2 | USPS Tracking "does not expedite or guarantee delivery"; tracking starts when the sender or shipping partner notifies USPS and ends on delivery or pickup; scan data updated throughout the day; Scan Event Status page | S2 | pass |
| C3 | First-Class postcards, letters and flats not eligible for USPS Tracking; extra services (Certified, Registered) carry barcodes | S2 | pass |
| C4 | Expected Delivery Window is a 2-hour slot and delivery within it is not guaranteed; "Alert" status: check USPS Service Alerts first | S2 | pass |
| C5 | Absence of a delivery scan does not necessarily mean not delivered; contact sender or recipient | S2 | pass |
| C6 | Shipping partner statuses: USPS does not have possession; contact the shipper. Label created / pre-shipment: not yet given to USPS. In Possession of Item: no action needed. Shipment Received, Package Acceptance Pending: container or pallet received | S1 | pass |
| C7 | In Transit, Arrived at and Departed USPS Facility: being processed or transported to the delivering Post Office; scans may repeat on the same or different days; no number of days given | S1 (absence of a number) | pass |
| C8 | Forwarded and Forward Processed: change of address request or wrong Post Office | S1 | pass |
| C9 | Arrived at Post Office: should arrive today or the next postal business day; service request after 1 full postal business day with no change and no delivery | S1 | pass |
| C10 | Delivery Status Not Updated / Awaiting Delivery Scan: no Delivered status by 9 pm local time on the Out for Delivery date; next business day anticipated; service request after more than 1 full postal business day with no delivery | S1 | pass |
| C11 | Held at Post Office, At Customer Request: Hold Mail, Hold for Pickup or Delivery Instructions request; redelivery cannot be scheduled; valid Hold Mail requests handled as instructed; otherwise pick up with photo ID | S1 | pass |
| C12 | First table: No Access (reasons; automatic reattempt next business day); Notice Left x2 (no automatic second delivery attempt; signature needed or no secure place); Available for Pickup (redelivery cannot be scheduled) | S1 | pass |
| C13 | Notice Left options: schedule a redelivery (tracking number or notice barcode; Smart Locker if indicated), pick up (authorized agent, photo ID), request return with the Redelivery application; unclaimed within the time limit goes back; the limit is not given | S1 | pass (absence tested) |
| C14 | No Access: service request if more than 24 hours since the status | S1 | pass |
| C15 | Insufficient Address / No Such Number: returned to the sender; sender reships with new postage | S1 | pass |
| C16 | Delivered: recorded date, time and location; places to check; parcel locker key; building office; service request after more than one postal business day for eligible items | S1 | pass |
| C17 | Second table (waits) repeats C1, C9, C10, C14 and C16 and adds no rule; the guide does not define "1 full postal business day" | S1 | pass (absence tested) |
| C18 | Records: 120 days (USPS Tracking), 1 year (Signature Confirmation), 2 years (several services); text and email updates active 2 weeks; Informed Delivery as another option | S2 | pass |
| C19 | 27 statuses in five groups; the article follows the groups | S1 (counted) | pass |
| C20 | Mail Delivery Standards chart is in "Delayed mail and packages?" (not read) | S2 | pass |

## Image checks

800 px wide SVG, 1200 px wide PNG (scale 1.5), render check printed `[]`, viewed in three crops. Alt text equals the front-matter alt and describes every card. C2PA metadata stripped on the device and the SHA-256 and sizes equal the originals (PNG 533,642 bytes, `b009b0b0…`; SVG 4,284 bytes, `1cb09fde…`). The card on waits is dashed (a hedged statement: "when the FAQ says to ask USPS").

## Format

One H1, H2 sections, two 3-column tables (post-only table font at publishing), prose with a bulleted list only for Sources, meta description 152 characters, focus keyword `usps tracking status` in the title and the first paragraph's topic.

## Open points for Gate 2

- Confirm the paired wording of "will be delivered by a carrier today" with S2's non-guarantee lines does not read as a promise.
- Confirm that the waits table (1 full postal business day against 24 hours) reads as a source difference and not as advice.
- Dated rule post: both FAQs are re-read right before publishing; report before publishing if a status entry, a wait, the notice options or the retention periods changed.
