# QA — USPS Registered Mail

Article: `content/drafts/usps-registered-mail-how-it-works.md` (draft, 2026-11-24, about 1750 words in the body, one H1, Sources included; meta description 141 characters; alt text 1237 characters).

Stage: draft. Gate 1 (Claude) run on 2026-11-24 on the rewritten article. Gate 2 not yet run. Backlog row 46.

## Handed-over draft
The first draft came in a bundle (commit `6e09600`, another environment). Its brief and QA said factual QA was incomplete. The article here was rewritten after Claude read the live pages; every claim below was tested against them.

## Gate 1 — claim groups
- FAQ 000006061 (May 14, 2025): 35 of 37 phrases, 2 table-spacing artifacts.
- DMM 503.2.1 to 2.5: 43 of 44 phrases, 1 my typo.
- FAQ 000007968 (May 19, 2026), Domestic Registered Mail row: 5 of 5.
- Dollar limits, fees and the cash threshold amount are in the sources and deliberately left out.
- Return Receipt post (WP 174) was a 404 on 2026-11-24 (scheduled for 2026-11-25 15:00 KST): confirm it is public before this post is published; otherwise remove that one link. The other four internal links returned 200.
- Certified Mail post says it does not compare Certified Mail with Registered Mail; this article does not compare either.

## Where the pages differ (shown in the article, not resolved)
- The word "receipt": mailing receipt (PS Form 3806) against the internal system of receipts, which the FAQ says is not readily available.
- Eligible classes: four in the FAQ text; the DMM points to exhibit 1.4 (not read).
- How soon to ask about a missing item: 14 or more days (Missing Mail FAQ) against 15 days (DMM, no declared value); different procedures, relation not stated.

## Image checks
PNG 1200 x 3165 px, 601,820 bytes, SHA-256 prefix `19deb80b13b60f6f`; SVG 6,045 bytes, `ac99f8c26c64fc38`; md 14,001 bytes, `1d10c1707fbfc58e`; C2PA chunk and metadata stripped on the device (hashes equal the originals). The rendering script printed no text past the right margin; the PNG was viewed. Diagram text only repeats facts from the article; alt text matches the front matter and the Markdown alt text. No dollar sign or percent sign in the article.

## Not checked
Search volume; any page not listed in the source notes; WordPress (no draft or schedule exists); mobile and editor checks (after Gate 2 PASS).
