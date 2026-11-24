# QA — USPS General Delivery

Article: `content/drafts/usps-general-delivery-how-it-works.md` (draft, 2026-11-24, about 1300 words in the body, one H1, Sources included; meta description 130 characters; alt text 993 characters).

Stage: draft. Gate 1 (Claude) run on 2026-11-24 on the rewritten article. Gate 2 not yet run. Backlog row 45.

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
