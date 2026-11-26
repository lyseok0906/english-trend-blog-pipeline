# QA — USPS General Delivery

Article: `content/drafts/usps-general-delivery-how-it-works.md` (draft, 2026-11-24, about 1300 words in the body, one H1, Sources included; meta description 130 characters; alt text 993 characters).

Stage: ready; scheduled (WordPress post 178). Gate 1 (Claude) run on 2026-11-24 on the rewritten article. **Gate 2 round 1 (ChatGPT, base `d955818`, user-reported 2026-11-25): PASS, no FIX**; the diagram was checked for cut-off text (none). Backlog row 45.

## Handed-over draft
The first draft came in a bundle (commit `6e09600`, another environment). Its brief and QA said factual QA was incomplete. The article here was rewritten after Claude read the live pages; every claim below was tested against them.

## Gate 1 — claim groups
- FAQ 000006989 (Aug 4, 2026), read directly: 30 of 30 phrases (purpose and four uses, finding the facility, address format, one facility, restrictions, PO Box suggestion, 30 days, longer hold, 10 and 15 days, free and no application, postmaster, Sunday and holidays).
- DMM 508.6.1 to 6.4: 12 of 12 phrases; the section has no longer-hold sentence and no 10 or 15 day note (checked by text search).
- DMM 508.11.1.1 (Hold Mail, 3 to 30 days): 2 of 2.
- Our PO Box post (line 44) says the DMM lets a postmaster provide general delivery until a box is available: the article attributes that point to our post, not to a page read here.
- Live link texts match titles: PO Box and Hold Mail (both 200 on 2026-11-24).

## Where the pages differ (shown in the article, not resolved)
- Longer hold: FAQ yes (approved by the postmaster), DMM states only 30 days.
- 10 and 15 day note: FAQ only; "a specific address" is not defined.
- Restrict (FAQ) against refuse or restrict (DMM).
- Purposes: four in the FAQ, two in the DMM.

## Image checks
PNG 1200 x 3372 px, 626,986 bytes, SHA-256 prefix `83d9e59e8461c6ab`; SVG 6,073 bytes, `3d81fe8ac9832038`; md 10,352 bytes, `a5ece4039f618178`; C2PA chunk and metadata stripped on the device (hashes equal the originals). The rendering script printed no text past the right margin; the PNG was viewed. Diagram text only repeats facts from the article; alt text matches the front matter and the Markdown alt text. No dollar sign or percent sign in the article.

## Not checked
Search volume; any page not listed in the source notes; WordPress (no draft or schedule exists); mobile and editor checks (after Gate 2 PASS).

## Scheduling record (2026-11-25)
Gate 2 round 1 on `d955818` was PASS (no FIX). Right before scheduling, both sources were read again: FAQ 000006989 still dated Aug 4, 2026, 30 of 30 phrase checks; DMM 508.6.1 to 6.4, 12 of 12, with no longer-hold sentence and no 10 or 15 day note, and 11.1.1 Hold Mail (3 to 30 days) unchanged. No important change, so nothing was reported first. Built from the repository files on `main` (md `a5ece4039f618178`, PNG `83d9e59e8461c6ab`; converted content hash `15b105dd1bafa1ef` equal to the Python reference), media 177 (image 200, hash equal), post 178 created as a draft in category Postal service and stamps, comments and pings closed, Rank Math keyword and description set (130 characters). Editor: 27 blocks, 0 invalid (one table). Preview at 375 px and 320 px: no page overflow, image 315 and 260 px wide, the table fits its figure, one H1. File moved to `content/ready/` with `status: ready`. Scheduled for 2026-11-26 09:00 KST (00:00 UTC; the site, timezone America/New_York, shows 2026-11-25 19:00). Re-read after saving: status future, date_gmt 2026-11-26T00:00:00. Not public yet (public posts: 39 at the time). Live QA is still to be run after the post appears.

## Live QA (2026-11-26, about 09:20 KST, logged out, no cache)
WordPress published post 178 on schedule (date_gmt 2026-11-26T00:00:00, status publish). Result: HTTP 200 at the canonical URL on the first fetch; canonical equals the URL; title as expected; meta description 130 characters; og:title and og:image set; robots `index, follow`; JSON-LD BlogPosting present; one H1; no comment form and no pingback link; image src returns 200 with SHA-256 prefix `83d9e59e8461c6ab` and the 993-character alt; the table is present (1 table); the 30-day wording is present; no dollar sign or percent sign; 2 internal links both 200 (PO Box, Hold Mail); 2 external links `target=_blank rel=noopener`; the URL is in `/post-sitemap.xml`, `/feed/`, the home page and the Postal service and stamps category page; `x-wp-total` is 42.
Note: unlike the two posts of 2026-11-25, the first logged-out fetch returned 200 and no 404 was seen.
