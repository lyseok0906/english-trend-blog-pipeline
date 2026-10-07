# QA record — usps-informed-delivery-how-it-works

Article: `content/drafts/usps-informed-delivery-how-it-works.md`
Brief: `research/briefs/usps-informed-delivery-how-it-works.md`. Sources: `research/sources/usps-informed-delivery-how-it-works.md` (S1 USPS FAQ "Informed Delivery - The Basics", S2 usps.com Informed Delivery page).
Stage: draft written 2026-10-07; Gate 1 done by Claude on 2026-10-07. Gate 2 (English + SEO, ChatGPT): not yet done. Not approved, not on WordPress, not published.

Method: both pages were opened in the built-in browser on 2026-10-07. The user asked for extra FAQ reading before drafting; the FAQ sections Overview, Signing Up / Welcome Letter, Opt Out, Dashboard, Daily Digest and Issues, and Privacy & Security / Missing Mail were read in full from the page text (the source notes list what was not read). After the draft was written, 33 phrases from S1 and 8 phrases from S2 were tested by script against the page text with the ® and ™ marks removed: all true. This is the drafting and factual-QA re-check required for service-description posts. The re-check right before the user approves publishing is still **mandatory**; if a page cannot be opened, do not publish.

## The user's condition for the letter section

The user said: include "why did I get a sign-up letter" only if the USPS FAQ clearly confirms the process, as one short subheading; otherwise leave it out. **Confirmed.** The FAQ describes it twice: the "Welcome Letter" subsection ("A Welcome Letter is sent as a part of our mail-based verification of new Informed Delivery accounts ... If you recognize the account information listed in the letter, no further action is required. If the account was not created by you (or someone in your household), or you do not recognize the masked username or email address, deactivate it by following the instructions in the letter") and the Privacy & Security answer ("I received a letter saying that someone at my home address signed up for Informed Delivery. This letter is sent as a part of our mail-based verification of new Informed Delivery accounts."). The article gives it one subheading, repeats only USPS's statements, and does not print the USPS web address for the unsubscribe step (the letter carries the instructions).

## Gate 1 — Factual QA (claim by claim)

