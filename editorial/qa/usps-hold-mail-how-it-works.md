# QA record — usps-hold-mail-how-it-works

Article: `content/drafts/usps-hold-mail-how-it-works.md`
Brief: `research/briefs/usps-hold-mail-how-it-works.md`. Sources: `research/sources/usps-hold-mail-how-it-works.md` (S1 USPS "Hold Mail", S2 USPS FAQ "USPS Hold Mail - The Basics", S3 USPS "Standard Forward Mail & Change of Address").
Stage: draft written 2026-10-07; Gate 1 done by Claude on 2026-10-07. Not sent to Gate 2, not approved, not on WordPress, not published.

Method: the three USPS pages were opened again in the built-in browser on 2026-10-07; their full text was read (the FAQ's collapsed sections from the page content), and after the draft was written the quoted statements were tested by script against the page text (6 phrases on S1, 26 on S2, 3 on S3): all present. This is the drafting and factual-QA re-check required for rule posts; the re-check right before the user approves moving to `ready` and again right before publishing is still **mandatory**; if a page cannot be opened, do not publish.

## Gate 1 — Factual QA (claim by claim)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | USPS Hold Mail holds your mail at your local Post Office until you return, for a minimum of 3 days and a maximum of 30 days | S1-1 | pass (attributed) |
| C2 | The USPS FAQ calls it a free service that pauses all mail delivery to an address | S2-1 | pass (attributed) |
| C3 | Wording as of October 7, 2026; three USPS pages; no advice on whether to use it | Browser reads; scope | pass |
| C4 | The FAQ says Hold Mail pauses all mail delivery, letters and packages, for all individuals at the address; it cannot be used to hold a single package or specific mail items | S2-1, S2-2 | pass (attributed) |
| C5 | USPS's forwarding page describes Hold Mail as a way to "pause" all mail delivery if you will be away for 3 to 30 days | S3-1 | pass (attributed; one quoted word) |
| C6 | A hold must be for at least 3 days and no more than 30; longer than 30: USPS says to sign up for a forwarding service | S1-1, S1-2, S2-7 | pass (attributed) |
| C7 | At least 3 days must pass between one hold period and the next; the example: a person at the end of a 30-day hold can ask for another one on the 31st day, but it takes effect after 3 days | S2-7 | pass (attributed) |
| C8 | The Hold Mail page says the online process requires creating or signing in to a USPS.com account and verifying identity; once verified, the step is not repeated for the current address | S1-5 | pass (attributed) |
| C9 | An online request can be made up to 30 days in advance or as early as the next scheduled delivery day | S1-3, S2-3 | pass (attributed) |
| C10 | FAQ: an online request submitted before 2:00 a.m. Central Time can begin on the same postal business day; one submitted after can begin on the next postal business day at the earliest | S2-4 | pass (attributed) |
| C11 | The Hold Mail page gives the same cutoff as 3 AM Eastern (2 AM Central or 12 AM Pacific) on the requested day | S1-4 | pass (USPS's own parenthetical equates 3 AM ET with 2 AM CT) |
| C12 | Postal business days are Monday through Saturday, except postal holidays | S2-4; S1-4 (Monday-Saturday) | pass (attributed) |
| C13 | The confirmation number for an online request is emailed; with it a request can be edited, changed or canceled | S2-6 | pass (attributed) |
| C14 | Online submission is not available at all addresses; where unavailable the request must be made in person at a local Post Office with PS Form 8076, Authorization to Hold Mail | S2-5 | pass (attributed) |
| C15 | On the last day USPS delivers all your mail or you can pick it up at the local Post Office; the choice is made when submitting the request | S2-8; S2 "How do I get mail when my request ends" (options "When submitting your request") | pass (attributed) |
| C16 | If you choose pickup: within 10 days or returned to the senders; acceptable ID required; regular delivery resumes the next postal business day after an in-person pickup; picking up earlier than the requested date cancels the hold | S2-9, S2-10 | pass (attributed) |
| C17 | If you choose carrier delivery and nobody is home, only the mail that fits the receptacle is delivered; overflow: PS Form 3849 left and the mail returned to the local Post Office for pickup | S2-8 | pass (attributed) |
| C18 | Scope: no holds for single packages or "held for pickup" (described separately by USPS), no authorizing others, change of address effects, PO boxes, business or military mail; no theft or safety advice | S2 overview; scope statement | pass (scope) |
| C19 | Sources: all three checked October 7, 2026; the FAQ shows Sep 16, 2026; the other two show no update date | Browser reads | pass |
| C20 | Source titles and URLs | Page titles: "Hold Mail - Pause Mail Delivery Online \| USPS", "USPS Hold Mail - The Basics", "Standard Forward Mail \| USPS" | pass |

### Image (`assets/optimized/usps-hold-mail-how-it-works.png`, original SVG in `assets/raw/`)

- Own four-step timeline, no photos, no USPS logo, no mailbox or carrier. 1200x2667. Every line traces to the claims above: "Online: sign in to USPS.com and verify your identity. Up to 30 days ahead, or as early as the next scheduled delivery day." (C8, C9); "Same-day start: request by 2:00 a.m. Central Time (USPS FAQ). Postal business days: Monday to Saturday, not holidays." (C10, C12); "USPS holds all mail at your local Post Office. Longer than 30 days: USPS points to a forwarding service. At least 3 days between holds." (C4, C6, C7); "The carrier delivers your held mail, or you pick it up at the Post Office. Pickup: within 10 days, or the mail is returned to the senders." (C15, C16); "Source: USPS pages, read Oct. 7, 2026" (C19).
- Alt text in the front matter and the body is identical (about 410 characters; it shortens the diagram's wording).
- File check on the device: pixel hash of the PNG matches the cloud render (md5 of RGB bytes c75043f7...). Visual check of the render: no text overflow.

### Handled by wording

- Every rule statement is attributed to USPS ("USPS says", "the FAQ says"); the cutoff is given in USPS's two forms and the article says which page states which.
- "Free" is attributed to the FAQ, as the brief required.
- No home-safety or theft advice; no recommendation.

### Not verified

- Which addresses are not eligible for online submission (USPS does not list them; the article says only what USPS says).
- The FAQ sections not used (authorizing someone else, effect of a change of address, identity problems, technical help).
- Whether the cutoff or limits change after today (the mandatory re-check covers this).
- Search volume and competition for the focus keyword (not measured; third-party pages rank ahead of USPS's).
- The exact diagram text size on a real phone (to be checked in the WordPress preview).

### Re-check obligations

**Mandatory**: re-read S1, S2 and S3 right before the user approves moving the article to `ready`, and again right before publishing. Compare the numbers (3 days, 30 days, 3 days between holds, 2:00 a.m. Central Time, 3 AM ET, 10 days), the account and identity requirement, the in-person route and the FAQ page date. If a page differs or cannot be opened, return to draft or do not publish.

## Gate 2 (ChatGPT, 2026-10-07, result reported by the user)

**PASS.** No changes requested. The mandatory re-check of the three USPS pages before the move to `ready` and again before publishing still applies. Publish order: this article goes live before `usps-mail-forwarding-how-long`, which links to it.

## Gate 2 final (ChatGPT, 2026-10-07)

**Gate 2 final PASS** (the original review result stands; no changes were requested).

## Mandatory pre-approval re-check (2026-10-07)

Before asking for the ready-move approval, the three USPS pages were opened again in the built-in browser and their text tested by script (strings normalized for case, quotes, registered marks, asterisks and spacing; the FAQ's collapsed sections tested from the page content after a 5-second wait):

| Page | Strings tested | Present |
|---|---|---|
| S1 USPS "Hold Mail" (https://www.usps.com/manage/hold-mail.htm) | 6 (3 to 30 days, longer: forwarding, 30 days in advance, 3 AM ET / 2 AM CT / 12 AM PT cutoff, account and identity verification, verification not repeated) | 6 of 6 |
| S2 USPS FAQ "USPS Hold Mail - The Basics" | 29 (free service and 3 to 30 days, last-day delivery or pickup, no single package, who may submit, online account, 2:00 a.m. Central Time cutoff, Monday to Saturday, PS Form 8076, online not available at all addresses, confirmation number, 3 days between holds with the 31st-day example, pickup within 10 days, ID for pickup, regular delivery after pickup, receptacle limit, PS Form 3849, early pickup cancels the hold, "when submitting your request", page date Sep 16, 2026) | 29 of 29 |
| S3 USPS "Standard Forward Mail" (https://www.usps.com/manage/forward.htm) | 3 (3 to 30 days "pause", the Post Office holds all mail, the carrier delivers on the last day or you pick it up) | 3 of 3 |

Result: no difference from the source notes; no article change. The FAQ page date is still Sep 16, 2026. The numbers checked: 3 days, 30 days, 3 days between holds, 2:00 a.m. Central Time, 3 AM ET, 10 days; the account and identity requirement and the in-person route are unchanged. The check is dated the same day as the as-of date in the text (October 7, 2026). Ready-move approval has not been given yet; a fresh read right before publishing is still **mandatory**.

Publish order (Gate 2): this article goes live before `usps-mail-forwarding-how-long`, which links to it.