| # | Claim in the draft | Source | Result |
|---|---|---|---|
| C1 | Informed Delivery is a free, optional USPS service that shows digital previews of incoming letter-sized mail and status updates for packages | S1-1, S2-1 | pass (attributed) |
| C2 | USPS says it digitally images the front of letter-sized mail as it runs through automated sorting equipment and uses the images for notifications before the physical mail arrives | S1-2 | pass (attributed) |
| C3 | Wording is as of October 7, 2026 and comes from two USPS pages; the article describes the service and does not recommend signing up | Browser reads 2026-10-07 | pass |
| C4 | USPS says the images show only the exterior, address side of letter-sized mailpieces; its Informed Delivery page describes them as grayscale | S1-3, S2-1 | pass (attributed) |
| C5 | Table, letters: the Daily Digest email shows images of up to 10 pieces; the dashboard has no limit on the number shown and displays mail images for a seven-day period | S1-4 | pass (attributed) |
| C6 | Table, catalogs and magazines: not imaged by USPS's automated equipment, so they do not appear in the email or dashboard | S1-5 | pass (attributed) |
| C7 | Table, packages: status updates for packages arriving at your address and packages you have sent; status updates, not images | S1-3 | pass (attributed) |
| C8 | Notifications are delivered by Daily Digest email, on the online dashboard and in the mobile app | S1-6 | pass (attributed) |
| C9 | The email is sent once a day, typically before 9:00 AM local time, Monday through Saturday; not sent on days with no mail, on Sundays or on federal holidays | S1-6 | pass (attributed) |
| C10 | An account can have only one email address, but multiple accounts can have Informed Delivery for the same address | S1-6 ("can only be sent to one email address per account. However, multiple accounts can have Informed Delivery for the same address") | pass (attributed) |
| C11 | Notifications are for mailpieces arriving soon, not necessarily the same day; USPS asks people to allow several days, up to one week, before reporting a mailpiece as missing | S1-7 | pass (attributed) |
| C12 | Images may not match the mail delivered that day, for example when automated equipment is moved or shut down for maintenance or pieces of mail overlap as the image is taken | S1-8 | pass (attributed) |
| C13 | Available to most residential and PO Box addresses and many business addresses | S1-9 | pass (attributed) |
| C14 | In rare cases a person cannot sign up in an eligible ZIP Code because the mailbox is not uniquely coded; USPS says this is more common in high-density buildings such as apartment buildings and condos | S1-9 ("most addresses are uniquely coded, not all are, especially in high density areas (e.g., apartment buildings or condos)"). "more common" paraphrases "especially" | pass (attributed) |
| C15 | Signing up means creating or using a USPS.com account and verifying your identity | S1-10, S2-3 | pass |
| C16 | If identity cannot be verified online, the person can request a code by mail (USPS says within 3 to 7 postal business days) or verify in person at a Post Office | S1-10 | pass (attributed) |
| C17 | "This article does not walk through the steps." | Scope statement | pass (scope) |
| C18 | USPS says a Welcome Letter is sent as part of its mail-based verification of new accounts; if you recognize the account information, no further action is required | S1-11 | pass (attributed) |
| C19 | If the account was not created by you or someone in your household, or you do not recognize the masked username or email address, USPS says to deactivate it by following the instructions in the letter | S1-11 | pass (attributed) |
| C20 | The instructions use an unsubscribe code printed in the letter, which USPS says is case-sensitive and must be entered exactly as it appears | S1-11 | pass (attributed) |
| C21 | Once the code is submitted, the account is unenrolled and access is disabled; the code expires 90 days after the date of issue, after successful use, or if the profile address is edited | S1-11 ("is unenrolled from Informed Delivery and access is disabled. The unsubscribe code expires 90 days after the date of issue, after successful use or if the associated USPS.com profile address is edited") | pass (attributed) |
| C22 | Scope paragraph (no mobile app features, redelivery, change-of-address features, other notification options or business marketing content; no worth-it judgment; no security advice beyond USPS's pages; no tracking of changes) | Scope statement | pass (scope) |
| C23 | Sources: both checked October 7, 2026; the FAQ shows Sep 30, 2026; the usps.com page shows no update date | FAQ page text "Sep 30, 2026"; usps.com page: no date seen | pass |
| C24 | Source titles and URLs | FAQ article title "Informed Delivery® - The Basics"; usps.com page title "Informed Delivery - Mail & Package Notifications \| USPS" | pass |

### Image (`assets/optimized/usps-informed-delivery-how-it-works.png`, original SVG in `assets/raw/`)

- Own flow diagram, no photos, no USPS logo, no sample mail images or dashboard screenshots. 1200x2325.
- Every sentence traces to the claims above: "A letter-sized mailpiece runs through USPS automated sorting equipment" (C2); "USPS images the address side. It shows only the exterior of the mailpiece (USPS)" (C2, C4); "You see it in: Daily Digest email: up to 10 letters, typically before 9:00 AM local time, Monday to Saturday; Online dashboard and mobile app" (C5, C8, C9); "What is not shown as an image: Catalogs and magazines: not imaged by the equipment. Packages: status updates only" (C6, C7); "A preview is not a delivery date. USPS: allow several days, up to one week, for the mailpiece" (C11). Source line: "Source: USPS websites, read Oct. 7, 2026".
- Alt text in the front matter and the body is identical and describes the diagram's content without repeating the keyword.
- File check on the device: pixel hash of the PNG matches the cloud render (md5 of RGB bytes b0de974c...); the SVG on the device contains the diagram text. Visual check of the render: no text overflow.

### Handled by wording

- The text repeats only USPS statements; there is no advice on what to click, no link to a sign-up or verification page, and the USPS web address for the unsubscribe step is not printed.
- Business-account code rules (shorter expiry in the FAQ) are not mentioned; the 90-day figure is stated only as the unsubscribe code's expiry as USPS gives it for the Welcome Letter.
- The mobile app and Mail Delivery Notifications are named only as out of scope, or as where notifications appear (app), without describing features.

### Not verified

- The FAQ sections not read (see the source notes), including the mobile app section; the article does not describe them.
- The cost question's own answer on the usps.com page (collapsed); "free" is taken from the visible page heading and the FAQ summary.
- Whether identity-verification wording differs for business accounts (not covered).
- Search volume and competition for the focus keyword (not measured; see the brief).
- The exact diagram text size on a real phone (to be checked in the WordPress preview).

### Re-check obligations

**Mandatory**: re-read S1 and S2 right before the user approves moving the article to `ready` and again right before publishing. Compare the numbers (10 pieces, seven days, 9:00 AM, 3 to 7 postal business days, 90 days, one week), the Welcome Letter wording and the FAQ page date. If a page differs or cannot be opened, return to draft or do not publish.

## Gate 2 — English + SEO QA

Not done yet. To be run by ChatGPT on the commit that contains this draft.
