# Decision Log

Dated record of decisions about how this blog is run, and why. Append new entries at the
bottom; do not rewrite past entries. If a decision is reversed, add a new entry that says
so and references the original date.

This log covers the English trends blog only. Decisions about the Excel blog or the
Korean economic blog belong in their own repositories.

---

## 2026-09-28 — Editorial operating baseline established

**Context.** The repository existed with an initial commit
(`10eccf1 chore: initialize English trends blog pipeline`) but no operating rules,
documentation, or folder structure. Before any article work begins, the operating model
needed to be fixed in writing so that three parties — Cowork, ChatGPT, and the user —
work from the same rules.

**Decisions.**

1. GitHub `main` is the single source of truth for this project.
2. Cowork researches, drafts, updates QA documents, and creates local commits. It is the
   only writer in this repository.
3. ChatGPT provides editorial direction, SEO / search-intent review, and US-English QA,
   and does not overwrite repository files. This is an operating rule chosen to avoid
   version conflicts between two assistants, not a tooling limitation.
4. The user reviews changes and performs the final `git push`.
5. No WordPress publishing or other public release without explicit human approval for
   the specific article. Blanket project approval does not substitute.
6. Every article follows a fixed sequence: topic brief → evidence / source review →
   draft → factual QA → English + SEO QA → ready → publish approval. Each stage has a
   required artifact and no stage is skipped or reordered.
7. The Excel blog (`excel-data-cleanup-pipeline`) and the Korean economic blog
   (`economic-blog-pipeline`) stay completely separate from this project.

**Written in this round.** `README.md`, `AGENTS.md`, `docs/operating-model.md`,
`docs/content-backlog.md`, `docs/decision-log.md`, `config/editorial-policy.md`, the
`content/` `research/` `editorial/` `assets/` subfolders with `.gitkeep`, and `.gitignore`.

**Deliberately not done.** No article draft was created, and nothing was pushed. Both
were out of scope for this round.

**Open items.**

- The topic selection framework for the first English trend article is not yet agreed.
  `docs/content-backlog.md` is intentionally empty until it is.
- Platform for this blog (WordPress or other) is not decided in this repository yet.

---

## 2026-09-28 — Conditional niche decision recorded, 14-day proof gate created

**Context.** With the operating baseline in place, the next question was the blog's actual
subject area. "Trends" is a format, not a niche, so no topic backlog could be built until a
vertical existed. Rather than confirm a vertical on the strength of an argument, the user
required a proof gate first.

**Decisions.**

1. **Candidate vertical: workflow automation for small teams.** Recorded as conditional, not
   confirmed. See `docs/niche-decision.md`.
2. **Trend handling: hook only.** A trend supplies the title and the opening; the body is
   evergreen problem-solving that still gets searched months later.
3. **n8n is a first-tool pilot, not the site identity.** The domain, site name and category
   structure carry no tool name, and no single-tool affiliate program is joined.
4. **Company, development and QA material are out of scope** for this blog — including
   anonymized or generalized work-derived cases. Positioning toward QA or operations teams is
   also out of scope and was removed from the niche documents.
5. **Local tool folders are not evidence of operator expertise.** An earlier revision of the
   niche comparison inferred expertise from installed tool folders; that reasoning is
   withdrawn. Capability is established only by reproduced evidence.
6. **External AI Overviews CTR figures are directional reference only,** not grounds for a
   niche decision. The −89% news figure in particular is one publisher's self-reported number
   relayed through secondary coverage. The basis for this blog's direction is this project's
   own measured history.
7. **A 14-day proof gate must pass before any backlog work.** Three reproducible workflows
   (webhook → normalization → output; scheduled check → change detection → notification;
   failure handling / retry / diagnosis), each with screenshots, sanitized exported JSON, a
   real failure case, and a verified fix. Run locally with no production credentials and
   synthetic data only. See `docs/proof-gate-n8n.md`.
8. **GO requires three pass/fail tests**, so that "can reproduce, explain and diagnose
   independently" is falsifiable: T1 unaided rebuild within 40 minutes; T2 explanation **in
   Korean** with three unscripted follow-up questions per workflow and zero technical errors;
   T3 diagnosis of a pre-broken workflow from the error message alone within 30 minutes. All
   three must pass. Extensions are not automatic.
9. **Prohibited until the gate passes:** article writing, publishing, affiliate enrollment,
   niche confirmation, backlog entries, scope changes to `README.md` or
   `docs/operating-model.md`, domain purchase, site creation.

**Revisions applied in this round at the user's direction.** The candidate vertical was
renamed from "workflow automation for QA and operations teams" to "workflow automation for
small teams"; QA and operations-team positioning was removed from the niche documents; T2 was
changed from an English-writing test to a Korean technical-explanation test, and its
unverifiable "not LLM-generated" requirement was dropped.

**Written in this round.** `docs/niche-decision.md`, `docs/proof-gate-n8n.md`, and this entry.

**Deliberately not done.** No article or brief was written. `README.md`,
`docs/operating-model.md` and `docs/content-backlog.md` were not changed. Nothing was pushed.

**Open items.**

- **A NO-GO result has no successor vertical.** The former fallback (a QA automation vertical
  based on Playwright / Android testing evidence) is void under decision 4. Left as a user
  decision.
- **The technical-depth boundary is undefined.** Decision 4 excludes development material
  while the candidate vertical still involves technical mechanics. Where the line falls needs
  to be stated before the first topic brief.

---

## 2026-09-28 — Correction: document scope cleanup

Correction entry. Earlier entries are left as written.

Cross-project references were removed from active policy and proof-gate documents.
Hidden-discovery wording was removed from W1 because the cases are intentionally disclosed.

**Files affected.** `docs/niche-decision.md`, `docs/proof-gate-n8n.md`.

**W1 is judged on three things**, recorded here so the criterion is unambiguous:

1. Whether the difference between `null`, an empty string and a non-breaking space is
   explained and handled from actual run results.
2. Whether the required-field validation step was built by the operator and the invalid path
   proven — a missing field does not fail an execution on its own.
3. Whether results that contradicted expectations are recorded rather than quietly fixed.

Detection of an undisclosed defect is measured by T3, which is sealed, and is not duplicated
in W1.

---

## 2026-10-06 — Direction change: n8n proof gate stopped, initial 4-week pilot scope adopted

Earlier entries are left as written.

**Context.** The 2026-09-28 conditional niche (workflow automation for small teams) depended
on a 14-day proof gate that was recorded as `NOT STARTED` and never returned a result. The
user then moved to a different direction, tested it with one unpublished trial article
(Meta Muse; see `docs/blog-c-trial1-record.md`), answered "no" to writing similar posts, and
confirmed the reason: the single AI-agent topic did not match their interest or their
original idea of covering several light keywords. That answer did not judge whether the
blog's operating method itself fits. Lane comparisons followed (`docs/blog-c-lanes-planning.md`
and further lane research kept outside this repository).

**Decisions.**

1. **The n8n / workflow-automation direction is stopped.** The proof gate is not started or
   resumed. `docs/niche-decision.md` and `docs/proof-gate-n8n.md` are marked
   `SUPERSEDED / STOPPED` and kept as history. The "prohibited until the gate passes" list
   (decision 9 of the 2026-09-28 niche entry) no longer applies as a gate condition.
2. **Initial pilot scope: three lanes**, each marked "want to continue" by the user:
   US dates, seasons and holidays; airport security rules; postal service and stamps. The
   user's confirmation rule (at least two different lanes marked "want to continue") is met.
3. **Site promise: "Everyday U.S. Questions, Explained Simply."**
4. **Pilot design: first 4 weeks, target 12 posts, 3 posts per week, daylight saving time
   first** (it ends November 1, 2026). Sustainability of this pace for this lane combination
   is not verified; it is evaluated after the 4 weeks, and no 12-week plan is made before
   then.
5. **This is not a permanent niche confirmation.** The active standard is
   `docs/blog-c-site-structure.md`, with status `ACTIVE — initial 4-week pilot scope`.
6. **Rule-type posts (airport security, postal) must be re-checked against the official page
   right before drafting and again right before publishing.** If the page cannot be opened,
   the post is not published.
7. **Excluded from the initial scope:** K-pop (copyright and publicity-rights dependence, an
   operating criterion and not a legal finding), viral video memes (failed source and image
   verification), weather-alert terms (definitions tie directly to immediate safety actions),
   and health, investment, legal and election-procedure topics.

**Written in this round.** `docs/blog-c-site-structure.md` (new), status banners on
`docs/niche-decision.md` and `docs/proof-gate-n8n.md`, the placeholder row in
`docs/content-backlog.md`, one row in the `README.md` Documents table, and this entry.

**Deliberately not done.** No topic brief, source note or article was written. Nothing was
pushed. `docs/operating-model.md`, `config/editorial-policy.md` and `AGENTS.md` were not
changed. The n8n installation and the `_proofgate-n8n` folder outside this repository were
not touched.

**Open items.**

- Twelve posts need twelve topics; five candidates exist (daylight saving end, first day of
  winter, Thanksgiving, the TSA 3-1-1 liquids rule, the Forever stamp). Seven more must pass
  the entry conditions in `docs/content-backlog.md`.
- `README.md` and `docs/operating-model.md` still call this an English "trends" blog. The
  pilot lanes explain rules, dates and how things work rather than cover trends. The wording
  is deliberately left for the user to decide after the pilot evaluation.

## 2026-10-07 — Publishing platform and site set up

**Decision (user).** The blog is published on its own WordPress site, separate from the Excel
blog: brand **Stateside Explained**, domain `statesideexplained.com`, hosted on the user's
existing Hostinger plan (second site), tagline "Everyday U.S. Questions, Explained Simply".
This replaces the earlier entry "platform for this blog is not decided".

**State on 2026-10-07 (checked from the public site and from the admin, logged in by the user).**

- HTTPS works; permalinks are "Post name"; time zone America/New_York; search engines are
  not discouraged (`index, follow`).
- Sample post moved to the trash; theme footer placeholder links removed; footer credit
  changed to "© 2026 Stateside Explained".
- Plugins added: Rank Math SEO (setup wizard done, account/Google connection skipped) and
  Wordfence Security (license registration not done). Hostinger plugins and LiteSpeed Cache
  were already present.
- About and Privacy Policy exist as drafts only. The Privacy Policy states only what was
  confirmed; it contains no retention periods and no contact email.
- `sitemap_index.xml` returned 404 while the site had no published content; re-check after the
  first post is published.
- No article is published yet. Publishing stays the user's step, per article.

**Not done.** No post was published. Credentials are not recorded in this repository.

## 2026-10-07 — TSA 3-1-1 liquids rule: draft written, Gate 1 passed

**Context.** The first post (daylight saving time) is published and live QA passed. The user told Claude to start research and drafting for the second post, the TSA liquids rule.

**What was done.**

1. Both TSA pages were opened in the built-in browser and the whole text of each was read (the earlier 403 problem applied only to the summarizing reader). Verbatim wording is in `research/sources/tsa-3-1-1-liquids-rule.md`.
2. The draft is `content/drafts/tsa-3-1-1-liquids-rule.md`. Title shortened to 50 characters (a question mark was added to the second question after the user's review on 2026-10-07) (the first post's title was flagged at 83 characters in review). The article uses TSA's wording that separating the liquids bag from the carry-on "facilitates the screening process" and does not add a "must remove" rule, because the page does not state one. It states no claim about whether the rule is new or changed.
3. Own flowchart, no photos (`assets/raw/` and `assets/optimized/`).
4. Gate 1 (factual QA) passed, claim by claim, in `editorial/qa/tsa-3-1-1-liquids-rule.md`.

**Not decided / not done.** Gate 2 (ChatGPT, by commit SHA) has not run. Publish approval has not been requested. A fresh read of both TSA pages is required right before approval; if a page cannot be opened, the article is not published. Medications are excluded from this article.

## 2026-10-07 — TSA 3-1-1 liquids rule: Gate 2 passed

ChatGPT reviewed commit `6db909d`: text and SEO passed; two diagram wordings were fixed in `df5d08c` (the "alarms" line now names liquids, aerosols, gels, creams and pastes; the duty-free line now says original receipt and a purchase within 48 hours). ChatGPT checked the new diagram on `df5d08c` and passed Gate 2. Claude re-read both TSA pages the same day; nothing changed. The article stays in `content/drafts/` until the user approves moving it to `ready`; publishing is a separate approval.

## 2026-10-07 — TSA 3-1-1 liquids rule: approved to move to ready

The user approved moving `tsa-3-1-1-liquids-rule` to `content/ready/` for this article only. Front matter set to `status: ready`; backlog stage `ready`. Publishing remains the user's separate step after the WordPress draft and preview. The user also allowed the Forever stamp source check and brief work to run in parallel.

## 2026-10-07 — Forever stamp: USPS sources re-read in a browser

Claude read S1–S4 in the built-in browser and recorded the wording in `research/sources/forever-stamp-how-it-works.md`. Findings: the S1 validity sentence is only in the page's meta description, so the article takes "remains valid" from the S2 store page's visible text; S3 price list (effective Oct 4, 2026) matches S2's price but has no Forever line; S4 says Global Forever never expires and does not say whether a regular Forever stamp works abroad. The brief was updated (re-check done by Claude, not the user). No price numbers go into article text. Next: draft, Gate 1, Gate 2 (ChatGPT), mandatory USPS re-check before approval.

## 2026-10-07 — Forever stamp: draft written, Gate 1 done

Claude drafted `content/drafts/forever-stamp-how-it-works.md` (about 700 words including front matter and sources) with its own flowchart (no stamp art, no USPS logo). The title was shortened to "How Does a Forever Stamp Work? What It Covers and Doesn't" (57 characters) from the 64-character working title, so it is less likely to be cut off in search results. No price number is in the text. Gate 1 (18 claims) is in `editorial/qa/forever-stamp-how-it-works.md`; one open wording point (C13, "separate stamp") is flagged for Gate 2. Next: Gate 2 by ChatGPT, then the mandatory USPS re-check before the user approves the move to `ready`.

## 2026-10-07 — Forever stamp: Gate 2 passed

ChatGPT reviewed commit `e0aee2b`: title kept (57 characters); body, meta description, structure and diagram readability passed. One fix in three places: the word "separate" (USPS does not use it) was removed from the body, the diagram and the alt text, leaving "the Global Forever stamp". Fixed and recorded; Gate 2 counts as PASS. The article stays in `content/drafts/`. Before the user approves the move to `ready`, Claude re-reads the four USPS pages (mandatory re-check).

## 2026-10-07 — Forever stamp: approved to move to ready

Claude re-read all four USPS pages in the browser first; nothing differed. The user then approved moving `forever-stamp-how-it-works` to `content/ready/` for this article only. Front matter set to `status: ready`; backlog stage `ready`. Publishing order set by the user: (1) the user previews and publishes the TSA article, (2) the user sends the live URL and Claude runs live QA, (3) Claude uploads the Forever stamp article as a WordPress draft, (4) the user previews and publishes it.

## 2026-10-07 — TSA 3-1-1 liquids rule: published and live QA passed

Claude created the WordPress draft (post 19) through the already logged-in browser: title, slug, new category "Airport security rules", diagram with alt text, Rank Math meta description and focus keyword. The user previewed and published it at https://statesideexplained.com/tsa-3-1-1-liquids-rule/. Live QA by Claude passed (body text identical to the repository file; meta, canonical, category, sitemap, feed and home all correct; both TSA source pages open and still carry the checked wording). Moved to `content/published/`. Next: Forever stamp article goes to WordPress as a draft; the user previews and publishes.

## 2026-10-07 — Forever stamp: WordPress draft created

After the TSA live QA, Claude uploaded `forever-stamp-how-it-works` as a WordPress draft (post 22): new category "Postal service and stamps", diagram with alt text, Rank Math meta description and focus keyword. Body text matches the repository file exactly. Not published; the user previews and publishes.

## 2026-10-07 — Forever stamp: published and live QA passed

The user previewed and published the Forever stamp article at https://statesideexplained.com/forever-stamp-how-it-works/. Live QA by Claude passed (body text identical to the repository file; meta, canonical, category, sitemap, feed and home correct). Moved to `content/published/`. Week 1 now has three published articles (daylight saving time, TSA liquids rule, Forever stamp). One non-blocking note: Rank Math's structured data shows `&#039;` for apostrophes in titles (this article and the TSA article).

## 2026-10-07 — Nine briefs written, all three lanes

The user allowed research and briefs only (no drafts, no WordPress, no publishing) for the remaining topics, keeping all three lanes: 12 target minus 3 published minus 2 existing candidates (winter start, Thanksgiving) leaves 7 new, so 9 briefs in total. Briefs in `research/briefs/`: lane 1 first-day-of-winter-2026, thanksgiving-2026-date, federal-holiday-weekend-observed; lane 2 real-id-to-fly-what-tsa-accepts, tsa-thanksgiving-food-carry-on, tsa-precheck-what-it-changes; lane 3 usps-hold-mail-how-it-works, usps-mail-forwarding-how-long, usps-post-office-thanksgiving. If all are written, the lanes finish 4:4:4. Each brief has a candidate card (official sources, photo-free diagram, search-question clarity, changing information, re-check condition) and the official wording read in a real browser on 2026-10-07. Search demand was NOT measured: the autocomplete tool returned results for an unrelated query and was discarded; web search gave only title-level competition (mostly third-party pages). Timing flags: the TSA food and USPS Thanksgiving articles are best written in mid-November, after TSA/USPS publish their 2026 holiday notices, which falls after the 4-week window (ends about Nov 2). Backlog rows 4–12 are at stage `brief`. Reserve ideas not researched: TSA shoe policy, USPS service comparison. Open questions are listed at the end of each brief and in the report to the user.

## 2026-10-07 — User decisions on the nine briefs; two replacement briefs; counts separated by stage

The user decided: (1) the REAL ID article leaves out the ConfirmID fee (not core to the question; a changing price adds re-check work); (2) the Thanksgiving date article goes ahead with the angle "how the date is set"; (3) the July 2026 USPS example is used only in a USPS operations article, only as a case attributed to USPS's own notice, and never as if OPM's substitute-day rule governed USPS, so it was removed from the federal-holiday brief; (4) the TSA Thanksgiving food and USPS Thanksgiving articles wait until mid-November, after the 2026 notices, and are not part of the 4-week pilot's 12 posts; two replacements were to be researched.

Replacements: lane 2 gets `power-bank-on-a-plane-tsa-faa` (two TSA pages and the FAA PackSafe page, updated Oct 2, 2026) and lane 3 gets `usps-informed-delivery-how-it-works` (USPS FAQ dated Sep 30, 2026, plus the usps.com page). The TSA shoe policy was checked and not briefed: its only source for the standard lane is the July 8, 2025 TSA/DHS release, while TSA's own evergreen pages read on 2026-10-07 still say only PreCheck travelers need not remove shoes (Steel Toe Boots, updated May 26, 2022; Laptops, July 15, 2026), so it is kept as a reserve idea (backlog row 15). New titles avoid apostrophes because of the `&#039;` structured-data issue.

Counting rule (user request): the backlog now has a "Count by stage" table and a "Pilot 12" column. Only the `published` row counts as articles on the live site (3 today); briefs, drafts, ready items, deferred items and ideas are tracked separately, and the pilot result is read from the published count only. Pilot plan: 3 published + 9 briefs = 12, four per lane. Search demand is still not measured for any brief.

## 2026-10-07 — User decisions on the replacements; first-day-of-winter-2026 drafted, Gate 1 done

The user approved the power-bank article as the lane 2 replacement (keep the mandatory pre-publish re-check) and told Claude to include the "why did I get a sign-up letter" explanation in the Informed Delivery article only if the USPS FAQ clearly confirms the process, as one short subheading; otherwise leave it out. The user recommended the next drafting order, one per lane: (1) first day of winter, (2) power banks, (3) Informed Delivery after extra FAQ reading. The user pushed `fbf065d`.

Claude re-read USNO and NOAA in the browser, wrote `research/sources/first-day-of-winter-2026.md`, drafted `content/drafts/first-day-of-winter-2026.md` (about 600 words, title 52 characters, meta description 152 characters), made its own diagram and recorded Gate 1 (21 claims, all pass) in `editorial/qa/first-day-of-winter-2026.md`. Two corrections to the brief: NOAA's visible update date is March 10, 2023 (the metadata dates differ), and the time-zone list is six zones from USNO's own selector instead of three. Next: Gate 2 by ChatGPT, then a recommended source re-check before the user approves the move to `ready`. Not on WordPress.

## 2026-10-07 — power-bank-on-a-plane-tsa-faa drafted, Gate 1 done

Claude wrote `research/sources/power-bank-on-a-plane-tsa-faa.md`, drafted `content/drafts/power-bank-on-a-plane-tsa-faa.md` (about 700 words; title 56 characters, shortened from the brief's 63-character proposal; meta description 149 characters), made its own decision diagram and recorded Gate 1 (21 claims, all pass) in `editorial/qa/power-bank-on-a-plane-tsa-faa.md`. The three pages (two TSA, one FAA) were re-read in the browser after the draft and 29 phrases and numbers were tested against them. The article attributes the 100 Wh limit to the FAA because TSA's "Power Banks" page does not state it. It links once to the published TSA 3-1-1 article. Next: Gate 2 by ChatGPT; the pre-approval re-check of all three pages stays mandatory. Not on WordPress.

## 2026-10-07 — usps-informed-delivery-how-it-works drafted, Gate 1 done; the sign-up-letter section is in

Before drafting, Claude read the USPS FAQ sections that the brief had listed as unread (Welcome Letter, Dashboard, Daily Digest and issues, Privacy & Security, Missing Mail). The FAQ confirms the "why did I get a letter" process twice, so the user's condition was met and the draft has one short subheading for it, repeating only USPS's statements and not printing the USPS web address. Claude wrote `research/sources/usps-informed-delivery-how-it-works.md`, drafted `content/drafts/usps-informed-delivery-how-it-works.md` (about 840 words; title 58 characters, no apostrophe; meta description 151 characters), made its own flow diagram and recorded Gate 1 (24 claims, all pass) in `editorial/qa/usps-informed-delivery-how-it-works.md`. 41 phrases were tested against the two USPS pages after drafting. Not read and not described: the mobile app section, change of address, redelivery, referrals. The article is longer than the other two drafts; Gate 2 may trim it. Next: Gate 2 by ChatGPT for all three drafts; the pre-approval re-check of the USPS pages stays mandatory. Nothing is on WordPress.

## 2026-10-07 — Gate 2 passed for the three drafts

ChatGPT reviewed commit `2edbc32` and passed the English + SEO review (Gate 2) for `first-day-of-winter-2026`, `power-bank-on-a-plane-tsa-faa` and `usps-informed-delivery-how-it-works`, with no changes requested. Gate 2 PASS is recorded in each QA record and in the backlog; the articles stay in `content/drafts/`. Next order set by the user: the winter article first, with the recommended source re-check, then a request for approval to move it to `ready`. The power-bank and Informed Delivery articles each need a mandatory official-source re-check right before their own ready-move approval. Counts: published 3; ready 0; draft 3; brief 6 (pilot) plus 2 deferred; idea 1.

## 2026-10-07 — first-day-of-winter-2026: pre-approval re-check done, approval requested

Claude re-ran the USNO query (seven time-zone offsets) and tested 13 NOAA phrases after Gate 2 passed. No difference from the draft. Claude asked the user to approve moving only this article to `content/ready/`. Nothing moved yet.

## 2026-10-07 — first-day-of-winter-2026: approved to move to ready

The user pushed `23c2394` and approved moving `first-day-of-winter-2026` to `content/ready/` (this article only). Claude moved the file, set `status: ready`, recorded Gate 3 in the QA record and set the backlog stage to `ready`. Next: WordPress draft by Claude, then the user previews and publishes. Counts: published 3; ready 1; draft 2; brief 6 (pilot) plus 2 deferred; idea 1.

## 2026-10-07 — first-day-of-winter-2026: WordPress draft created

After the user pushed `0f95e56` and asked for it, Claude created the WordPress draft through the logged-in browser: post 25, slug `first-day-of-winter-2026`, category "US dates, seasons and holidays", diagram (media 24) with alt text, Rank Math meta description and focus keyword. Body text on the preview matches the repository file exactly. Not published; the user previews on phone width and publishes. Counts: published 3; ready 1 (WordPress draft); draft 2; brief 6 (pilot) plus 2 deferred; idea 1.

## 2026-10-07 — first-day-of-winter-2026: published and live QA passed

The user pushed `20132c7`, previewed and published the winter article at https://statesideexplained.com/first-day-of-winter-2026/. Live QA by Claude passed (body text identical to the repository file; meta, canonical, category, sitemap, feed and home correct; the structured data has no `&#039;` because the title has no apostrophe). Moved to `content/published/`. Counts: published 4 (daylight saving time, TSA liquids rule, Forever stamp, first day of winter); ready 0; draft 2 (power bank, Informed Delivery); brief 6 (pilot) plus 2 deferred; idea 1.

## 2026-10-07 — power-bank-on-a-plane-tsa-faa: mandatory re-check done, approval requested

After the user's push of `50a1a5a`, Claude re-read the two TSA pages and the FAA page and tested 29 phrases and numbers: no difference, same page dates. Claude asked the user to approve moving only this article to `content/ready/`. Nothing moved yet.

## 2026-10-07 — power-bank-on-a-plane-tsa-faa: approved to move to ready; push rule changed

The user pushed `81318be` and approved moving `power-bank-on-a-plane-tsa-faa` to `content/ready/` (this article only). Claude moved the file, set `status: ready`, recorded Gate 3 in the QA record and set the backlog stage to `ready`. The mandatory re-check of the TSA and FAA pages is repeated right before publishing.

Rule change by the user (2026-10-07): Claude may now push local commits itself, by typing `git push origin main` in the user's own VS Code terminal through computer control, after showing the list of commits to be pushed and after the user has granted access to the app. Only `git push origin main`; never a forced push or another branch; Claude reads the result and reports it. Publishing on WordPress stays the user's step. Counts: published 4; ready 1; draft 1; brief 6 (pilot) plus 2 deferred; idea 1.

## 2026-10-07 — push rule: computer-control push does not work; user pushes

The push rule recorded above (Claude types `git push origin main` into the user's VS Code terminal) could not be used: when Claude checked the access it would get, VS Code is granted only at a click-only level (no typing or key presses), and Claude did not work around that block. The user pushed `a8ca13e` themselves (`81318be..a8ca13e`). Standing rule again: the user pushes; Claude shows the commit list and asks.

## 2026-10-07 — power-bank-on-a-plane-tsa-faa: WordPress draft created

At the user's request Claude created the WordPress draft (post id 28, media id 27): title, slug, category "Airport security rules", diagram with alt text, Rank Math meta description and focus keyword as in the front matter. Not published. Body text on the draft equals `content/ready/`. The user previews on a phone and publishes; mandatory re-check of the three TSA/FAA pages right before Publish. Counts: published 4; ready 1 (on WordPress as a draft); draft 1 (Informed Delivery); brief 6 (pilot) plus 2 deferred; idea 1.

## 2026-10-07 — usps-informed-delivery-how-it-works: mandatory re-check done, approval requested

After the power bank WordPress draft, Claude re-read the USPS FAQ "Informed Delivery - The Basics" and the usps.com Informed Delivery page and tested 36 + 8 phrases and numbers: no difference, same FAQ date (Sep 30, 2026). Claude asked the user to approve moving only this article to `content/ready/`. Nothing moved yet.

## 2026-10-07 — usps-informed-delivery-how-it-works: approved to move to ready

The user pushed `cafc738` and approved moving `usps-informed-delivery-how-it-works` to `content/ready/` (this article only). Claude moved the file, set `status: ready`, recorded Gate 3 in the QA record and set the backlog stage to `ready`. Not on WordPress yet. The mandatory re-check of the two USPS pages is repeated right before publishing. Counts: published 4; ready 2 (power bank on WordPress as a draft, id 28; Informed Delivery not yet on WordPress); draft 0; brief 6 (pilot) plus 2 deferred; idea 1.

## 2026-10-07 — usps-informed-delivery-how-it-works: WordPress draft created

At the user's request Claude created the WordPress draft (post id 30, media id 29): title, slug, category "Postal service and stamps", diagram with alt text, Rank Math meta description and focus keyword as in the front matter. Not published. Body text equals `content/ready/`. The user previews on a phone and publishes; mandatory re-check of the two USPS pages right before Publish.

Instruction for today (user, 2026-10-07): draft the six remaining pilot briefs in order, starting with the Thanksgiving date article. Each gets: official sources re-opened, source notes, draft with a photo-free diagram, Gate 1 factual QA, local commit. No WordPress upload, no move to `ready`, no publishing. If a source cannot be opened or checking is insufficient, the article is not forced; only a hold and its reason are recorded.

## 2026-10-07 — thanksgiving-2026-date: draft written, Gate 1 done

Under the user's instruction of 2026-10-07 (drafts only, up to Gate 1 and a local commit), Claude re-opened the OPM Federal Holidays page and 5 U.S.C. 6103 (2023 edition, govinfo.gov), wrote the source notes, the draft with its own calendar diagram, and the Gate 1 claim table (14 claims, all pass; two are computed and labeled). The OPM tables for 2024 to 2030 match the computed fourth Thursdays. No WordPress upload, no move to ready. Counts: published 4; ready 2; draft 1; brief 5 (pilot) plus 2 deferred; idea 1.

## 2026-10-07 — federal-holiday-weekend-observed: draft written, Gate 1 done

Claude re-opened the OPM Federal Holidays page and read 5 U.S.C. 6103 with Executive Order 11582 (govinfo.gov, 2023 edition), wrote the source notes, the draft with its own diagram, and the Gate 1 claim table (19 claims, all pass; weekday facts computed and labeled). No USPS source is used. Alt text is long (539 characters); Gate 2 may shorten it. No WordPress upload, no move to ready. Counts: published 4; ready 2; draft 2; brief 4 (pilot) plus 2 deferred; idea 1.

## 2026-10-07 — real-id-to-fly-what-tsa-accepts: draft written, Gate 1 done

Claude re-opened the three TSA pages (acceptable ID, REAL ID, ConfirmID), tested 34 quoted statements (all present, none changed), wrote the source notes, the draft with its own flowchart (no ID images, no fee amount), and the Gate 1 claim table (18 claims, all pass). Mandatory re-check before approval and before publishing stays. No WordPress upload, no move to ready. Counts: published 4; ready 2; draft 3; brief 3 (pilot) plus 2 deferred; idea 1.

## 2026-10-07 — tsa-precheck-what-it-changes: draft written, Gate 1 done

Claude re-opened the TSA PreCheck page and also read the PreCheck FAQ and the KTN benefits page (the brief had read only the first), tested 30 quoted statements (all present), wrote the source notes, the draft with its own three-step diagram, and the Gate 1 claim table (20 claims, all pass). The brief's open question 2 was not answered, so the 99% wait-time statement was left out as promotional; no prices or offers. Mandatory re-check before approval and publishing stays. No WordPress upload, no move to ready. Counts: published 4; ready 2; draft 4; brief 2 (pilot) plus 2 deferred; idea 1.

## 2026-10-07 — usps-hold-mail-how-it-works: draft written, Gate 1 done

Claude re-opened the three USPS pages (Hold Mail, the Hold Mail FAQ dated Sep 16, 2026, Standard Forward Mail), tested 35 quoted statements (all present, none changed), wrote the source notes, the draft with its own four-step timeline, and the Gate 1 claim table (20 claims, all pass). The brief's open question 2 was not answered; the in-person route (PS Form 8076) is one sentence attributed to the FAQ. Mandatory re-check before approval and publishing stays. No WordPress upload, no move to ready. Counts: published 4; ready 2; draft 5; brief 1 (pilot) plus 2 deferred; idea 1.

## 2026-10-07 — Draft: usps-mail-forwarding-how-long

Sixth and last pilot draft. Three USPS pages re-read; extension prices and fee left out; periodicals difference between the pages reported separately; Gate 1 done; no WordPress upload, no ready move. Counts: published 4; ready 2; draft 6; brief 0 (pilot) plus 2 deferred; idea 1.

## 2026-10-07 — Power bank and Informed Delivery: published, live QA, moved to `content/published/`

The user published both articles in WordPress and sent the live URLs: https://statesideexplained.com/power-bank-on-a-plane-tsa-faa/ (post 28) and https://statesideexplained.com/usps-informed-delivery-how-it-works/ (post 30). Claude read the live pages in the built-in browser: HTTP 200, canonical equals the URL, robots index/follow, Rank Math meta description present and equal to the front matter, one diagram with alt text, correct category, BlogPosting JSON-LD, no comment form, listed on the home page, in `/feed/` and in `post-sitemap.xml`, official source links present. The files moved from `content/ready/` to `content/published/` with `status: published`, `published_date: 2026-10-07` and `live_url` added; backlog stage set to `published`. The diagram text size on a real phone and the pre-publish re-check of the official pages are the user's steps and are not recorded here. Local commit only; the push is the user's step. Counts: published 6; ready 0; draft 6; brief 0 (pilot) plus 2 deferred; idea 1.

## 2026-10-07 — Policy: no comments and no pingbacks (incoming or outgoing)

**Trigger.** The power bank article links to the TSA 3-1-1 liquids article, and WordPress created an automatic pingback on the liquids post (comment 2, type pingback, from the site's own post). It was not a reader comment.

**Decision (user).** The site does not use regular comments, incoming pingbacks/trackbacks or outgoing pingbacks.

**Done in WordPress 2026-10-07 (Claude, logged-in browser).**

1. The pingback (comment 2) was moved to the trash (not permanently deleted).
2. `ping_status` set to closed on post 19 (`tsa-3-1-1-liquids-rule`) and post 22 (`forever-stamp-how-it-works`), which were still open. All six published posts now show ping closed and comments closed.
3. Settings → Discussion, all three unchecked and saved ("Settings saved" confirmed on reload): "Attempt to notify any blogs linked to from the post" (outgoing pingbacks), "Allow link notifications from other blogs (pingbacks and trackbacks) on new posts" (incoming), and "Allow people to submit comments on new posts" (new-post comment default).

**Going forward.** New posts are created with comments and pings closed by default; still confirm both are closed when creating each WordPress draft and in live QA. Revisit this policy only if the user decides to open comments.

## 2026-10-07 — Gate 2 for the six new drafts, fixes applied

ChatGPT's Gate 2 result (reported by the user): PASS for `thanksgiving-2026-date`, `federal-holiday-weekend-observed` and `usps-hold-mail-how-it-works`; FIX REQUIRED for three.

1. `real-id-to-fly-what-tsa-accepts`: the first answer and the meta description now answer "is a REAL ID required?" directly ("No—not necessarily ...").
2. `tsa-precheck-what-it-changes`: the bold first sentence now reads "offers eligible travelers a speedier security experience"; the diagram label "Stays on you:" became "You can keep on:" (alt text updated to match).
3. `usps-mail-forwarding-how-long`: the 12 months is stated as the permanent-change figure in the first answer, the meta description and the diagram ("2. Permanent forwarding: 12 months"); the temporary-change wording ("the period you specify") is now in the first three sentences.

Each fix was re-checked against the source notes and recorded in the article's `editorial/qa/` file. Condition from Gate 2: the forwarding article keeps its internal link to the Hold Mail article only if Hold Mail is published first; otherwise the link is removed. Not done: the fixed articles have not gone back to Gate 2 (ChatGPT re-reviews the fix commit); no WordPress upload, no ready move, no publishing. Counts: published 6; ready 0; draft 6; brief 0 (pilot) plus 2 deferred; idea 1.

## 2026-10-07 — Gate 2 final PASS for all six new drafts

ChatGPT re-reviewed the fix commit `4746e4a`: `tsa-precheck-what-it-changes` and `usps-mail-forwarding-how-long` passed. `real-id-to-fly-what-tsa-accepts` got one more sentence fix, applied locally: the REAL ID page sentence now reads "TSA's REAL ID page says that a traveler using a state-issued driver's license or ID card for a domestic flight must use one that is REAL ID compliant. TSA's identification page also lists other acceptable forms of ID, including a U.S. passport." Claude noted in the QA record that this narrows the REAL ID page's own wording (S2-2) using the identification page (S1-6). With the three earlier PASS results, all six drafts are recorded as Gate 2 final PASS. They are still drafts: not on WordPress, not in `content/ready/`, not published. Next steps: the user approves each move to `ready` separately; the mandatory official-page re-check comes right before approval for the REAL ID, PreCheck, Hold Mail and forwarding articles (recommended for the two lane-1 articles); Hold Mail is published before forwarding, or the forwarding article's internal link is removed.

Also on 2026-10-07: Informed Delivery (post 30) was found in `draft` status with a 404 for logged-out visitors (modified 03:43 site time, not by Claude). Per the user's instruction it was not recreated or republished; the user will check the preview and press Publish. The repository record `content/published/usps-informed-delivery-how-it-works.md` is unchanged until the post is live again.

## 2026-10-07 — Recommended re-check for the Thanksgiving and weekend-holiday drafts

At the user's request, Claude re-read the sources of `thanksgiving-2026-date` and `federal-holiday-weekend-observed` before asking for ready-move approval: the OPM "Federal Holidays" page (19 of 19 strings present) and 5 U.S.C. 6103 on govinfo (14 of 14 items present; three differ only in formatting), and recomputed the dates. No difference; no article change. Approval to move each article to `content/ready/` is requested separately. Order condition kept: `usps-hold-mail-how-it-works` is published before `usps-mail-forwarding-how-long`. Informed Delivery (post 30) is still a WordPress draft until the user publishes it; live QA and the `content/published/` record follow after that.

## 2026-10-07 — Thanksgiving date and weekend-holiday articles: moved to `content/ready/`

The user approved moving `thanksgiving-2026-date` and `federal-holiday-weekend-observed` to `content/ready/`, each for its own article, after Gate 2 final PASS and the recommended source re-check (no difference). Front matter set to `status: ready`; backlog stage `ready`; the weekend-holiday article's alt text was first kept at 539 characters (Gate 2 passed it). Not on WordPress and not published. Publish order kept: Hold Mail before mail forwarding. Counts (repository): published 6 (Informed Delivery is a WordPress draft again, not live); ready 2; draft 4; brief 0 (pilot) plus 2 deferred; idea 1.

## 2026-10-07 — Weekend-holiday article: alt text shortened before the push

With the ready-move approval, the user asked for a shorter alt text for `federal-holiday-weekend-observed` and gave the wording: "Diagram of the federal-holiday weekend rule for most federal employees: Saturday holidays are observed Friday; Sunday holidays Monday. It shows OPM examples from 2026–2028, including July 4, 2026 observed July 3 and July 4, 2027 observed July 5." Applied in `content/ready/federal-holiday-weekend-observed.md` (front matter and body identical, 245 characters), checked against the diagram and OPM's wording, recorded in the QA file. The diagram image is unchanged. Both articles stay in `content/ready/`; not on WordPress, not published. The user pushes the local commits together.

## 2026-10-07 — Informed Delivery: republished, live QA passed again

After the status of post 30 changed to draft about 03:43 (not by Claude; 404 for logged-out visitors), the user previewed it and published it again at 04:10. Claude checked the live page: 200, canonical equals the URL, robots index/follow, meta description 151 characters, one diagram with alt text, correct category, the same seven headings and 4,496 characters of visible text as before, two USPS source links, comments and pings closed, listed on the home page, in the feed and in the sitemap. The repository file `content/published/usps-informed-delivery-how-it-works.md` needed no change. The cause of the 03:43 status change is not known; if a bulk edit in the posts list is the cause, avoid bulk status edits there. Counts: published 6 (all live); ready 2; draft 4; brief 0 (pilot) plus 2 deferred; idea 1.

## 2026-10-07 — WordPress drafts for the Thanksgiving date and weekend-holiday articles

Claude created the two WordPress drafts through the logged-in browser (no publishing): `thanksgiving-2026-date` as post 34 (media 33) and `federal-holiday-weekend-observed` as post 36 (media 35). Title, slug, category (US dates, seasons and holidays), diagram with alt text, Rank Math meta description and focus keyword were set; comments and pings are closed (per the no-comments policy). Checks: the text equals the repository text (1,967 and 2,960 letters and digits), the uploaded PNGs match the repository hashes, the Rank Math values were confirmed in the edit screens, and both drafts return 404 when logged out. Preview links: https://statesideexplained.com/?p=34 and https://statesideexplained.com/?p=36. The user previews on a phone and publishes; live QA and the move to `content/published/` follow. Counts: published 6; ready 2 (both with WordPress drafts); draft 4; brief 0 (pilot) plus 2 deferred; idea 1.

## 2026-10-07 — Thanksgiving date and weekend-holiday articles published; Hold Mail re-check

The user published `thanksgiving-2026-date` (post 34) and `federal-holiday-weekend-observed` (post 36) at 04:15 site time and sent the live URLs. Claude's live QA passed for both: 200, canonical, robots index/follow, meta description equals the front matter, one diagram with identical alt text, body text equals the repository text, two official source links, BlogPosting JSON-LD, comments and pings closed, listed on the home page, in the feed and in the sitemap. Both files moved from `content/ready/` to `content/published/` with `status: published`, `published_date` and `live_url`; backlog stage `published`.

Then, as step 2 of the user's sequence, Claude ran the mandatory pre-approval re-check of the three USPS pages for `usps-hold-mail-how-it-works` (S1 6 of 6, S2 29 of 29, S3 3 of 3 strings present; FAQ date still Sep 16, 2026): no difference, no article change. The ready-move approval for Hold Mail is requested separately. Order condition kept: Hold Mail before mail forwarding. Counts: published 8; ready 0; draft 4 (REAL ID, PreCheck, Hold Mail, forwarding); brief 0 (pilot) plus 2 deferred; idea 1.

## 2026-10-07 — Hold Mail: moved to `content/ready/`

The user approved moving `usps-hold-mail-how-it-works` to `content/ready/` after Gate 2 final PASS and the mandatory pre-approval re-check (S1 6 of 6, S2 29 of 29, S3 3 of 3 strings; no difference). Front matter set to `status: ready`; backlog stage `ready`. Not on WordPress and not published. Still mandatory: a fresh read of the three USPS pages right before publishing. Order kept: Hold Mail before mail forwarding. Counts: published 8; ready 1; draft 3 (REAL ID, PreCheck, forwarding); brief 0 (pilot) plus 2 deferred; idea 1.

## 2026-10-08 — Hold Mail WordPress draft; TSA re-check for REAL ID and PreCheck

Hold Mail: Claude created the WordPress draft (post 40, media 39; not published): title, slug, category (Postal service and stamps), diagram with alt text, Rank Math meta description and focus keyword set; comments and pings closed; text equals the repository text (3,137 letters and digits); Rank Math values confirmed in the edit screen; 404 when logged out. WordPress scaled the 1200x2667 diagram to 1152x2560, so the post's image block now points to the original file (hash equals the repository PNG). The draft was built from the draft-folder text as pushed, because the ready-move commit had not been pushed; the two differ only in the `status` line. Preview: https://statesideexplained.com/?p=40. Before publishing: mandatory USPS re-check; Hold Mail goes live before mail forwarding.

REAL ID and PreCheck: Claude ran the mandatory TSA re-check. REAL ID: identification page 25 of 25, REAL ID page 4 of 4, ConfirmID page 3 of 3. PreCheck: PreCheck page 9 of 9, FAQ 15 of 15 (three strings differed only in spacing), benefits page 7 of 7. No difference; no article change. The ready-move approval is requested separately for each. The mail forwarding article waits until Hold Mail is actually published (user instruction). Counts: published 8; ready 1 (Hold Mail, with a WordPress draft); draft 3 (REAL ID, PreCheck, forwarding); brief 0 (pilot) plus 2 deferred; idea 1.


## 2026-10-08 — REAL ID and PreCheck: moved to `content/ready/`

The user approved moving `real-id-to-fly-what-tsa-accepts` and `tsa-precheck-what-it-changes` to `content/ready/`, each for its own article, after Gate 2 final PASS and the mandatory TSA re-check (2026-10-08, no difference). Front matter set to `status: ready`; backlog stage `ready`; QA files and briefs updated. Neither is on WordPress and neither is published; WordPress drafts are created only when the user asks, and each needs a fresh TSA re-check right before publishing. Hold Mail (post 40) stays a WordPress draft: the user previews it and asks for the USPS re-check right before Publish. The mail forwarding article waits until Hold Mail is actually published. Counts: published 8; ready 3 (Hold Mail with a WordPress draft; REAL ID and PreCheck without); draft 1 (forwarding); brief 0 (pilot) plus 2 deferred; idea 1.


## 2026-10-07 — Hold Mail published; live QA passed

The user published `usps-hold-mail-how-it-works` (post 40) at 19:44 site time and sent the live URL https://statesideexplained.com/usps-hold-mail-how-it-works/ . Claude's live QA passed: 200, canonical, robots index/follow, meta description equals the front matter, one diagram with identical alt text and the original PNG, body text equals the repository text, three official USPS links, comments and pings closed, listed on the home page, in the feed and in the sitemap. The user published before asking for the pre-publish USPS re-check, so Claude ran it right after publishing: all three pages unchanged. The file moved from `content/ready/` to `content/published/` with `status: published`, `published_date` and `live_url`. Hold Mail is now live, so the mail forwarding article can start: its internal link to Hold Mail may stay. Next for forwarding: mandatory USPS re-check and the ready-move request (no WordPress draft until asked). Counts: published 9; ready 2 (REAL ID, PreCheck); draft 1 (forwarding); brief 0 (pilot) plus 2 deferred; idea 1.


## 2026-10-08 — WordPress drafts for REAL ID and PreCheck; mail forwarding re-check finds a USPS change

The user pushed `3a634ab` (Hold Mail publish record) and asked for WordPress drafts of the REAL ID and PreCheck articles (not published), then the mandatory USPS re-check for mail forwarding.

Drafts: Claude created `real-id-to-fly-what-tsa-accepts` as post 43 (media 42) and `tsa-precheck-what-it-changes` as post 45 (media 44), both draft, category Airport security rules, comments and pings closed, title, slug, diagram with alt text, Rank Math meta description and focus keyword set. Checks: text equals the repository text (3,372 and 2,843 letters and digits), images equal the repository PNGs (the REAL ID diagram, 2,607 px tall, was scaled by WordPress; the block points to the original file), Rank Math values confirmed in the edit screens, 404 when logged out. Previews: https://statesideexplained.com/?p=43 and https://statesideexplained.com/?p=45 . Standing instruction: the user asks for a TSA re-check right before Publish for each; Claude does not publish.

Mail forwarding: the re-check found a difference. S2 and S3 unchanged. The USPS forwarding page (S1) now says to allow at least 7-10 business days after approval (the "3 business days / 2 weeks" sentence is gone), that periodicals are forwarded free for 60 days if prepaid by the sender, and that Marketing Mail is not forwarded unless the sender paid forwarding postage. The article and its diagram still use the old S1 wording, so the ready-move approval is not requested. Proposed fix (needs the user's decision, then a new Gate 2 check of the changed parts): (a) replace the start-timing sentence with S1's new "allow at least 7-10 business days for it to go into effect" and change the diagram's first step and the alt text the same way; (b) delete the paragraph about the two pages describing periodicals differently and state the shared 60-day wording for periodicals; (c) change "USPS Marketing Mail is not forwarded" to "not forwarded unless the sender has paid forwarding postage". The 12-month answer, meta description and Extended Mail Forwarding section stay. The user's Publish-time USPS re-check for this article also stays.

Counts: published 9; ready 2 (REAL ID and PreCheck, each with a WordPress draft, not published); draft 1 (forwarding, needs the fix above); brief 0 (pilot) plus 2 deferred; idea 1.


## 2026-10-07 — REAL ID and PreCheck published; live QA passed

The user published `real-id-to-fly-what-tsa-accepts` (post 43) and `tsa-precheck-what-it-changes` (post 45) at 19:56 site time and sent the live URLs https://statesideexplained.com/real-id-to-fly-what-tsa-accepts/ and https://statesideexplained.com/tsa-precheck-what-it-changes/ . Claude's live QA passed for both: 200, canonical, robots index/follow, meta description equals the front matter, one diagram with identical alt text and the original PNG, body text equals the repository text, official TSA source links (and the one internal link in PreCheck), comments and pings closed, listed on the home page, in the feed and in the sitemap. The pre-publish TSA re-check was not requested before Publish, so Claude ran it right after publishing: all six TSA pages unchanged (identification 30 of 30, REAL ID 4 of 4, ConfirmID 4 of 4, PreCheck 7 of 7, FAQ 10 of 10, benefits 3 of 3). Both files moved from `content/ready/` to `content/published/` with `status: published`, `published_date` and `live_url`; backlog stage `published`. Counts: published 11 (lane 1: 4; lane 2: 4; lane 3: 3 of 4); ready 0; draft 1 (forwarding, being fixed after the USPS change); brief 0 (pilot) plus 2 deferred; idea 1.


## 2026-10-08 — Mail forwarding article fixed after the USPS change

The user approved the three proposed fixes after the USPS forwarding page changed (start timing, periodicals, Marketing Mail). Claude changed `content/drafts/usps-mail-forwarding-how-long.md`: the start-timing sentence now says to allow at least 7-10 business days after approval; periodicals are forwarded for free for 60 days if fully prepaid by the sender (the old "the two pages disagree" paragraph is replaced by "the FAQ gives the same 60-day figure"); Marketing Mail is not forwarded unless the sender has paid forwarding postage. The diagram (cards 1 and 2 and the footer date), its alt text (366 characters, identical in front matter and body) and the as-of dates (October 8, 2026) were updated, and the source notes record the new S1 wording. The 12-month answer, meta description and Extended Mail Forwarding section are unchanged. The article stays in `content/drafts/`; Gate 2 of the changed parts comes next, then the mandatory USPS re-check and the ready-move request. The user's Publish-time USPS re-check also stays. Hold Mail is published, so the internal link to it stays.


## 2026-10-08 — Mail forwarding: Gate 2 PASS on the fix; re-check accepted; ready-move requested

ChatGPT's Gate 2 re-review of `usps-mail-forwarding-how-long` on commit `e323977` is PASS (reported by the user); body, diagram and alt text stay unchanged. The user decided that the 2026-10-08 USPS re-check (S2 and S3 unchanged, S1 changed and then fixed in the article) counts as the mandatory pre-approval re-check; Claude noted in the QA record that it was run before the fix and that no USPS page was re-read after it. QA record, backlog and briefs updated. Claude asks the user for the ready-move approval; nothing is moved until the user says yes. Still required later: a fresh USPS re-read right before Publish, on the user's request. Counts unchanged: published 11; ready 0; draft 1 (forwarding, waiting for the ready-move approval); brief 0 (pilot) plus 2 deferred; idea 1.


## 2026-10-08 — Mail forwarding article moved to `content/ready/`

The user approved moving `usps-mail-forwarding-how-long` to `content/ready/` after Gate 2 PASS on the fix (commit `e323977`) and the accepted 2026-10-08 USPS re-check. Front matter set to `status: ready`; backlog stage `ready`; QA record and brief updated. Not on WordPress and not published; the WordPress draft is created only when the user asks, and a fresh USPS re-read is needed right before Publish. This was the last pilot article to reach `ready`. Counts: published 11; ready 1 (forwarding); draft 0; brief 0 (pilot) plus 2 deferred; idea 1.


## 2026-10-08 — Mail forwarding WordPress draft

At the user's request Claude created the WordPress draft for `usps-mail-forwarding-how-long` (post 49, media 48; not published) from the `content/ready/` file as pushed (`a56b560`): title, slug, category Postal service and stamps, diagram with alt text, Rank Math meta description and focus keyword set; comments and pings closed. Checks: text equals the repository text (3,638 letters and digits), the image equals the repository PNG (WordPress scaled the 2,697 px tall upload; the block points to the original file), Rank Math values confirmed in the edit screen, 404 when logged out, one post with the slug. Preview: https://statesideexplained.com/?p=49 . The user previews and publishes; the USPS re-check right before Publish is on the user's request. Counts: published 11; ready 1 (forwarding, with a WordPress draft); draft 0; brief 0 (pilot) plus 2 deferred; idea 1.


## 2026-10-07 — Mail forwarding published; live QA passed; pilot content complete

The user published `usps-mail-forwarding-how-long` (post 49) at 20:11 site time and sent the live URL https://statesideexplained.com/usps-mail-forwarding-how-long/ . Claude's live QA passed: 200, canonical, robots index/follow, meta description equals the front matter, one diagram with identical alt text and the original PNG, body text equals the repository text, one internal link (Hold Mail) and three official USPS links, comments and pings closed (the site has no comments or pingbacks), listed on the home page, in the feed and in the sitemap. The pre-publish USPS re-check was not requested before Publish, so Claude ran it right after publishing: all three USPS pages unchanged since the 2026-10-08 fix (forwarding page 16 of 16, FAQ options page 2 of 2, Extended Mail Forwarding FAQ 7 of 7). The file moved from `content/ready/` to `content/published/` with `status: published`, `published_date` and `live_url`; backlog stage `published`. All 12 pilot articles are now published (lane 1: 4; lane 2: 4; lane 3: 4). Counts: published 12; ready 0; draft 0; brief 0 (pilot) plus 2 deferred (Thanksgiving, mid-November); idea 1. Next: the 1-week checkpoint and the 4-week evaluation, the DST source re-check before 2026-11-01, and the site cleanup items.

## 2026-10-08 — Pilot checkpoint and evaluation record frame created

At the user's request Claude wrote `docs/pilot-evaluation.md`: a checklist and record frame for the 1-week checkpoint (on or after 2026-10-14) and the 4-week evaluation (on or after 2026-11-04), counted from the publish date of all 12 pilot articles (2026-10-07, site time). The principle is kept: the pilot result is read only from the 12 `published` rows of `docs/content-backlog.md`; the deferred briefs, the idea, the home page, categories, About and Privacy Policy are recorded separately and not added to the 12. The document covers: Search Console setup steps for the user (property type, ownership, sitemap submission of `https://statesideexplained.com/sitemap_index.xml`, whether to use "Request indexing"), the index and Pages report items, URL inspection per article (indexed, last crawl, Google-selected canonical), sitemap submission and read status, the Performance report (7 days at the checkpoint, 28 days at the evaluation; Pages and Queries), manual search checks (title, focus keyword, no numeric rank, `site:` only as a rough hint), the four per-lane evaluation items from `docs/blog-c-site-structure.md` section 4, and a log of operating events (pingbacks, the Informed Delivery draft flip, post-publish re-checks, the USPS forwarding wording change). Tables A to E carry the 12 articles with URL, publish date and focus keyword pre-filled; check dates and values are blank and marked `—` when unknown.

Facts recorded as of 2026-10-08 (Claude, public pages): `sitemap_index.xml` returns 200 and lists `post-sitemap.xml` (13 URLs: the home page plus the 12 posts) and `category-sitemap.xml` (3 categories); `robots.txt` allows crawling except `/wp-admin/` and declares the sitemap; the `www` address does not load. Not known: whether a Search Console property exists (Rank Math's Google connection was skipped at setup); Claude has no access to the user's Search Console.

Noted for the evaluation: all 12 articles were published on one day instead of 3 per week, so whether 3 posts per week is sustainable cannot be read from the schedule; it can only be read from the user's own time record. No pass or fail thresholds were set; the user decides them before the evaluation and records them here. No article, diagram or WordPress setting was changed.

## 2026-10-08 — Site cleanup: inspection results and the user's decisions

**Inspection (Claude, read-only; nothing in WordPress, DNS or hosting was changed).**

- Author display `admin`: the visible byline (post-author-name block, linking to `/author/admin/`), the JSON-LD Person and BlogPosting author, the social meta "Written by admin" and the feed `dc:creator` all show `admin`. There is one user: login name, display name and URL slug are all `admin`, so the author URL discloses the login name. Already blocked: the public users REST list returns 401, `/?author=1` returns 404, no users sitemap (404). The author archive `/author/admin/` opens (200) and is `noindex` (Rank Math). The JSON-LD Person image is a Gravatar URL derived from the account email (a hash of the email is public).
- `www`: DNS answers for `www.statesideexplained.com` as a CNAME to `statesideexplained.com`; both resolve to `31.170.160.71` (so `www` is DNS-only, not proxied). The authoritative DNS answer shows Cloudflare name servers. HTTPS to `www` fails in the built-in browser (cause not confirmed: certificate not covering `www` or no `www` alias at the host). `http://statesideexplained.com` redirects to HTTPS and opens (200). WordPress Address and Site Address are `https://statesideexplained.com`; canonical and sitemap use the non-`www` address.
- About (page 9) and Privacy Policy (page 3) are drafts, linked nowhere (no header menu, no footer links); the Privacy Policy is set as the WordPress privacy page. The Privacy Policy matches the site in these respects: no advertising or analytics scripts; the Hostinger Reach script (`cdn-reach.hostinger.com`) does load. Points to fix before publishing: page 3 has pings `open` (policy: no pingbacks); the Comments paragraph is conditional ("if comments are turned on") although comments are off site-wide; no contact method; the cookie statement for visitors is not verified; About has no operator, contact or non-affiliation statement.

**Decisions (user, 2026-10-08).**

1. Public author name is `Stateside Explained`; the byline stays.
2. Create a new site-only administrator account (public display name `Stateside Explained`); move the 12 articles and the pages to it; propose how to retire `admin` separately, after the move is done and checked.
3. The personal Gmail is not published. A site-only address of the form `hello@statesideexplained.com` is created first; About and Privacy Policy are not published before it exists.
4. About gets a statement, in the gist of: "Stateside Explained is an independent informational website and is not affiliated with USPS, TSA, NIST, DOT, or any government agency."
5. About and Privacy Policy are linked in the footer only, not in the header.
6. `www` should 301-redirect to `https://statesideexplained.com/`; Claude gives the exact procedure first (below); no setting is changed yet.
7. The text of About and Privacy Policy is version-controlled in `content/pages/`; the existing WordPress drafts are moved there first and compared, then edited and published.

**Done in this step (repository only).** `content/pages/about.md` and `content/pages/privacy-policy.md` created from the WordPress drafts (page 9 and page 3, as last modified 2026-10-06). Check: the letters-and-digits text of each file equals the text of the WordPress draft (About 675 characters, Privacy Policy 1,654; same SHA-256 prefix on both sides). The only difference: the Hostinger link in the WordPress draft carries `rel="nofollow"`, which the Markdown file does not express. No wording was changed.

**Stages, each needing the user's separate approval before Claude touches WordPress.**

1. New account: create the administrator (username not `admin` and not guessable; public name and nickname `Stateside Explained`), set its URL slug so the author URL does not repeat the login name (for example `stateside-explained`), choose the account email. Open choices: the account email (the site-only address once it exists is preferred, so no personal address hash appears in the Gravatar URL), and whether the author archive stays (`noindex`) or is disabled.
2. Move authorship: the 12 articles (posts 14, 19, 22, 25, 28, 30, 34, 36, 40, 43, 45, 49), the 2 pages (9, 3) and the uploaded images. This updates each item's modified time (sitemap lastmod, JSON-LD dateModified), with no content change; recorded here so the 1-week and 4-week readings can account for it. Check afterwards on the public pages: byline, JSON-LD, social meta, feed, text unchanged, sitemap.
3. Retire `admin`: separate proposal after stages 1 and 2 are checked (including whether the hosting's WordPress login tools depend on that account).
4. Contact address: the user creates `hello@statesideexplained.com` (mailbox or forwarding); Claude records it. Claude does not enter any password.
5. Page text in the repository: update About (non-affiliation statement, contact) and Privacy Policy (contact and email handling, comments paragraph, cookie statement after the cookie check, pings) in `content/pages/`; optional English review; then Claude applies the text to the WordPress drafts, closes pings on page 3, and the user previews and publishes.
6. Footer links: after both pages are published, add the About and Privacy Policy links to the footer template part only.
7. `www`: redirect procedure below, done by the user (or by Claude only with explicit approval and access).

**`www` to non-`www` 301 redirect: procedure (not applied).**

0. Diagnose: open `https://www.statesideexplained.com/` in a normal browser and note the error (certificate warning, connection refused, timeout). Check in Cloudflare (the DNS answer shows Cloudflare name servers) that the zone exists and what the `www` record is.
1. Preferred path, in Cloudflare: make the `www` DNS record exist and be proxied (orange cloud); it is currently DNS-only. Leave the apex record as it is. Then create a Redirect Rule: when the hostname equals `www.statesideexplained.com`, redirect with status 301 to `https://statesideexplained.com` plus the same path, keeping the query string (Cloudflare's "redirect from www to root" template does this). A proxied `www` is answered by Cloudflare's own certificate, so the origin does not need a `www` certificate.
2. Fallback, at the host (Hostinger hPanel): make sure `www.statesideexplained.com` is attached to the site and the SSL certificate covers it, then redirect `www` to the root there (host redirect setting or `.htaccess`); WordPress's own canonical redirect would then also send `www` to the Site Address.
3. Do not add a second redirect for the same hostname (loop risk), and do not change WordPress Address or Site Address.
4. Test afterwards (Claude can check): `https://www.statesideexplained.com/` and `.../usps-mail-forwarding-how-long/` end at the non-`www` HTTPS URL with one 301 hop; `http://www...` ends at the same place; the apex pages, canonical, `robots.txt` and `sitemap_index.xml` are unchanged; no redirect loop.
5. Rollback: delete the Redirect Rule or set the `www` record back to DNS-only.
6. Search Console: use a URL-prefix property for `https://statesideexplained.com/`; a Domain property would need a DNS TXT record (in Cloudflare).

No article, diagram, page or WordPress setting was changed in this step. Counts unchanged: published 12; ready 0; draft 0.

## 2026-10-08 — Author display: new account and authorship move put on hold; smaller path chosen

The user put stages 1 and 2 of the site cleanup (new administrator account, moving the 12 articles, the pages and the images to it) **on hold** and chose a smaller path: keep the existing `admin` account, change its public display name to `Stateside Explained`, and, once the site-only address `hello@statesideexplained.com` exists, change the account email to that address. About and Privacy Policy stay version-controlled in `content/pages/`. Decisions 1, 3, 4, 5, 6 and 7 of the previous entry are unchanged; decision 2 is replaced by this one. Retiring or renaming `admin` is not planned now.

**Investigation of the byline (Claude, read-only; nothing was changed).**

- Theme: Twenty Twenty-Five 1.5 (active, no child theme).
- The only template that outputs an author is the theme's `single` template (`twentytwentyfive//single`, source `theme`, not customized). It contains one block, inside the group "Written by": `<!-- wp:post-author-name {"isLink":true} /-->`, which renders "Written by [name linked to `/author/admin/`] in [category]". The home page, the page-2 listing, the category archive and the search results show no author (zero author blocks and zero `/author/admin/` links). The `footer` template part is already customized (stored in the database since 2026-10-06); no header or footer part contains an author block.
- On a post page `/author/admin/` appears 4 times: the byline link (1) and the JSON-LD (3: Person `@id`, Person `url`, BlogPosting author `@id`).
- Public pages are served from the LiteSpeed page cache (`x-litespeed-cache: hit`), so a template or profile change may not show to logged-out visitors until the cache is purged.

**Smallest change to the link.** In the `single` template, change that one block to `<!-- wp:post-author-name {"isLink":false} /-->`. Result: "Written by Stateside Explained in [category]" with the name as plain text (the "Written by" row, the category link and the layout stay). Done in the Site Editor (Appearance, Editor, Templates, the single-post template; select the author name; in the block settings turn off "Link to author archive"; Save) or through the templates REST endpoint with the same one-attribute change. Saving creates a customized copy of the template in the database (like the footer); theme updates will not overwrite it, and "Clear customizations" on that template restores the theme version. No post is edited, so no post modified time or sitemap lastmod changes. Hiding the whole row is a larger change (three blocks: "Written by", the author name, the word "in"; the category link would need to be kept), and hiding the name with CSS leaves the link in the HTML and is not recommended.

**What this does not change.** The `/author/admin/` URL stays in the JSON-LD (3 places) and the author archive stays open (`noindex`). Changing the author URL slug (not the display name) would remove the login name from those URLs; that is a separate, optional step.

**Changing the display name.** Done on the `admin` profile (nickname and the public display name set to `Stateside Explained`; in the profile screen the public-name dropdown only offers names built from the first name, last name, nickname and username, so the nickname is set first) or by the users REST endpoint (`name`). It changes the name text in the byline, the JSON-LD Person and BlogPosting author names, the social meta "Written by", the feed `dc:creator` and the author archive heading.

**Changing the account email later.** WordPress sends a confirmation message to the new address, so the `hello@` mailbox must exist and be readable first. The site Administration Email (Settings, General) is separate and is also a personal address; it is not public, but WordPress notices go there. The JSON-LD image is a Gravatar URL derived from the account email, so it changes with the email.

**Proposed order (each step only after the user's approval).**

1. Display name of `admin` to `Stateside Explained`; purge the LiteSpeed cache; verify.
2. Template change `isLink` true to false; purge the cache; verify.
3. After the `hello@` mailbox exists: account email change (confirm via the new inbox), then decide about the Administration Email.
4. Optional later: author URL slug, a separate decision.

**Verification after step 1 (logged-out requests, cache-busted).** Byline text, JSON-LD `name` values, `twitter:data1`, feed `dc:creator` and the author archive heading all read `Stateside Explained` on all 12 posts; no `admin` text remains in those places (the URL `/author/admin/` may remain); post text, canonical, meta description and post modified times unchanged.

**Verification after step 2.** On all 12 posts: the byline has no link (no `<a>` containing `/author/admin/` in the page body; `/author/admin/` appears 3 times, all in JSON-LD); the "Written by" row still shows "Written by", the name and "in" plus the category link, same order; no new elements; phone-width layout unchanged (screenshot of one post); home, category and search pages unchanged; the template record shows the new attribute and source `custom`; post modified times and sitemap lastmod unchanged; the 12 article texts equal the repository texts.

**Verification after step 3.** The profile shows the new email; the Gravatar URL in the JSON-LD changes; Search Console, Rank Math and Wordfence notices go to the intended address.

No WordPress setting, theme template, article or page was changed in this step. Counts unchanged: published 12; ready 0; draft 0.

## 2026-10-08 — Author display name changed to `Stateside Explained` (step 1); cache purged; verified

With the user's approval for step 1, Claude changed the public name of the existing `admin` account through the users REST endpoint: `name` (public display name) and `nickname` both from `admin` to `Stateside Explained`. Nothing else in the profile was sent. Unchanged and re-read afterwards: login name `admin`, URL slug `admin` (author URL `/author/admin/`), account email, first and last name (empty), role administrator. No post, page, theme template or other setting was changed. (Noted, not changed: the profile's Website field is `http://statesideexplained.com`, with `http`.)

Cache: LiteSpeed "Purge All - LSCache" (page cache only) was run from the admin bar link; a public post page then returned `miss` and the next request `hit`.

Verification (logged-out requests, canonical URLs, after the purge, against a baseline taken before the change):

| Check | Result |
|---|---|
| Visible byline on all 12 posts | `Stateside Explained` (before: `admin`); still a link to `/author/admin/` (step 2 removes the link) |
| JSON-LD author Person `name`, BlogPosting author `name` (12 posts) | `Stateside Explained`; Person `url` still `/author/admin/` |
| Social meta `twitter:data1` (12 posts) | `Stateside Explained` |
| Feed `dc:creator` | `Stateside Explained` (no `admin` text left in the feed) |
| Author archive | heading `Author: Stateside Explained`; robots `follow, noindex`; title `Stateside Explained - Stateside Explained` (the site name repeats because the archive title format is name plus site name; noindex, left as is) |
| Visible text on a post page | no standalone `admin` outside styles and scripts; the 15 remaining occurrences in the HTML are CSS variable names (`--wp-admin-...`) and the `/wp-admin/*` path in the JSON |
| `/author/admin/` count per post page | still 4 (byline link and 3 in JSON-LD), as expected |
| Canonical, meta description, robots on 12 posts | unchanged (index, follow) |
| Article text on 12 posts (letters and digits) | same count as before the change |
| Post modified times (REST) | unchanged |
| Home page | no author links |

Open for the next steps: step 2 (remove the link in the `single` template; needs the user's approval), step 3 (account email after `hello@` exists), and the optional author URL slug. The 1-week checkpoint note: no post changed, so no sitemap lastmod changed. Counts unchanged: published 12; ready 0; draft 0.

## 2026-10-08 — Byline link removed (step 2); profile Website corrected; cache purged; verified

With the user's approval for step 2, Claude made two WordPress changes and nothing else.

1. **Template `single` (twentytwentyfive//single).** Through the templates REST endpoint, the single occurrence `<!-- wp:post-author-name {"isLink":true} /-->` was replaced by `<!-- wp:post-author-name {"isLink":false} /-->`. The rest of the template content is byte-identical (length +1 character). The record now shows source `custom` (before: `theme`); it is the only customized template. To undo: Site Editor, Templates, Single Posts, Clear customizations.
2. **Profile Website (user id 1).** `url` changed from `http://statesideexplained.com` to `https://statesideexplained.com/`. Only `url` was sent. Re-read afterwards: login `admin`, slug `admin`, display name and nickname `Stateside Explained`, role administrator unchanged; email not touched.

Cache: LiteSpeed "Purge All - LSCache" run from the admin bar link, then verified.

Verification (logged-out requests, cache-busted, on all 12 posts; baseline taken before the change):

| Check | Result |
|---|---|
| Byline row text vs baseline | identical on 12/12 ("Written by Stateside Explained in [category]", same order) |
| Link to `/author/*` inside the byline row | 0 on 12/12 (before: 1) |
| Category link in the row | same URL as baseline on 12/12 |
| `/author/admin/` count per post page | 3 on 12/12, all in JSON-LD (before: 4) |
| JSON-LD author name occurrences | `Stateside Explained` present on 12/12 |
| Canonical equals the post URL; robots | 12/12; `index, follow` |
| Post modified times (REST) | unchanged on 12/12 |
| Home, page 2, three category pages, `?s=usps` | no author block and no `/author/admin/`; they were not affected by a `single` template change |
| Author archive | `noindex`, title unchanged; feed `dc:creator` `Stateside Explained`; post sitemap 13 URLs |
| Phone-width screenshot of one post | row reads "Written by Stateside Explained in Postal service and stamps"; name is plain text; layout intact |
| Pages 3 and 9 | still `draft`, modified times unchanged |

Not reproduced, stated honestly: the pre-change baseline stored a body text length/hash and per-page hashes of home, category and search pages, but the measuring method was not kept in a form that could be repeated exactly, so those numbers could not be compared. They were replaced by the checks above (modified times unchanged, REST content untouched because no post was written, byline row text and links compared directly, the non-post pages containing no author block). The planned comparison of the 12 article texts with the repository files was not run. No post was written, so a change there is not expected.

Still open: step 3 (account email after the `hello@statesideexplained.com` mailbox exists; the user will request it separately), the Administration Email, the optional author URL slug, About and Privacy edits, the `www` 301, Search Console. Counts unchanged: published 12; ready 0; draft 0.

## 2026-10-08 — Site-only mailbox `hello@` created; account email and Administration Email changed (step 3); verified

**Mailbox.** Hostinger offered only a 12-month trial of a paid email product that auto-renews, so it was not started (no email subscription exists; the hosting plan is Premium Web Hosting, auto-renewal on). Instead the user enabled Cloudflare Email Routing for `statesideexplained.com`: a rule forwards `hello@statesideexplained.com` to the owner's personal mailbox; catch-all is disabled (Drop). Cloudflare added three MX records, one SPF TXT (`v=spf1 include:_spf.mx.cloudflare.net ~all`) and a DKIM TXT; these are locked (managed by Email Routing). The user confirmed that a test mail to `hello@` arrived. The unused Hostinger domain-verification TXT was selected for deletion by the user. The domain itself is registered at another provider (shown as such in the Hostinger panel); its renewal date has not been checked yet. Reply-from-`hello@` is not set up (receive only).

**Change (user chose "account email + administration email").** Through the REST endpoints: `users/1` `email` and `settings` `email` (Administration Email) both set to `hello@statesideexplained.com`; both calls returned 200 and applied immediately (no confirmation mail was involved on this route). Login `admin`, slug `admin`, display name `Stateside Explained`, role administrator, Website `https://statesideexplained.com/` unchanged. No post, page, template, plugin or other setting was touched. LiteSpeed "Purge All - LSCache" was run afterwards.

**Verification (logged-out, 12 posts plus home, feed, author archive, REST root).** All 12 posts HTTP 200 with the byline `Stateside Explained` and `/author/admin/` 3 times (JSON-LD only); no `gmail.com`, personal address text or `hello@` text appears in any of those pages (the address is not published yet); `/wp-json/wp/v2/users` is 401 for anonymous requests. The JSON-LD Gravatar hash is identical on all 12 posts and equals SHA-256 of `hello@statesideexplained.com`, so the old personal-address hash is gone from the markup.

Still open: About and Privacy edits (non-affiliation statement, contact `hello@`, comments paragraph, pings, cookie check), publish, footer links; `www` 301; Search Console; domain renewal date at the registrar; optional DMARC record; optional Gmail "send as" for replies; optional two-factor authentication on the hosting account. Counts unchanged: published 12; ready 0; draft 0.

## 2026-10-08 — About and Privacy Policy source text revised in `content/pages/` (WordPress drafts not yet updated)

Edited only the repository files; the WordPress drafts (page 9 About, page 3 Privacy Policy) are unchanged and still drafts. Front matter gained `content_revised: 2026-10-08` and `wp_applied: false`.

**About.** Added the non-affiliation sentence ("Stateside Explained is an independent informational website and is not affiliated with USPS, TSA, NIST, DOT, or any government agency.") and a Contact section with `hello@statesideexplained.com`. No operator name was added (open decision for the user). The FAA is not in the user's list although one article cites it; left as decided.

**Privacy Policy.** Date set to October 8, 2026. Changes and the checks behind them:

| Change | Basis |
|---|---|
| "does not offer visitor accounts, newsletter signup, comments or contact form" | no forms on the home page or on two posts (0 `<form>`); comments disabled by policy |
| Hostinger Reach wording from "may load" to "loads" | `cdn-reach.hostinger.com` script and stylesheet found on the home page and on two posts |
| Added Cloudflare (DNS and email routing) | DNS is at Cloudflare in DNS-only mode; Email Routing forwards `hello@` |
| New section "If you email us" | the mailbox exists; text states what is received and that it is used only to answer; no retention period was claimed |
| Comments paragraph replaced by "comments are turned off" | the earlier conditional text was inaccurate for this site |
| Cookie paragraph: removed the commenter clause | comments off. The statement that readers get no login cookie is unchanged and is still not verified in a logged-out browser (needs the user's incognito check of Application, Cookies) |
| Changes section now lists comments and contact form | consistent with the above |
| No analytics or advertising script | external hosts found on the pages were only `cdn-reach.hostinger.com`; `secure.gravatar.com` appears only as an image URL string inside JSON-LD |

Front matter records `wp_ping_status_target: closed` (page 3 still has pings open in WordPress; to be closed when the text is applied).

Next, each only with the user's approval: optional English check by ChatGPT; apply the text to the two WordPress drafts and close pings on page 3; the user publishes; footer-only links; live QA. Counts unchanged: published 12; ready 0; draft 0.

## 2026-10-08 — Cookie check result and Privacy Policy cookie wording

The user checked a logged-out private window (browser DevTools, Application, Cookies) on the home page. One cookie was present: `__cf_bm`, domain `.hostinger.com` (not `statesideexplained.com`), path `/`, Secure, HttpOnly, SameSite None, expiry about 30 minutes after setting (2026-10-08T03:48:59Z shown). No WordPress login or comment cookie. Conclusion: the statement that readers do not get a login cookie holds, and the only cookie comes from a Hostinger domain, consistent with the `cdn-reach.hostinger.com` script found earlier.

`content/pages/privacy-policy.md` Cookies section now says that the Hostinger Reach script may cause a short-lived bot-protection cookie (`__cf_bm`) from a Hostinger domain, that it is not used for tracking or ads by the site, and that the site does not control it. Not yet applied to WordPress (see the previous entry). Also noted, not changed: no site icon is set (`/favicon.ico` returns 404); an optional fix in Appearance, needs approval. Counts unchanged: published 12; ready 0; draft 0.

## 2026-10-08 — About and Privacy Policy: five Gate 2 wording fixes applied to the repository text

Applied exactly as supplied by the user after ChatGPT's Gate 2 review: (1) About opening paragraph; (2) About disclaimer first sentence now "The content on Stateside Explained is for general information only. It is not legal, medical, financial, or travel advice." (the sentence after it, "For a decision that matters...", is unchanged); (3) About Contact paragraph; (4) Privacy opening paragraph; (5) Privacy cookie sentence now "We do not set or use this cookie for advertising or analytics, and we do not control it." Only `content/pages/about.md` and `content/pages/privacy-policy.md` changed. The WordPress drafts remain unchanged and unpublished; final Gate 2 check is by the commit SHA of this change. Counts unchanged: published 12; ready 0; draft 0.

## 2026-10-08 — About and Privacy Policy text applied to the WordPress drafts (Gate 2 PASS at `5c72d19`)

ChatGPT's final Gate 2 for About and Privacy Policy passed at commit `5c72d19`. With the user's approval, Claude applied the text to the two WordPress **drafts** only: page 9 (About) and page 3 (Privacy Policy). Nothing was published and no footer link was added.

**What was written.** Through the pages REST endpoint: `content` for both pages, and `ping_status: closed` for page 3 (it was `open`; page 9 was already `closed`). No other field was sent. Status, slug, title, comment status, parent and template are unchanged (re-read and compared). The Markdown was fetched from `raw.githubusercontent.com` at the full SHA and its SHA-256 matched the local file (About `d589e71b…`, Privacy `b63d66dd…`) before conversion. Conversion to blocks follows the format of the earlier drafts (paragraph, heading, list blocks); the Hostinger privacy-policy link keeps `rel="nofollow"` as in the earlier draft; the cookie name is a `<code>` element.

**Verification.**

| Check | About (9) | Privacy (3) |
|---|---|---|
| Stored block content equals the generated content | yes | yes |
| Text of headings, paragraphs and list items vs repository Markdown (syntax removed by a separate routine) | identical, 11 items, 1,211 characters | identical, 21 items, 2,656 characters |
| Preview render (logged-in) matches the Markdown text after typographic-quote normalisation | yes, 11 of 11 | yes, 21 of 21 |
| Status | draft | draft |
| Ping status | closed | closed (changed from open) |
| Anonymous request to `?page_id=` | 404, no content | 404, no content |
| In the page sitemap | no | no |
| Hostinger link `rel=nofollow`, `<code>` present | n/a | yes |

The 12 published posts were not touched (latest modified time still 2026-10-07T20:11:36). Preview URLs (login required): `https://statesideexplained.com/?page_id=9&preview=true` and `https://statesideexplained.com/?page_id=3&preview=true`.

Front matter of both files was updated to `wp_applied: true`, `wp_applied_from_commit: 5c72d19`, `wp_modified_at_apply: 2026-10-08T01:19:42`; the body text is unchanged from `5c72d19`. Next, only with the user's approval: the user previews and publishes both pages, then footer-only links (template part `footer`), then live QA (logged-out render, sitemap, Rank Math noindex/index state, canonical). Open items elsewhere: `www` 301, Search Console, domain renewal date, favicon. Counts unchanged: published 12; ready 0; draft 0.

## 2026-10-08 — About and Privacy Policy published; live QA passed; footer links added; header side effect found

The user published page 9 (About, 2026-10-08 01:35:46 site time) and page 3 (Privacy Policy, 01:35:57). Live URLs: `https://statesideexplained.com/about/`, `https://statesideexplained.com/privacy-policy/`. (Earlier in the session the user was looking at the Posts list instead of Pages; the pages had still been drafts at that moment.)

**Live QA (logged-out).** Both pages: HTTP 200 (first request a cache miss, then hit); text of headings, paragraphs and list items identical to the repository text at `5c72d19` (11 and 21 items); one `h1` each; canonical equals the page URL; title `About - Stateside Explained` / `Privacy Policy - Stateside Explained`; robots `index, follow`; no comment form, no author block; `hello@statesideexplained.com` is shown, no personal address or `gmail.com` anywhere in the HTML; the Hostinger link is `nofollow noopener`; phone-width view of the Privacy page renders normally. `page-sitemap.xml` now lists the home page, `/privacy-policy/` and `/about/`; `robots.txt` points to `wp-sitemap.xml`, which redirects to `sitemap_index.xml` (works).

Notes (not changed): (a) Rank Math auto-generated meta descriptions are weak: About's is cut mid-sentence ("...how common services"), Privacy's is just "Last updated: October 8, 2026."; setting both by hand would need the user's approval. (b) Both pages carry `Article` among their JSON-LD types, Rank Math's default for pages; left as is. (c) Both pages are indexable; the Privacy Policy could be set to noindex if the user prefers (a choice, not applied).

**Footer.** With the user's approval, one paragraph block was inserted into the `footer` template part, after the `© 2026 Stateside Explained` paragraph: `About · Privacy Policy`, two absolute links. Nothing else in the part changed (the stored content equals the original plus exactly that block). LiteSpeed "Purge All - LSCache" was run. Check on 20 URLs (home, page 2, About, Privacy, three categories, search `usps`, the 12 posts): HTTP 200 on all; the footer contains each link exactly once; the `© 2026` text and the WordPress credit are intact; no personal address; both links return 200.

**Side effect found, not fixed.** The header navigation (Navigation post 5, content `<!-- wp:page-list /-->`) automatically lists every published page, so About and Privacy Policy now also appear in the header menu on all pages. This contradicts the decision that both links live in the footer only. Fix options, each needing the user's approval: (1) set Navigation 5 content to empty; (2) remove the navigation block from the header template part; (3) accept the header links. Option 1 is the smallest change but its effect on the empty mobile menu button must be checked after the change. Counts unchanged: published 12 posts, 2 pages; ready 0; draft 0.

## 2026-10-08 — Header Navigation block removed; Rank Math descriptions set for About and Privacy; verified

The user chose "remove the Navigation block from the header template part" for the header side effect (the page-list menu had started listing the two new pages after they were published), and supplied the meta descriptions for About and Privacy Policy.

**Changes (REST).**
1. Template part `header` (`twentytwentyfive//header`, was theme default, now `custom`): removed exactly one line, `<!-- wp:navigation {...} /-->` (160 characters; the stored content equals the original minus that line). The site title block and all other groups were left as they were. The wrapper group around the removed block remains (it is empty and takes no space). Navigation post 5 (`<!-- wp:page-list /-->`) was not touched and is simply no longer used by the header.
2. Rank Math description (`updateMeta`, only `rank_math_description`): About: "Learn how Stateside Explained uses official sources and clear diagrams to answer everyday U.S. questions." Privacy Policy: "Read the Stateside Explained Privacy Policy, including how this site handles email, cookies, hosting, and security." No robots or schema setting was sent.
3. LiteSpeed "Purge All - LSCache".

**Verification (logged-out, cache-busted, 20 URLs: home, page 2, About, Privacy, three categories, search `usps`, the 12 posts).** HTTP 200 on all; no `<nav>` and no menu button in the header; no link to About or Privacy in the header; the footer contains each of the two links exactly once; the site title is present; the WordPress credit is intact; no personal address in the HTML. About and Privacy: `description`, `og:description`, `twitter:description` and the JSON-LD description all equal the supplied text; title, canonical, robots (`index, follow, ...`) and the JSON-LD type list (including `Article`) are identical to the values measured before the change. Layout, measured in an embedded frame before and after (home, one post, About at 1280 px and 375 px width): header box and site title position identical to the pixel, page heading position identical, so no empty space or shifted content; no menu button remains. A phone-width view of About shows the site title alone in the header and the footer line `© 2026 Stateside Explained · About · Privacy Policy` followed by the WordPress credit. The 12 posts were not touched (latest modified still 2026-10-07T20:11:36). Note: the 375 px measurement reported horizontal scroll for the home page and one post both before and after the change; no element wider than the viewport was found at the pane width, so it looks like a measuring artifact of the embedded frame and is not related to this change.

Open items elsewhere: `www` 301, Search Console and sitemap submission, domain renewal date at the registrar, favicon, optional DMARC and Gmail send-as, optional two-factor authentication on the hosting account. Counts unchanged: published 12 posts, 2 pages; ready 0; draft 0.

## 2026-10-08 — Search Console setup recorded (user-reported facts only)

The user reported that on 2026-10-08 (user's local date) they completed three things in Search Console: domain-property verification, submission of `https://statesideexplained.com/sitemap_index.xml`, and an indexing request ("Request indexing") for the home page. Source label: `사용자`. Claude did not access Search Console and did not check these; no Search Console screen values (sitemap status, discovered URL count, coverage numbers) are recorded here. The user will record screen values at the 1-week checkpoint (on or after 2026-10-14).

Recorded in `docs/pilot-evaluation.md`: table E rows (property verification, property type = domain property, sitemap submission, new row for the home-page indexing request), the note under section 4 step 5, and the open-decision items in section 9. Caveat noted there: the indexing request was reported for the home page only (none reported for the 12 posts); because the home page links to the posts, an early home crawl can speed up discovery of the posts, so the 1-week notes in tables B/C should mention it. Table E's "홈·카테고리·About·Privacy 상태" cell still says About/Privacy are drafts (written before publication); the 1-week column will carry the current state. Counts unchanged: published 12 posts, 2 pages; ready 0; draft 0.

## 2026-10-08 — `www` to apex redirect (Cloudflare) verified, with one gap

The user changed the `www` CNAME to Proxied and deployed a `www` → apex 301 Redirect Rule in Cloudflare (done by the user; Claude made no change and has no Cloudflare access). Claude then checked from the built-in browser pane.

**Method and limits.** The pane can navigate and read the final page but cannot see redirect status codes or hop counts: the network log lists only the final document, the navigation timing `redirectCount` is 0 for cross-origin redirects, and scripted requests to the `www` host are blocked from the apex page. The device shell and cloud shell cannot reach the site (proxy 403). So final destinations and final status were verified; **the 301 status code and the "exactly one hop" part of the success criteria were not verified by Claude** and need a `curl -sIL` run by the user (or a Cloudflare rule screenshot showing status 301).

**Final destinations (navigation to the `www` URL; the final address, final status 200 unless noted).**
- `https://www.statesideexplained.com/` → `https://statesideexplained.com/` (200, canonical equals the final URL)
- `https://www.statesideexplained.com/usps-mail-forwarding-how-long/` → same path on the apex (200, canonical equals)
- `https://www.statesideexplained.com/category/postal-service-and-stamps/` → same path on the apex (200, canonical equals)
- `https://www.statesideexplained.com/?s=usps` → `https://statesideexplained.com/?s=usps` (200, query kept)
- `http://www.statesideexplained.com/` → `https://statesideexplained.com/` (200)
- `https://www.statesideexplained.com/robots.txt` → apex `robots.txt` (200, text/plain, content as before: disallows `/wp-admin/`, allows `admin-ajax.php`, `Sitemap: https://statesideexplained.com/wp-sitemap.xml`)
- `https://www.statesideexplained.com/sitemap_index.xml` → apex `sitemap_index.xml` (200; lists `post-sitemap.xml`, `page-sitemap.xml`, `category-sitemap.xml`, all on the apex)
- Extra: `https://www.statesideexplained.com/about/` → apex `/about/` (200); a nonexistent path on `www` → the same path on the apex with the WordPress 404 page (404 preserved, no redirect to the home page).
- No redirect loop appeared in any of these (every navigation ended on a loaded apex page).

**Apex unchanged (scripted fetch, no cookies, no redirect following, cache bypassed).** Home, the 12 posts, About, Privacy Policy, the 3 category pages: all 200 with no redirect; canonical equals the requested URL on all 18; robots meta `index, follow` (posts and pages also `max-snippet:-1,...`) as before. Apex `robots.txt` and `sitemap_index.xml`: 200, no redirect. Site Address and WordPress Address were not touched. No page content hash was compared (no baseline hash was stored), so "unchanged" means status, canonical and robots meta only.

**DNS (DoH, dns.google).** `www` now answers with Cloudflare proxy addresses (104.21.31.107, 172.67.176.57), no CNAME is exposed, i.e. it is proxied; the apex still answers `31.170.160.71` (DNS only, unchanged). Mail records preserved: MX route1 / route2 / route3 `.mx.cloudflare.net` (three records); SPF `v=spf1 include:_spf.mx.cloudflare.net ~all`; DKIM at `cf2024-1._domainkey` present (`v=DKIM1; h=sha256; k=rsa; p=...`); the `google-site-verification` TXT (Search Console) is also present. A mail delivery test to `hello@` was not repeated.

**Result.** Final-destination, query-string, http→https, `robots.txt` and sitemap criteria met; apex unchanged; mail DNS records preserved. Not verified: 301 (versus 302/308) and the single-hop count. Still open: that `curl` check by the user; Search Console may still show `www` URLs in its reports for a while (no action). Note: `docs/pilot-evaluation.md` table E row "`www` 주소" still says the address does not open (written before this change); update it at the 1-week checkpoint. Counts unchanged: published 12 posts, 2 pages; ready 0; draft 0.

## 2026-10-08 — `www` redirect: 301 status and single hop confirmed (user-run curl)

The user ran `curl.exe -sIL` from their own computer (output pasted in chat, 2026-10-08 06:18 GMT) and so closed the gap left in the previous entry. Results (source: user-run command; Claude did not run it):

| Request | Hop 1 | Hop 2 |
|---|---|---|
| `https://www.statesideexplained.com/usps-mail-forwarding-how-long/` | `301 Moved Permanently`, Location `https://statesideexplained.com/usps-mail-forwarding-how-long/` (Server: cloudflare) | `200 OK` (Server: LiteSpeed, `X-LiteSpeed-Cache: hit`) |
| `https://www.statesideexplained.com/?s=usps` | `301`, Location `https://statesideexplained.com/?s=usps` (query kept) | `200 OK` (not cached: `no-cache` headers on search) |
| `http://www.statesideexplained.com/` | `301`, Location `https://statesideexplained.com/` (straight to https apex, no intermediate http hop) | `200 OK` (cache hit) |

Success criteria from the procedure are now all met: 301 (not 302/308), exactly one redirect hop in each case, query string kept, final status 200, no loop, apex pages/canonical/`robots.txt`/`sitemap_index.xml` unchanged (previous entry), mail DNS records preserved (previous entry). Cloudflare's reporting headers in the output were not copied into the repository. `docs/pilot-evaluation.md`: table E row "`www` 주소" and the section 9 line on `www` were updated to this state. Remaining open items elsewhere: domain renewal date at the registrar, favicon (404), optional DMARC, Gmail send-as, two-factor authentication on the hosting account, the 1-week checkpoint (on or after 2026-10-14), DST source re-check before 2026-11-01, 4-week evaluation (on or after 2026-11-04). Counts unchanged: published 12 posts, 2 pages; ready 0; draft 0.

## 2026-10-13 — Homepage and navigation redesign: design decided, nothing applied

Context: the user is concerned that a site made only of articles and diagrams looks like an AI-generated blog (reference: the CleanSheetHQ homepage, which has an intro, category groups, a menu and a footer). Claude looked at the current homepage (read-only): it is the default "Blog" listing, with no intro, no category grouping and no header menu, and it shows full article text. This is treated as a structure problem (also duplicate full text on the homepage), not decoration. No change has been made to WordPress or the theme. Implementation starts only after the 1-week Search Console values (on or after 2026-10-14) are recorded in `docs/pilot-evaluation.md`, and each step needs the user's approval.

**Decisions by the user (2026-10-13).**
1. Homepage: build a new static Page and set it as the homepage (URL `/` unchanged). Consequence to handle: the homepage moves from the post sitemap to the page sitemap, so its Rank Math title and meta description must be set.
2. Cards show the real publication date in small text (no invented or backdated dates; all 12 posts are dated 2026-10-07, so the same date repeats).
3. Accent colour: dark teal `#2F5D62`; white background; no flag/seal/government-style imagery.
4. Intro copy: first check all 12 posts for a sources list and a stated check date; only claims that are true for all 12 stay in the final text. Draft: "Stateside Explained answers practical questions about U.S. mail, airport rules, and the calendar. Each article is based on official sources, lists them at the end, and says the date we checked them. This is an independent site and is not affiliated with USPS, TSA, or any government agency. For anything that affects your travel or mail, check the agency's own page." No operator name, credentials, testimonials or "expert" wording.
5. AI-use wording: not added to About for now.
6. Post-bottom links, first round: only `More in [category] →`. Same-category previous/next only if the default blocks can actually restrict it to the same category; Claude checks this and proposes it separately. Hand-picked related links in post bodies wait until after the 4-week evaluation (separate approval, edits published posts).

**Layout agreed.** Homepage: short intro, then three category sections (Airport security rules, Postal service and stamps, US dates seasons and holidays; names to be confirmed against the existing categories; the assignment of the 12 posts is inferred from slugs and must be checked), 4 text cards each in 2 columns on desktop and 1 on mobile; each card has category label, title link, excerpt of about 25-30 words taken from the first paragraph (no change to post bodies), small date, "Read →"; thin border, no shadow, no card images in round one; a link to the category archive per section. Category filter in the list blocks must set both `categoryIds` and `taxQuery` (lesson from CleanSheetHQ). Header: a hand-built menu of three category links (not an automatic page list, which caused the About/Privacy side effect on 2026-10-08), labels such as `Airport rules · Mail & stamps · Dates & holidays`; About and Privacy stay in the footer only; check the mobile menu button. Also check that category archive pages show excerpts and not full text.

**Planned order (each step with approval).** (1) Check the 12 posts for sources and check dates, finalize intro. (2) Build the static homepage as a draft, review, publish, purge LiteSpeed cache. (3) Header menu. (4) Date and `More in [category] →` on the post template. (5) Logged-out verification of the 12 posts, homepage, categories, About and Privacy, then a decision-log entry and local commit. Post bodies are not edited in this round. Pilot note: the homepage change does not alter post pages and every post stays linked from the homepage; record the change date next to the 1-week and 4-week observations.

## 2026-10-13 — New-article work resumed: article 13 selected (alcohol on a plane); brief, sources, draft and Gate 1 done

**User instruction (2026-10-13).** The 1-week checkpoint stays as planned (record the Search Console values on or after 2026-10-14), but new-article writing restarts today. Today: research 2-3 candidates for the 13th article from official sources, pick the safest evergreen question, take it to brief and draft. Thanksgiving articles may be prepared as drafts, but their publication requires re-reading this year's TSA/USPS notices. The homepage restructure still waits for the 1-week values.

**Candidates read (official pages opened in the built-in browser on 2026-10-13).**
1. Alcohol on a plane: TSA "Alcoholic beverages" (updated Feb 20, 2025), FAA PackSafe "Alcoholic Beverages" (updated Apr 13, 2026), 49 CFR 175.10(a)(4) on eCFR (title 49 up to date as of 10/08/2026). Short sources that agree on every number. **Selected.**
2. Lighters on a plane: five TSA pages with type-specific rules and special instructions; more nuance, overlaps the power-bank material. Kept as `idea` (reserve), row 17.
3. What is a ZIP+4 code: no clear consumer-facing official explainer; recorded as rejected with the reason.

**Selected: `alcohol-on-a-plane-tsa-faa`** ("Can You Bring Alcohol on a Plane? What TSA and the FAA Say", focus keyword `can you bring alcohol on a plane`, lane airport security rules, rule-type: mandatory re-check). Files: `research/briefs/`, `research/sources/`, `content/drafts/`, `editorial/qa/` (all `alcohol-on-a-plane-tsa-faa.md`). The draft is about 800 words including front matter. Quoted source statements were tested by script against the live pages (TSA 11 of 11, FAA 9 of 9, eCFR 6 of 6). Gate 1: 20 of 20 claims pass. Careful points: the article states **no rule for beverages over 70% alcohol** (the FAA page text under "Alcoholic Beverages Over 140 Proof" has a definition and a regulation link but no rule, and the TSA page is silent; the regulation's exception, as written, covers up to 70% alcohol by volume); "alcohol" (TSA) versus "alcohol by volume" (FAA, regulation) is said once; the 3-1-1 article is linked once for the general carry-on rule.

**Status and limits.** Stage `draft`. Not sent to Gate 2, not approved, not on WordPress, not published. No diagram or image alt text yet (front matter `pending`). Search demand and competition not measured. Post-pilot article: it is **not counted** in the pilot 12; if it is published during the pilot window, note its publication date next to the 1-week and 4-week observations. The 13th article does not change the pilot result, which is read from the 12 `published` rows only.

**Thanksgiving briefs.** Rows 8 (`tsa-thanksgiving-food-carry-on`) and 12 (`usps-post-office-thanksgiving`) now carry the condition in `docs/content-backlog.md`: draft preparation is allowed, but before any publication the 2026 TSA / USPS notice must be re-read (mandatory), not the 2025 text.

**Access note.** The built-in browser needed one-time access grants for ecfr.gov (two page loads); no other site-level changes were made. Counts: published 12 posts, 2 pages; ready 0; draft 1 (post-pilot); briefs 2 deferred; ideas 2.

## 2026-10-13 — Article 13 (alcohol-on-a-plane-tsa-faa) revised: over-70% rule stated, diagram and alt text made, Gate 1 re-run

**User instruction (2026-10-13).** Before Gate 2, add the over-70% beverages: using TSA's "Alcoholic beverages over 140 proof" entry and the FAA's official guidance, state in the body, table, source notes and Gate 1 that beverages over 70% alcohol (over 140 proof) are not allowed in carry-on or checked bags. Confirm that the 5 L for over 24% up to 70% is a total per passenger, limit the 24%-or-less wording to a scoped statement such as "TSA: no separate alcohol limit for checked bags", keep the airline-check line, then make the diagram and alt text and re-pass Gate 1; the user will request Gate 2 on the resulting commit.

**What was checked (2026-10-13).**
- TSA "Alcoholic beverages over 140 proof" (page shows "Last Updated on February 20, 2025"): "Carry On Bags: No", "Checked Bags: No", the definition (more than 70% alcohol, including grain alcohol and 151 proof rum), a reference to 49 CFR 175.10(a)(4). Opened in the built-in browser; 7 of 7 quoted statements found by script.
- FAA PackSafe web page "Alcoholic Beverages" (Apr 13, 2026): re-checked; the heading "Alcoholic Beverages Over 140 Proof" and the regulation link exist, but the page text states **no rule**. My earlier assumption that this page states the prohibition was wrong and is corrected in the article ("its text does not state a rule").
- FAA PackSafe printable chart (PDF, "Updated: 11/14/25"): row for over 140 proof says "Not allowed in Carry-On or Checked Bags"; under 140 proof: unopened retail packaging, 5 L per packaging and 5 L total per passenger, 100-ml carry-on footnote. **Read limit:** the PDF would not render in the browser pane (empty text, screenshot timeout), so it was read twice through a document-reader tool; the two reads agree. It was **not** opened directly and **not** script-tested. A direct open is mandatory before approval.
- 49 CFR 175.10(a)(4) (eCFR, up to date as of 10/08/2026): exception covers not more than 24% ABV, or more than 24% and not more than 70% in unopened retail packagings not exceeding 5 L, carry-on or checked, total net quantity 5 L per person. The article says the regulation's exception covers up to 70% and does **not** say the regulation itself prohibits stronger beverages.

**Changes in the article.** Lead and table now state the over-70% prohibition, attributed to TSA (lead) and TSA plus the FAA chart (section). New section "The 5-liter limit is a total per passenger" (TSA per passenger; FAA per packaging and total per passenger; regulation total net quantity per person). The 24%-or-less section is scoped: TSA's statement is about checked bags only, it does not change the carry-on limit or speak for any airline; the table row says TSA sets no separate alcohol limit for checked bags. The airline-check sentence is kept. Sources list: five pages. Meta description (134 characters) and alt text (313 characters) updated. Diagram `assets/raw/alcohol-on-a-plane-tsa-faa.svg` and `assets/optimized/alcohol-on-a-plane-tsa-faa.png` (1200 x 2286) made and viewed.

**Gate 1 (Claude, re-run).** 23 of 23 claims and 5 of 5 image checks pass; one open caveat (the FAA chart PDF read method; the over-70% rule is also stated by TSA's own entry). Files updated: brief, source notes (S4, S5 added), QA record, backlog row 16.

**Status and limits.** Stage `draft`. Not sent to Gate 2 by Claude, not approved, not on WordPress, not published; post-pilot, not counted in the pilot 12. Mandatory before approval: direct open of the FAA chart PDF and re-read of all five pages.

## 2026-10-13 — Article 13: pre-Gate-2 self-check by the writer; three wording fixes applied (not a Gate 2 pass)

**Context.** After commit `6ff8034`, Claude (the article's writer) checked the four points the user listed. This is a **self-check and is not recorded as Gate 2**; the independent Gate 2 is done by the user's other reviewer on the new commit, against the repository's actual draft, QA record and PNG.

**Decisions by the user (2026-10-13).** (1) Diagram: card title "over 24% to 70%" becomes "over 24% up to 70%". (2) Body: "without a quantity limit" becomes "does not state a quantity limit". (3) Alt text: include the "On board" card and the airline-check line, kept near 400 characters (now 402). (4) The focus keyword is not forced into the meta description or first sentence; the title and H1 carry it. (5) The FAA printable chart PDF stays a supporting source for this article; a direct open of the PDF is required right before publishing (the over-70% rule also rests on TSA's own entry). (6) Claude commits and pushes this revision and reports only the new SHA; the user explicitly asked for the push this time.

**Applied.** SVG and PNG regenerated (1200 x 2286, 115,201 bytes) and viewed; draft, alt (front matter and embed), QA record (Gate 1 re-run result unchanged: 23 of 23 claims, 5 of 5 image checks; new self-check section; Gate 2 still "not done"), brief and backlog row updated.

## 2026-10-13 — Article 13 (alcohol-on-a-plane-tsa-faa): independent Gate 2 PASS on `33aea2b`; conditions before `ready`

**Result (user-reported, 2026-10-13).** ChatGPT's independent Gate 2 on commit `33aea2b`: **PASS**. No change requested to the body, SEO, the diagram SVG or the alt text. Recorded in `editorial/qa/alcohol-on-a-plane-tsa-faa.md` and backlog row 16. The reviewer's own text is not stored in the repository; this entry records the result as relayed by the user.

**Stage.** Still `draft`. Not approved for `ready`, not on WordPress, not published. Post-pilot article, not counted in the pilot 12.

**Conditions kept (user decision).** Before the user approves the move to `ready`, re-read five pages: TSA "Alcoholic beverages", TSA "Alcoholic beverages over 140 proof", the FAA PackSafe web page, eCFR 49 CFR 175.10, and the FAA PackSafe printable chart. **The FAA PDF must be opened directly in a browser.** If it cannot be opened, the article is not published. A changed or missing statement sends the draft back to Gate 1. The same re-check is repeated right before publishing.

## 2026-10-13 — 1-week Search Console values recorded (user screenshots, 5)

**Source and timing.** Five Search Console screenshots sent by the user on 2026-10-13 (source label `사용자`), one day before the planned "on or after 2026-10-14" checkpoint. Search Console data in them runs only to 2026-10-10 ("last updated 9 hours ago"). Treated as the 1-week values; if the user wants a fresh read on or after 2026-10-14, add a second reading rather than overwriting. Recorded in `docs/pilot-evaluation.md` (table E "1주 점검" column, table B, checklist 5-1 and 5-3). Property: `statesideexplained.com` (domain property).

**Values.**
- Sitemaps: `sitemap_index.xml` submitted 2026-10-08, status **Success**, last read 2026-10-10, "sitemap index processed". Children: `category-sitemap.xml` 3 URLs (read 10-11), `page-sitemap.xml` 3 URLs (read 10-12), `post-sitemap.xml` 13 URLs (read 10-13). Discovered pages **19**, videos 0.
- Performance (web, window "3 months", data 2026-10-07 to 10-10): **clicks 0, impressions 496, CTR 0%, average position 16.2**. Queries: 103 rows; top `thanksgiving 2026` (227 impressions), then `cuando cae thanksgiving 2026` 8, `first day of winter 2026` 7, `fecha de thanksgiving 2026` 6, `start of winter 2026` 6; all with 0 clicks.
- Pages tab (impressions, clicks all 0): `thanksgiving-2026-date` 274, `first-day-of-winter-2026` 84, `usps-hold-mail-how-it-works` 53, `federal-holiday-weekend-observed` 36, `forever-stamp-how-it-works` 13, `usps-mail-forwarding-how-long` 12, `daylight-saving-time-end-2026-us` 9, `tsa-3-1-1-liquids-rule` 7, `real-id-to-fly-what-tsa-accepts` 5, home 3. The 10 rows sum to 496. Listed as 11 rows; the 11th was not visible.
- Home URL inspection (`https://statesideexplained.com/`): "URL is on Google", page indexing "page is indexed", HTTPS fine. Last-crawl date and canonical were collapsed on screen, not recorded. A "Request indexing" link is shown.

**Not received / not verified.**
- Pages (indexing) report: indexed / not indexed counts and reasons.
- URL inspection for the 12 posts (only home was sent), so table B's index, last-crawl and canonical columns stay empty.
- Content of the notification badge ("3") shown top right on every screen; Security and manual actions report.
- `power-bank-on-a-plane-tsa-faa`, `tsa-precheck-what-it-changes` and `usps-informed-delivery-how-it-works` are not among the 10 visible Pages rows; recorded as `—`, not as 0.
- The 7-day filter was not used (window was 3 months, which for a site live since 2026-10-07 covers the same days, assumed not verified).

**Open item.** `page-sitemap.xml` lists 3 URLs while the repo counts 2 pages (About, Privacy). The third URL is unknown from the screenshots. Post-sitemap 13 is consistent with "home + 12 posts" (Claude's inference, URL list not compared). Both matter for the homepage step (the home moves from the post sitemap to the page sitemap).

**Reading (Claude, not a decision).** One week is too early to judge: impressions exist, no clicks, nothing in these numbers says to change a post. Over half of the impressions (274 of 496) sit on the Thanksgiving date article, and the Spanish and "start of winter" queries show seasonal date queries are the first to be shown. The 12 posts' pass/fail thresholds for the 4-week evaluation are still undecided.

**Next (needs the user's approval each step).** Homepage restructure step 1: check the 12 posts for a sources list and a stated check date, then finalize the intro copy. No WordPress or theme change has been made.

## 2026-10-13 — Open item closed: public sitemap URLs checked against the 19 discovered

Claude opened the three child sitemaps in the built-in browser (logged out). `post-sitemap.xml` (13): `/` plus the 12 posts of table A. `page-sitemap.xml` (3): `/`, `/privacy-policy/`, `/about/` (last mod 2026-10-08 05:35 UTC). `category-sitemap.xml` (3): `/category/us-dates-seasons-holidays/`, `/category/airport-security-rules/`, `/category/postal-service-and-stamps/`. So the third page-sitemap URL is the home page, which is listed in both the post and the page sitemap: the 19 shown by Search Console counts it twice (18 unique URLs). Correction to the entry above: my inference that the home moves from the post sitemap to the page sitemap only after the redesign is not needed to explain the count; the home is already in both. Not a defect that was changed or fixed here; recorded for the homepage step (check what the sitemap lists after the static front page is set).

## 2026-10-13 — Search Console follow-up screenshots: second home indexing request; message list

**Source.** Two more user screenshots, 2026-10-13 (`사용자`).

**Home indexing request (second).** The home URL inspection screen shows the "Indexing requested" dialog ("URL added to the priority crawl queue; submitting repeatedly does not change the queue position or priority"). The dialog appears only right after the click, so the request is dated to the screenshot (2026-10-13), not stated on screen. This is the second request for the home page (first: 2026-10-08, user-reported). Claude had advised not pressing it; recorded as a fact, no harm assumed. Still no request for any of the 12 posts is known.

**Message list (3, all unread).**
1. 2026-10-12, type "page indexing": "New reason is preventing pages on statesideexplained.com from being indexed" (Korean title as shown in the screen). **The body, which names the reason and the affected URLs, has not been seen.** Until it is opened, nothing is known about which pages or why; this is not interpreted here.
2. 2026-10-11, general: Google Search traffic monitoring for the site.
3. 2026-10-08, general, sent directly: tips on raising the site's visibility.
No security-issue or manual-action message appears in the list (the Security and manual actions reports themselves were not seen).

**Needed next.** The body of message 1 and the Pages (indexing) report (indexed / not indexed counts and the reasons list). Table E rows for those stay `—`.

## 2026-10-13 — Pages (indexing) report and message bodies received; Claude's check of the 18 sitemap URLs

**Received (`사용자` screenshots, 2026-10-13).** Pages report "all known pages", last updated 2026-10-09: **indexed 12, not indexed 9 (4 reasons)**: "Page with redirect" 3 (source: website), "Excluded by 'noindex' tag" 2 (website), "Discovered – currently not indexed" 3 (Google systems), "Crawled – currently not indexed" 1 (Google systems); validation "not started" for all. Message 1 (2026-10-12) says the two new reasons are "Page with redirect" and "Excluded by 'noindex' tag"; no URLs are named. Message 2 (2026-10-11): Google Search impressions started being collected on 2026-10-09. Message 3 (2026-10-08): domain property verification and getting-started tips. No manual-action or security message in the list.

**Not known.** Which URLs are the 12 indexed and which are the 9 not indexed (the report's per-reason URL lists were not sent). So the 12 posts' individual index status is still unknown.

**Claude's check (read-only, built-in browser, same-origin fetch, logged out, 2026-10-13).** All 18 unique URLs of the three sitemaps (home, About, Privacy Policy, 3 category pages, 12 posts) return 200, declare `index, follow` in the robots meta and a self-referencing canonical, and send no `X-Robots-Tag` header. So none of the sitemap URLs is a "noindex" or canonical-pointing-elsewhere page. Pages that do carry `noindex` today: `/author/admin/` (200, "follow, noindex", the author archive whose link was removed from post bylines on 2026-10-08, JSON-LD still has some URLs) and `/author/stateside-explained/` (404, "follow, noindex"). These are candidates for the 2 noindex pages, **not confirmed** (the report's URL list is needed). The 3 "Page with redirect" URLs are most likely the non-canonical `www` or `http` variants that the 2026-10-08 Cloudflare 301 rule redirects, again **not confirmed**.

**Reading (Claude, not a decision).** Nothing seen so far points at a problem with the 12 posts: they are indexable, in the sitemap and canonical to themselves. "Discovered" and "Crawled – currently not indexed" (4 URLs) are common states for a one-week-old site and are recorded as observation, not as a defect. No change made to WordPress, the theme or Search Console; no indexing request for any post.

**Next.** The user clicks each of the four reasons in the Pages report and sends the URL lists (9 URLs in total); then the table E rows get filled and the 12 posts' individual status is settled.

## 2026-10-13 — Pages report: URLs behind each "not indexed" reason (user screenshots)

**Received (`사용자`, 2026-10-13; report last updated 2026-10-09; "first detected" 2026-10-10 for all four reasons).**
- **Page with redirect (3):** `http://www.statesideexplained.com/` (last crawl 10-10), `https://www.statesideexplained.com/` (10-10), `http://statesideexplained.com/` (10-08). These are the non-canonical address variants that the 2026-10-08 Cloudflare `www` → apex 301 rule and the http → https redirect send to `https://statesideexplained.com/`.
- **Excluded by 'noindex' tag (2):** `https://statesideexplained.com/author/admin/` (10-10) and `https://statesideexplained.com/?s={search_term_string}` (10-08). The first matches Claude's own check earlier today (`follow, noindex`). The second is the literal search-URL template (`{search_term_string}`), which comes from a site-search structured-data entry, not a real search; search result pages are normally `noindex`.
- **Discovered – currently not indexed (3):** `/power-bank-on-a-plane-tsa-faa/`, `/tsa-precheck-what-it-changes/`, `/usps-informed-delivery-how-it-works/`. Last crawl "not applicable": Google knows the URL (from the sitemap) but has not crawled it yet. These are exactly the three posts that had no impressions in the Pages tab of Performance.
- **Crawled – currently not indexed (1):** `https://statesideexplained.com/comments/feed/` (10-09), the WordPress comments feed.

**Reading (Claude, not a decision).** Nothing here is a defect to fix: three redirects, two intended noindex pages and a feed are expected states; none of the four is one of the 12 posts. Only the three "discovered" posts are a pilot observation: **3 of 12 posts not yet crawled as of the report date**. The other 9 posts appear in no "not indexed" list and all 9 had impressions in Performance, so they are very likely among the indexed 12 (inference: the indexed 12 URL list was not seen). Not changed: no indexing request, no WordPress or theme edit. Whether to request indexing for the 3 uncrawled posts is left open (a request would change the "natural discovery" observation); the user decides, at the latest at the 4-week evaluation. The next Pages report update (and a second reading on or after 2026-10-14) will show whether they get crawled.

**Closed from earlier today.** The message of 2026-10-12 ("new reasons: page with redirect and noindex") is explained by the first two items. The 2-noindex and 3-redirect candidates named in the previous entry are confirmed (noindex: author archive and the search-URL template; redirect: www and http variants).

## 2026-10-14 — 1-week checkpoint, second reading (user screenshots, 9)

**Received (`사용자`, 2026-10-14).** Performance (web, 7 days and 3 months give the same numbers): **clicks 0, impressions 710, CTR 0%, average position 15.1** (first reading, 2026-10-13: impressions 496, position 16.2). Chart covers 2026-10-07 to 2026-10-11, "last updated 10 hours ago". Top queries (7 days): `thanksgiving 2026` 249, `cuando es thanksgiving 2026` 32, `fecha de thanksgiving 2026` 11, `first day of winter 2026` 10, `winter kab se start hoga 2026` 8; all with 0 clicks. Pages (indexing) report unchanged and **still "last updated 2026-10-09"**: indexed 12, not indexed 9 (redirect 3, noindex 2, discovered 3, crawled 1), same URL lists as the first reading. Sitemaps: `sitemap_index.xml` success, last read 2026-10-10, 19 discovered (unchanged). The notification badge is gone (messages read).

**Not received.** The list of the 12 indexed URLs; per-post impressions for the 7-day view.

**Reading (Claude, not a decision).** The Pages report has not refreshed since the first reading, so there is no new information about the three posts Google has discovered but not crawled (`power-bank-on-a-plane-tsa-faa`, `tsa-precheck-what-it-changes`, `usps-informed-delivery-how-it-works`). Impressions rose (496 to 710, data one day longer), clicks stay 0. Nothing here asks for a change to a post, WordPress or Search Console. Recorded in `docs/pilot-evaluation.md` as a second reading below table B; the first reading was not overwritten. Suggested next look at the Pages report: when its "last updated" date moves past 2026-10-09 (not before about 2026-10-16), then decide whether to ask for indexing of the three posts.

## 2026-10-14 — Homepage restructure, step 1: do the 12 posts list sources and a check date? (read-only)

**Scope (user instruction, 2026-10-14).** Check only whether each of the 12 published posts really has a source list and a stated check date. No change to WordPress, the theme or any post. The user will finalize the intro copy from this result. Method: Claude, logged out, built-in browser, same-origin fetch of the 12 post pages on 2026-10-14; the "Sources" section and the date text were read from the page HTML. Not changed: anything on the site; not checked: whether each source statement still matches the live agency page (that is the separate DST re-check before 2026-11-01 and the 4-week evaluation).

**Result: 12 of 12 have both.** Each post has an H2 "Sources" with linked official pages (33 links in total: 2 to 4 per post) and a sentence in that section saying when the pages were checked ("All pages were checked on ..."). Each also says "as of [date]" in the body. All 33 links are on government or agency domains: nist.gov, transportation.gov, govinfo.gov, opm.gov, aa.usno.navy.mil, ncei.noaa.gov, tsa.gov, faa.gov and USPS sites (usps.com, faq., pe., store., facts.usps.com). Sources lines also note the page's own update date where the page shows one, and say "no update date" where it does not. The About page already says: facts come from official sources, each article lists its sources at the end and says when they were checked, independent site not affiliated with USPS, TSA, NIST, DOT or any government agency.

| Post | Sources | Check date stated |
|---|---|---|
| `daylight-saving-time-end-2026-us` | 4 | October 6, 2026 |
| `federal-holiday-weekend-observed` | 2 | October 7, 2026 |
| `first-day-of-winter-2026` | 2 | October 7, 2026 |
| `thanksgiving-2026-date` | 2 | October 7, 2026 |
| `power-bank-on-a-plane-tsa-faa` | 3 | October 7, 2026 |
| `real-id-to-fly-what-tsa-accepts` | 3 | October 7, 2026 |
| `tsa-3-1-1-liquids-rule` | 2 | October 7, 2026 |
| `tsa-precheck-what-it-changes` | 3 | October 7, 2026 |
| `forever-stamp-how-it-works` | 4 | October 7, 2026 |
| `usps-hold-mail-how-it-works` | 3 | October 7, 2026 |
| `usps-informed-delivery-how-it-works` | 2 | October 7, 2026 |
| `usps-mail-forwarding-how-long` | 3 | **October 8, 2026** |

**Consequence for the intro draft.** The sentence "Each article is based on official sources, lists them at the end, and says the date we checked them" is true for all 12 as written. Do not say "updated" or give one shared check date: the dates differ (Oct 6, 7 and 8).

**Finding for the user to decide (nothing changed).** Eleven posts carry the publish time 2026-10-07 20:11 (US Eastern) on the site and the daylight-saving post is dated Oct 6, 2026 (corrected 2026-10-14 after the draft home page showed real card dates); a date shown on a card displays Oct 7 for the eleven. `usps-mail-forwarding-how-long` says its sources were checked on October 8, 2026, a day after that displayed date. The likely cause is the date convention: the check was written in the user's local date (Oct 8 in Korea, still Oct 7 in US Eastern time). A reader could see a check date later than the publish date. Options for later, each needing the user's approval because it edits a published post: leave as is (low risk), or word that date with its time zone. Cards with a real publish date show Oct 7 for eleven posts and Oct 6 for the daylight-saving post. The daylight-saving post's check date (Oct 6) is earlier than the publish date, which is normal.

**Next step (needs approval).** Finalize the intro copy from this result, then step 2: build the static homepage as a draft.

**User decision (2026-10-14).** Leave the one-day difference between the check date (Oct 8) and the displayed publish date (Oct 7) as it is; the real check date is not changed to match the publish date, and no time zone is added now. Intro copy is final: headline "Everyday U.S. questions, explained simply"; "Stateside Explained answers practical questions about U.S. mail, airport rules, and the calendar. Each article is based on official sources, lists them at the end, and notes the date they were checked." / "This is an independent site and is not affiliated with USPS, TSA, or any government agency. For information that affects your travel or mail, check the relevant agency’s current page."

## 2026-10-14 — Homepage restructure, step 2: static home page built as a WordPress draft (not published)

**Scope (user instruction).** Build the static home page as a WordPress draft only. No switch to public, and the existing public home address, posts and theme stay unchanged until the draft is reviewed.

**What was done.** Claude, signed in to wp-admin in the built-in browser, created a new Page: ID 56, slug `home`, status `draft`, title "Everyday U.S. questions, explained simply". Built with core blocks only (saved with no invalid blocks): the two confirmed intro paragraphs; then, for each category, an H2 heading with a 2 px bottom border in `#2F5D62`, a Query Loop (4 posts, ordered by title A to Z, not inheriting the main query; category set by both the category id and the tax query), a grid post template (columns from a 17 rem minimum width, so one column on a phone), and a link `More in <category> →` to the category archive. Each card is a bordered group: category label, post title (link), a 28-word excerpt, the real post date (small, grey), and `Read →`. Categories: Airport security rules (id 5), Postal service and stamps (id 6), US dates, seasons and holidays (id 4).

**Not changed.** The home setting (Reading: still the latest-posts home), the theme and templates, the header, any of the 12 posts, the Rank Math title and description for the new page, the sitemap, LiteSpeed cache. Nothing was published.

**Checked in the preview (`https://statesideexplained.com/?page_id=56&preview=true`, login required).** Text read from the rendered page: headline, both intro paragraphs, three sections with four cards each (12 cards, each with label, title, excerpt, date, `Read →`) and three `More in … →` links. Dates are the real post dates: Oct 6, 2026 for the daylight-saving post and Oct 7, 2026 for the other eleven. A narrow (phone-like) pane showed a single column of bordered cards. A desktop-width view was not measured separately; the user should look at it in their own browser.

**Observations for the user (not decided).** (1) Each card repeats the category label already given by the section heading; it can be removed from the home cards. (2) Cards are ordered by title A to Z, so the order is stable but not by date. (3) Excerpts are cut at 28 words with an ellipsis. (4) With only four posts per section and 4 to 4 posts per category, `More in … →` leads to the archive that lists all of the category.

**Needs the user's approval next.** Review the draft; then, in this order and each with approval: set the Rank Math title and description for the page; publish; set it as the static front page (Settings, Reading) and check that `/home/` redirects or is canonical and that the sitemap moves it from the post sitemap to the page sitemap; purge the LiteSpeed cache; then header menu (step 3), post template date and `More in [category] →` (step 4), logged-out verification (step 5).

## 2026-10-14 — Homepage draft (Page 56) revised after the user's review notes; still a draft

**User decisions (2026-10-14).** (1) Remove the category label from the home cards; keep the real date on each card. (2) Card order: keep the native Query Loop ordering by publish date, newest first. The user chose this over a "date, then title" rule: posts on the same day have different real publish times, newest-first is natural, no PHP or manual ordering is added, and new posts appear automatically. (3) Meta title and description set on the draft first: title `Stateside Explained | Everyday U.S. Questions, Explained Simply`; description `Official-source explanations of U.S. airport rules, postal services, and dates, with sources and checked dates.` (4) Do not publish `/home/` on its own. The user previews on PC and phone and checks three things (3 categories with 4 cards each; excerpt length and card heights; card, date and `Read →` readable on a phone). When satisfied the user says "홈 공개 진행", and Claude then does, in one flow: publish the home page, set it as the static front page, purge the LiteSpeed cache, and check canonical and sitemap for `/` and `/home/`.

**Changes made to the draft (Page 56 only; nothing public changed).** Post-terms (category label) removed from the three card templates; the three Query Loops ordered by date, newest first; Rank Math title and description set (read back from the preview HTML: `<title>` and `meta description` equal the values above; robots `index, follow` because the page is a draft preview and is not yet public). Found while measuring at 1280 px: the grid layout of the card lists had not been saved (cards showed in one wide column). Fixed by setting the post template layout to grid with a 17 rem minimum column width.

**Measured on the draft preview (Claude, logged in, emulated viewports).** 1280 px wide: two columns, four cards per section, 12 cards, no horizontal scroll; card heights within a row are equal (rows 254, 273 and 296 px tall), so the grid looks even. 375 px wide: one column, 12 cards, each 315 px wide with a 30 px left margin, card heights 249 or 269 px, date and `Read →` at 14 px, no horizontal scroll (the only element past the viewport edge is the WordPress admin bar user name, which logged-out visitors do not see). Excerpts are about 28 words plus an ellipsis. Order in each section now: Airport security rules: PreCheck, REAL ID, Power bank, 3-1-1; Postal service and stamps: Forwarding, Hold, Informed Delivery, Forever Stamp; US dates, seasons and holidays: Federal holiday weekend, Thanksgiving, First day of winter, Daylight saving (Oct 6, last). Visual check by the user on a real PC and phone is still pending.

**Not changed.** Home setting (Reading), theme, header, the 12 posts, sitemap, LiteSpeed cache. Nothing published.

## 2026-10-14 — Homepage published as the static front page (steps 2 to 4 of the homepage plan done)

**Approval.** The user previewed the draft on PC and phone, found no problem and said to proceed ("홈 공개 진행"): publish, set as static home, purge LiteSpeed cache, check canonical and sitemap for `/` and `/home/`, in one flow.

**Done (Claude, built-in browser, signed in to wp-admin).** (1) Page 56 (`home`, title "Everyday U.S. questions, explained simply", Rank Math title and description as set on the draft) changed from draft to published. (2) Settings, Reading: "Your homepage displays" changed from latest posts to a static page, homepage = page 56; posts page left unset; "Discourage search engines" stays off. Settings saved. (3) LiteSpeed "Purge All - LSCache" run; the notice "Notified LiteSpeed Web Server to purge all LSCache entries" appeared. Not changed: theme, header, the 12 posts (latest modified still 2026-10-07T20:11:36), About, Privacy.

**Verification (logged out, cache-busted, same-origin fetch without credentials).** `/`: 200, title `Stateside Explained | Everyday U.S. Questions, Explained Simply`, description as set, canonical `https://statesideexplained.com/`, `og:url` the same, robots `index, follow, max-snippet:-1, max-video-preview:-1, max-image-preview:large`, H1 "Everyday U.S. questions, explained simply", 12 cards, three `More in … →` links to the three category archives, no admin bar. `/home/`: 200 after a redirect to `/` (WordPress redirect), same canonical, so there is no duplicate under `/home/`. Sitemaps: `sitemap_index.xml` lists post, page and category sitemaps; the page sitemap now contains `https://statesideexplained.com/` (with About and Privacy Policy) and not `/home/`; the post sitemap lists only the 12 posts; the category sitemap lists the 3 categories; `robots.txt` still points to `sitemap_index.xml`. About, Privacy, a category archive, one post, the feed and search all return 200.

**Observations (nothing changed).** (a) `/page/2/` still returns 200 and shows the same home page (WordPress serves the front page for a paged URL) with canonical `https://statesideexplained.com/`, so it is a canonical duplicate; it is not in the sitemap and no link points to it. (b) The home page's JSON-LD includes an `Article` type, the same as About and Privacy (Rank Math's default for pages). It is harmless; a plain WebPage type would be tidier and can be changed in Rank Math if the user wants. (c) The home URL moved from the post sitemap to the page sitemap; Search Console will pick this up on its next sitemap read. No indexing request was made; the user's plan is to re-check the Pages report around 2026-10-16.

**Next (each needs the user's approval).** Step 3: hand-built header menu with the three category links (About and Privacy stay footer-only). Step 4: real date and `More in [category] →` on the post template (and check whether previous/next blocks can be limited to the same category). Step 5: logged-out verification and decision-log entry.

## 2026-10-14 — Homepage plan step 3: header menu with the three categories

**Approval.** The user pushed `32a86d0` and approved step 3: the header gets a hand-built menu with only the three category links; About and Privacy stay footer-only; afterwards verify line breaks, menu button and link behavior on PC and phone.

**Done (Claude, built-in browser, signed in).** (1) A new Navigation (wp_navigation, ID 62, title "Header categories") with three taxonomy links in this order and with the full category names: Airport security rules, Postal service and stamps, US dates, seasons and holidays (category archive URLs). The older Navigation (ID 5) was not touched or used. (2) The Header template part (`twentytwentyfive//header`, customized copy) now contains a Navigation block that references ID 62, small font, `overlayMenu: mobile` (menu button under 600 px). (3) After the first check showed the links wrapping badly between 600 and about 900 px (third link alone on a second line, site title on two lines at 800 px), the header's outer group was changed from no-wrap to wrap, so on a medium-width screen the three links move together onto one second row under the site title. (4) LiteSpeed "Purge All - LSCache" was run after each header change. Not changed: the 12 posts (latest modified still 2026-10-07T20:11:36), the page content, Footer, About, Privacy, theme files.

**Verified, logged out (fetch without credentials).** On the home page, About, Privacy, one category archive, one post and a search page: the header contains the site title plus exactly the three category links (same URLs), no About or Privacy link in the header, and the footer still has About and Privacy Policy once each. The three category URLs return 200.

**Verified, rendered (built-in browser, emulated widths, logged in; admin bar adds 32 px at the top).** 1280 and 1024 px: title and the three links on one line, no menu button, no horizontal scroll. 800 and 600 px: title on one line (single line, about 180 px wide) and the three links on one row below it, no menu button, no horizontal scroll. 375 px (phone): title on one line, only the menu button (24 x 24 px, label "Open menu"). Opening it shows the three links one under another; the close button works and releases the page scroll lock; tapping "Postal service and stamps" opened `/category/postal-service-and-stamps/` with the menu closed and the button back. Not tested: a real touch device or Safari; the three overlay links are 20 px tall with about 30 px spacing and the menu button is 24 px, which is the theme's default and small for touch.

**Left for the user to decide (not changed).** Longer labels make the 600 to 900 px header two rows tall; shorter labels (for example "Airport rules", "Postal service", "Dates and holidays") would keep one row longer, but category names were kept as they are. The theme's overlay link size and button size can be made larger if wanted.

**Next (needs approval).** Step 4: real date and `More in [category] →` on the post template; check whether previous/next blocks can be limited to the same category (proposed separately). Step 5: logged-out verification of the whole round and decision-log entry.

## 2026-10-14 — Homepage plan step 4: investigation only (same-category previous/next, date, `More in [category] →`); nothing changed

**User instruction.** Keep the header as it is (a two-row header at 600 to 900 px is fine; the 20 px menu link height is to be checked once on a real phone: text height or real tap area). Pushed `278d26f`. For step 4, first only investigate whether previous/next links limited to the same category are possible, then decide the date display and `More in [category] →` blocks in one go. No template change now.

**Method.** Read-only: read the custom `single` template (`wp_template`, ID `twentytwentyfive//single`), checked the block definitions available in this site (WordPress 7.1.3, Twenty Twenty-Five), and fetched the 12 posts logged out. No save, no template edit, no cache purge.

**Findings.**
1. Same-category previous/next is possible with a core block and no code. `core/post-navigation-link` has a `taxonomy` attribute (the editor option "Filter by taxonomy"); setting it to `category` makes the link go only to the previous (older) or next (newer) post in the same category. The template already has the two navigation links (`previous` and `next`, title shown, arrow style) inside a "Post navigation" group; only the attribute would be added to both.
2. Today's links cross categories. Live previous/next on all 12 posts matched exactly the order by publish time over all posts (checked against the data: 12 of 12), so e.g. a Postal post links to an Airport post. That also validates the model used for the prediction below.
3. Predicted same-category links (previous = older, next = newer; by exact publish time): Airport security rules, newest to oldest: PreCheck, REAL ID, Power bank, 3-1-1. Postal service and stamps: Forwarding, Hold, Informed Delivery, Forever Stamp. US dates, seasons and holidays: Federal holiday weekend, Thanksgiving, First day of winter, Daylight saving time. Each category has four posts, so every post has at least one link; the newest and the oldest of each category would show one link only (no next, or no previous). The block renders nothing at the end of a chain. The REST block renderer returned nothing for this block, so the same-category result is predicted from the data and from WordPress's adjacent-post rule, not yet observed on the live pages; it would be verified on all 12 posts right after applying.
4. `More in [category] →` can be built dynamically with `core/post-terms` (term: category) using its prefix `More in ` and suffix ` →`. The link covers the category name only; the words and the arrow around it are plain text. Posts have exactly one category each, so no separator shows. A fully linked phrase would need a fixed link per category, which cannot follow the post's category by itself.
5. The template already shows, below the title and image, the line "Written by Stateside Explained in [category link]" (post-author-name plus post-terms). It has no date. Dates on a post page currently appear only in the "More posts" list at the bottom, not for the post itself. A `core/post-date` block (format as on the home cards: "October 7, 2026"; Oct 6 for the daylight-saving post) can be added next to that line, or under the title.
6. The "More posts" section at the bottom is the same site-wide list of the four newest posts on every post (checked on two posts), including the current post itself when it is among them (the forwarding post lists itself). It cannot follow the post's category without code; the Query block has an option to exclude the current post (`excludeCurrent`) if wanted.

**Options for the decision (nothing applied).** Date: (a) add the date to the existing "Written by ... in [category]" line, (b) show it under the title above the featured image. `More in [category] →`: (a) after the post content and above the previous/next navigation, (b) replace the "in [category]" part of the byline with it (not recommended: the byline would repeat the same words). Previous/next: add `taxonomy: category` to both blocks. Risk: the template change applies to all 12 posts at once; post bodies are not edited; rollback is restoring the template to the content read above (the current template content was read and is unchanged). After applying: purge LSCache and check logged out all 12 posts for date, `More in [category] →`, same-category links, then record and commit.

## 2026-10-14 — Homepage plan step 4 applied: post template (date, `More in [category] →`, same-category previous/next, "More posts" removed)

**Approval.** The user pushed `674bf69` and approved the options from the investigation: date at the end of the existing byline as `· October 7, 2026`; `More in [category] →` between the end of the post content and the previous/next links; category restriction on both previous/next links; the whole "More posts" block removed (not only the current post excluded). Post bodies not to be changed; purge the cache; check all 12 posts logged out (category-only movement, link counts at the first and last post, date, mobile layout).

**Done (Claude, site editor, one save of the customized `single` template, `twentytwentyfive//single`).** (1) Byline group "Written by [author] in [category]": added a "·" paragraph and a post-date block (default format, e.g. `October 7, 2026`). (2) New post-terms block (category, prefix `More in `, suffix ` →`, small, semibold, link color `#2F5D62`) placed after the tags group and before the "Post navigation" group. (3) `taxonomy: category` set on both post-navigation-link blocks (previous and next). (4) The "More posts" pattern group (heading plus the site-wide four-newest Query Loop) removed. The template was parsed and re-serialized (no invalid blocks); the previous template text (7,035 characters) was kept in the browser session before saving; the template history in the site editor can also restore it. LiteSpeed "Purge All - LSCache" was run after saving ("Notified LiteSpeed Web Server to purge all LSCache entries"). Not changed: the 12 posts (latest modified still 2026-10-07T20:11:36), header, footer, About, Privacy, theme files, home page.

**Verification, logged out, cache-busted, all 12 posts (fetch without credentials; results compared with values computed from the post data).** Previous/next: 12 of 12 equal the predicted same-category link (previous = older, next = newer by publish time). Link count: the newest and the oldest post of each category show one link, the other six posts show two (Postal: Forwarding has previous only, Forever Stamp has next only; Airport: PreCheck previous only, 3-1-1 next only; Dates: Federal holiday previous only, Daylight saving next only). Byline: all 12 read `Written by Stateside Explained in [category] · [date]` with the date equal to the post date (Oct 6, 2026 for daylight saving; Oct 7, 2026 for the other eleven). `More in [category] →` present on 12 of 12, linking to the post's category archive, placed after the post content and before "Post navigation". "More posts" text absent on 12 of 12. Post body text identical to the REST-rendered content on 12 of 12; one H1 and a canonical link on each. Header (3 category links) and footer (About, Privacy) unchanged on the home page, About, Privacy, a category archive and a search page.

**Verification, rendered (built-in browser, emulated widths).** 1280 px: byline on one line (`Written by Stateside Explained in Airport security rules · October 7, 2026`), `More in …` aligned with the text column, two navigation links left and right. 375 px: the byline wraps to two lines (the category name and date on the second line), 42 px tall on all 12 posts; the navigation links sit side by side (about 120 to 170 px each) or one full-width link (256 to 295 px), no overflow of the navigation or byline.

**Finding outside this change (nothing changed).** At 375 px, 11 of 12 posts scroll sideways by 15 to 128 px (scroll width 383 to 503 px). The cause is a long official URL printed as a link in the body's "Sources" list (for example the FAA battery page URL), which cannot wrap. Only `real-id-to-fly-what-tsa-accepts` fits. This is not caused by this round (the navigation and byline do not overflow) and was probably present before; the earlier note about a "measuring artifact" for one post should be read as this real overflow. A fix would be either a CSS rule letting long link text wrap in the post content (a theme/CSS change) or shortening the visible URL text in the bodies (a post edit); both need the user's approval.

**Next.** Step 5: a final logged-out round (home, header, posts, About, Privacy) and decision-log entry were largely covered by the checks above; remaining: the user's own look on a real phone, including the 20 px menu link height and the sideways scroll above. Search Console: re-check the Pages report around 2026-10-16.

## 2026-10-14 — Sideways scroll on phones fixed with CSS (post bodies not edited)

**Approval.** The user pushed `4a2a0b3` and decided: fix the sideways scroll with CSS, do not edit post bodies; apply only to body links and not to header, menu or footer: `.wp-block-post-content a { overflow-wrap: anywhere; }`; then purge the cache and re-check the 12 posts at 375 px logged out (no sideways scroll; short links, body text, tables, previous/next links, header menu not broken).

**Done (Claude, site editor).** The rule was added as Additional CSS in Styles (the site's user global styles record, ID 4, `styles.css`; the record had no other customizations before). No theme file, no post and no template was changed. LiteSpeed "Purge All - LSCache" was run ("Notified LiteSpeed Web Server to purge all LSCache entries").

**Verification (logged out: HTML fetched without credentials and rendered in a 375 px frame; 12 of 12 posts).** No sideways scroll on any post (document scroll width equals the visible width, no element past the right edge); previous/next navigation and header do not overflow; the 8 to 9 tables (1 or 2 on seven posts) are about 300 px wide inside the 330 px content area. Computed `overflow-wrap`: `anywhere` on body links, `normal` on header and previous/next links; the footer's `break-word` is the theme's own and unchanged. Effect isolated by switching the rule off in the same frame: short link text (non-URL links) has identical size on all 12 posts, header, footer and navigation heights identical on all 12; only the printed source URLs now wrap, and the body grows by 0 to 102 px in height (two posts, `real-id-to-fly-what-tsa-accepts` and `usps-informed-delivery-how-it-works`, unchanged). The home page, About, Privacy and the category archives were not part of this check; the rule targets `.wp-block-post-content` only, which they use for body text but with no printed URL.

**Not checked.** A real phone or Safari; the user's own look at the 20 px menu link height and tap area remains.

## 2026-10-20 — 1-week checkpoint, third reading (Claude read Search Console directly; read-only)

**How.** The built-in browser pane is signed in to Search Console; Claude opened the domain property `statesideexplained.com` (after the user's pane access was granted) and only read the Pages report, the four reason lists, the indexed list and Performance (7 days, by page). Nothing was clicked that changes data: no indexing request, no validation, no setting. Details recorded in `docs/pilot-evaluation.md` ("1주 점검 3차 값").

**Result.** Pages report last updated 2026-10-12 (it had been 10-09). Indexed 12 (home, 9 posts, About, Privacy), not indexed 15 (noindex 3, redirect 3, discovered 6, crawled 3). Indexed posts: 9 of 12; **not yet crawled: `power-bank-on-a-plane-tsa-faa`, `tsa-precheck-what-it-changes`, `usps-informed-delivery-how-it-works`** (discovered, last crawl "not applicable"). The 6 new not-indexed pages are not posts: the 3 category archives (discovered through the category sitemap), 2 feeds (`/feed/`, `/author/admin/feed/`) and `/author/admin/page/2/` (noindex). Performance 2026-10-11 to 10-17: clicks 1 (`tsa-3-1-1-liquids-rule`), impressions 2,340, average position 12.8; per page: Thanksgiving 843, first day of winter 527, 3-1-1 341, Hold Mail 203, weekend holidays 142, Forever stamp 117, forwarding 100, DST 40, REAL ID 14, home 13, Privacy 1; none for the three uncrawled posts and About.

**Reading (Claude, not a decision).** First click; all nine crawled posts have impressions; three posts still uncrawled about 13 days after publishing (they were discovered on 2026-10-10). Nothing says a post, WordPress or Search Console needs a change. The new not-indexed items are expected states (archives not yet crawled, feeds, a noindex author page).

**Open decision for the user (nothing done).** Whether to request indexing for the three uncrawled posts now or keep observing until the 4-week evaluation (on or after 2026-11-04). Requesting would change the "natural discovery" observation; waiting costs time on three posts that Google already knows from the sitemap. Option for later: inspect only those three URLs in the URL Inspection tool (read-only view) to see the sitemap/discovery state before deciding.

## 2026-10-20 — URL Inspection of the three uncrawled posts (read-only; no indexing request)

**User decision (2026-10-20).** Do not request indexing now. First inspect the three uncrawled posts with the URL Inspection tool only (known-to-Google status, last crawl date, indexability, discovery path); do not press "Request indexing". Keep observing natural crawling until the 4-week evaluation (on or after 2026-11-04). Reasons given: the pilot should keep showing whether natural crawling continues after the sitemap submission and the home restructure; nine posts are already indexed and shown, and the first click happened; "not yet crawled" as of 2026-10-12 is not an error signal. The user pushed `7abdb36`.

**Method.** Claude, in the signed-in built-in browser, typed each URL into the Search Console inspection box (domain property `statesideexplained.com`) and read the result page. The "Test live URL" and "Request indexing" buttons were not clicked. Nothing in Search Console or on the site was changed.

**Result (all three the same, 2026-10-20).** Status: "URL is not on Google" with the reason **"Discovered - currently not indexed"**. Discovery path: Sitemap `https://statesideexplained.com/sitemap_index.xml`; referring page `https://statesideexplained.com/` (the home page). Last crawl: not applicable; crawl agent, crawling allowed, page fetch, indexing allowed: not applicable (never crawled, so these are not assessed yet); user-declared canonical and Google-selected canonical: not applicable. So Google knows each URL from the sitemap and from the home page, has not crawled it, and shows no error, block or noindex for it. URLs: `/power-bank-on-a-plane-tsa-faa/`, `/tsa-precheck-what-it-changes/`, `/usps-informed-delivery-how-it-works/`.

**One odd reading.** The first inspection of `/usps-informed-delivery-how-it-works/` said "URL is unknown to Google" with no referring sitemap or page; running the same inspection again a minute later returned the same "Discovered - currently not indexed" result as the other two (sitemap and home page as referrers). Treated as a momentary inconsistency of the tool, not a change of state; the Pages report (2026-10-12) also lists this URL under "Discovered".

**Reading (Claude, not a decision).** The discovery path is clean: the home page now links to the posts and the sitemap lists them, so nothing on the site side blocks crawling. The state is a Google crawl-queue matter, not a site problem. No change to a post, WordPress or Search Console is suggested. Next look: the Pages report again after its "last updated" moves past 2026-10-12, and the 4-week evaluation (on or after 2026-11-04); the decision on requesting indexing is left to that point.

## 2026-10-29 — Daylight saving post: source re-check before the November 1 change (no change needed)

**Request (user, 2026-10-29).** Re-check the published post `daylight-saving-time-end-2026-us` against NIST, DOT Daylight Saving Time, DOT Uniform Time and 15 U.S.C. § 260a: the November 1, 2026 end at 2:00 a.m., the clock going back to 1:00 a.m., the non-observing places and the legal rule. If nothing changed, record the re-check date in the QA record and this log and make a local commit only; do not change the body, WordPress or SEO settings.

**Done.** Claude opened each page in the built-in browser (this time as a real page load, not through a summarizing tool) and compared it with the QA record (`editorial/qa/daylight-saving-time-end-2026-us.md`, new section "Re-check before 2026-11-01"). Result: **no source changed.** NIST (updated Feb 9, 2026) still says DST ends November 1, 2026 at 2 a.m. local time and clocks go back to 1 a.m.; its non-observing list is unchanged (no Northern Mariana Islands; Navajo Indian Reservation observes DST). DOT Daylight Saving Time (Sept 3, 2025) still lists Hawaii, American Samoa, Guam, Northern Mariana Islands, Puerto Rico, the Virgin Islands and most of Arizona. DOT Uniform Time (July 15, 2026): the exemption, no-permanent-DST and no-power-to-change sentences are unchanged. 15 U.S.C. § 260a (govinfo 2024 edition): same rule, latest amendment still Aug. 8, 2005. All page dates are the same as on 2026-10-06 and 2026-10-07. The article body, front matter, WordPress post and SEO settings were not touched. Limit: the statute link in the article opens a PDF whose text the browser could not extract, so the HTML copy of the same section on govinfo was read.

**Status.** The follow-up item "before 2026-11-01, re-open S1 to S4" is closed. Remaining: nothing for this post unless a source changes before November 1; the 4-week evaluation (on or after 2026-11-04) is next.

## 2026-10-29 — Article 13 (alcohol on a plane): five official sources re-checked before the `ready` approval request; no change; post-pilot cadence noted

**Request (user, 2026-10-29).** Re-check the five official sources of `alcohol-on-a-plane-tsa-faa` against the draft (two TSA pages, the FAA web page, eCFR, the FAA PDF chart), open the FAA PDF directly, report "not verified" if it cannot be opened, and if nothing is off, record the re-check and ask for approval to move to `ready`. No WordPress upload and no publishing yet.

**Done.** Claude opened each page in the built-in browser and compared it with the draft and the source notes. **No source changed, no statement of the draft is contradicted.** TSA pages: still Last Updated Feb 20, 2025, same text (carry-on 3.4 oz/100 ml; checked yes; over 24% up to 70%: 5 liters per passenger, unopened retail packaging; 24% or less not subject to limitations in checked bags; over 70%: no in carry-on and checked). FAA web page: still last updated April 13, 2026, 5 L per packaging and 5 L total per passenger, no drinking on board unless served by the air carrier. eCFR 49 CFR 175.10(a)(4): word for word the same; only the page's "up to date as of" date moved (10/08/2026 to 10/27/2026). **FAA PDF: opened directly in the browser (9 pages), "Updated: 11/14/25", alcohol rows read on page 3 and unchanged.** This closes the caveat that had travelled with C17 since 2026-10-13. One observation only: the PDF file's HTTP "Last-Modified" header says 2026-05-14 while its printed date and the alcohol rows are unchanged. Details: `editorial/qa/alcohol-on-a-plane-tsa-faa.md` (new section), `research/sources/alcohol-on-a-plane-tsa-faa.md`, `docs/content-backlog.md` row 16. The article text, WordPress and SEO settings were not touched.

**Status.** Article 13 stays `draft`. Claude asked the user for approval to move it to `ready`; not moved until the user says so. The same five-page re-check (FAA PDF opened directly) is required again right before publishing.

**Post-pilot cadence (user, 2026-10-29).** After the pilot, new posts continue at a target of 1 to 2 per week, recorded separately from the 12 pilot posts, and adjusted to the real workload. Article 13 is a post-pilot post (not counted in the 12). Search volume and any crawl effect of a faster cadence are not stated as facts; they are not measured.

## 2026-10-29 — Article 13 (alcohol on a plane): approved to move to ready

The user approved moving `alcohol-on-a-plane-tsa-faa` to `content/ready/` on 2026-10-29, after the five-page source re-check (no source changed; FAA PDF opened directly) recorded above, and pushed `9d09a1a`. Claude moved the file from `content/drafts/` to `content/ready/` and set `status: ready`; the article text, front matter fields other than status, image and alt text are unchanged. Backlog row 16 stage `ready` (post-pilot, not counted among the 12) and the stage table (deferred or reserve: ready 1, draft 0) updated; QA record updated. Not on WordPress and not published: the WordPress upload and publishing are separate steps the user will request. Before publishing the five-page re-check is mandatory again, with the FAA PDF opened directly; if it cannot be opened, the article is not published.

## 2026-10-29 — Article 13 (alcohol on a plane): WordPress draft created (not published)

At the user's request Claude created the WordPress draft for `alcohol-on-a-plane-tsa-faa` from the `content/ready/` file as pushed (`0b87786`): post id 69, media id 68, slug, title, category Airport security rules, diagram with alt text (402 characters), Rank Math meta description and focus keyword, comments and pings closed. The pane's wp-admin session had expired at first; the user signed in again (Claude does not enter passwords). Checks: 21 valid blocks; body text equals the repository text (3,662 letters and digits) and the link URLs match; the image equals the repository PNG by hash (1200 x 2286, not scaled); Rank Math values re-read after a fresh load of the edit screen; one post with the slug; 404 when logged out. Mobile preview at 375 px: no horizontal scroll, table and diagram fit and read; byline, `More in Airport security rules →` and no comment form as on the other posts. Details in `editorial/qa/alcohol-on-a-plane-tsa-faa.md`. Not published. Preview: https://statesideexplained.com/?p=69 . Before Publish the five-page re-check is mandatory (FAA PDF opened directly). Counts: published 12 (pilot, unchanged); post-pilot ready 1 (with a WordPress draft).

## 2026-10-29 — Article 13 (alcohol on a plane): pre-publish re-check of the five sources (no change)

At the user's request, right before publishing, Claude re-read the five official pages as real page loads in the built-in browser: TSA "Alcoholic beverages" (11 of 11 statements present, Last Updated February 20, 2025), TSA "over 140 proof" (7 of 7, same date), FAA PackSafe web page (9 of 9, last updated April 13, 2026; the "Over 140 Proof" section still states no rule), eCFR 49 CFR 175.10(a)(4)(i) and (ii) (3 of 3 word for word; up to date as of 10/27/2026), and the FAA printable chart PDF, **opened directly** (page 3, "Updated: 11/14/25"; under 140 proof: unopened retail packagings, 5 L per packaging and 5 L total per passenger; over 140 proof: not allowed in carry-on or checked bags; file size and Last-Modified unchanged since the check earlier the same day). **No source changed.** WordPress draft 69 re-read: still draft, text equal to the repository. Nothing was changed or published. Record: `editorial/qa/alcohol-on-a-plane-tsa-faa.md`. Publishing is the user's step; if it happens on a later day the re-check is repeated.

## 2026-10-29 — Article 13 (alcohol on a plane): published; live QA passed; moved to `content/published/`

The user published `alcohol-on-a-plane-tsa-faa` (post 69) on 2026-10-29 at 02:01:16 site time and pushed `3fb0082` (the pre-publish re-check record). The first message said it was published but left the URL as a placeholder; Claude checked and found the post still `draft` and the URL returning 404, said so, and ran the live QA after the user confirmed publishing; the post was then `publish` and returned 200. Live URL: https://statesideexplained.com/alcohol-on-a-plane-tsa-faa/ .

**Live QA (Claude, logged-out request plus a 375 px phone render): passed.** Title, H1, body text (3,662 letters and digits), table (5 x 2), diagram (repository PNG, 402-character alt), six links (internal link once; five official pages), meta description, canonical, robots `index, follow`, category Airport security rules, structured data, comments and pings closed (no form, no pingback tag or header), post and category sitemaps, feed, home card, category archive: all as expected; no horizontal scroll on a 375 px screen. Details in `editorial/qa/alcohol-on-a-plane-tsa-faa.md`. Nothing was changed on WordPress.

**Records.** File moved to `content/published/` with `status: published`, `published_date: 2026-10-29`, `live_url`; backlog row 16 stage `published` (post-pilot, not counted); stage table: pilot 12 published, 1 post-pilot published. `docs/pilot-evaluation.md`: new rule and table F keep the 13th post apart from the 12 pilot posts; the 12 pilot values are not mixed with it.

**Observation (not changed, for the user).** The home page shows four cards per category. With the fifth airport-security post, `tsa-3-1-1-liquids-rule` (the oldest in that category, and the first post to get a click) is no longer among the home cards; it stays in the category archive, sitemap, feed and body links of two articles. Options are the user's to decide (nothing applied): (a) leave it, since the structure was frozen unless the real-phone check finds a problem; (b) raise the card count for that section; (c) record it and read the 4-week values with this fact in mind (recorded in `docs/pilot-evaluation.md`). Claude does not claim an effect on search or crawling in either direction.

**Counts.** Live: 13 (12 pilot + 1 post-pilot). Pilot 12 unchanged. Post-pilot cadence stays: target 1 to 2 new posts per week, adjusted to the real workload.

## 2026-10-29 — Home cards: keep the newest 4 per category (user decision)

After reading the live QA and the publish record for article 13 (and pushing `6e412d4`), the user decided to keep the home page as it is: the newest 4 cards per category. The fact that `tsa-3-1-1-liquids-rule` is no longer among the home cards stays as recorded in `docs/pilot-evaluation.md` (table F note) and is to be looked at together with the 4-week evaluation (on or after 2026-11-04). Nothing changed on the site. Any new post in a category with four or more posts will push the oldest card off the home page the same way; this is expected under the chosen setting.

## 2026-10-29 — Cadence back to 3 posts per week; candidate research (nothing drafted)

**User decision.** From now on the English blog targets 3 new posts per week, spread across the week rather than published at once. The 4-week evaluation (on or after 2026-11-04) and new-article work run in parallel. This replaces the earlier post-pilot target of 1 to 2 per week. Post-pilot posts stay recorded separately from the 12 pilot posts.

**Research done (no brief, draft or WordPress work started).** Three candidates were compared on official sources, overlap with live posts, reader question, difficulty and whether demand can be checked: A lighters (`lighters-on-a-plane-tsa`, row 17), B Veterans Day post office (`usps-veterans-day-post-office`, new row 18), C TSA medications (`tsa-medications-liquids-carry-on`, new row 19). Full record: `docs/next-candidates-2026-10-29.md`. Search demand cannot be confirmed with the tools available; Google Trends gives relative, coarse values only and these are labelled estimates. Recommended order: B first (deadline), then A (hardest, start sources early), then C (swap-in).

**Thanksgiving notices.** No 2026 USPS or TSA Thanksgiving release found as of 2026-10-29. Rows 8 and 12 stay deferred; the 2026 notices must be re-read before publishing (earlier user rule unchanged). USPS notice expected around mid-November (estimate); the TSA release probably comes too late for indexing before the holiday (estimate).

**Waiting for the user** to choose the candidate(s) before any brief or draft starts.

## 2026-10-29 — Candidate selection: B first, A in parallel, C checked only

**User decision.** Start with B (Veterans Day post office), and run A (lighters) sources and brief in parallel. For B, re-check whether USPS published its 2026 notice; if not, report what can be written from confirmed official evidence, do not use last year's notice as this year's operating information, and hold publication if the 2026 evidence is not enough. For A, define first what one article can say accurately. For C (medications), check against the existing health exclusion and do not write it now. The 3-posts-per-week target stays, with no shortcut on source checks or review.

**Done (no draft, no WordPress work).**
- B: no 2026 USPS Veterans Day notice as of 2026-10-29 (newsroom, RSS, Sept. 22 and Oct. 22 holiday releases, "Holidays & events" page, ELM 518.1). The standing page lists Nov. 11, 2026 but does not say open or closed. Brief written, on hold: `research/briefs/usps-veterans-day-post-office.md`.
- A: scope set (disposable and Zippo-type, arc/electronic and lithium-battery, torch, unabsorbed-liquid lighters, lighter fluid in one row; DOT special-permit mechanics out). FAA FAQ PDF (2013) opened directly. Source conflicts recorded (checked bags for disposable/Zippo-type: TSA vs FAA; number of lighters; torch lighters: 2013 FAQ vs current FAA and TSA pages). DOT-SP 14415 shows an expiration date of Feb. 28, 2017. Brief and nine source notes written; all quotes tested against source text: `research/briefs/lighters-on-a-plane-tsa.md`, `research/sources/lighters-on-a-plane-tsa.md`.
- C: conflicts with `docs/blog-c-site-structure.md` (common criterion 3 and the lane-2 exclusion "medication rules (close to a health topic)"); outside current criteria; not drafted. Details in `docs/next-candidates-2026-10-29.md`.

**Waiting for the user.** Approval of the A scope and the 2013 FAQ handling; the B hold or fold-in decision; whether to research non-health replacement candidates for the third weekly slot.

## 2026-10-29 — Lighters draft and Gate 1; B monitoring; third-slot research

**User decision.** Proceed with A (lighters) to a draft and Gate 1; record the older 2013 FAA FAQ in source notes and QA first and propose before it enters the body; do not state a current special permit that cannot be confirmed; report the checked-bag and cabin rules that cannot be set out clearly. For B, check the USPS notice until about Nov. 5 and hold publication if 2026 operations are not confirmed. C is out this week; research 2 or 3 non-health third candidates; mark unverified demand as not measured. Commit locally; no WordPress upload or publishing.

**Done.**
- A: draft `content/drafts/lighters-on-a-plane-tsa.md`, diagram (`assets/raw/lighters-on-a-plane-tsa.svg`, `assets/optimized/lighters-on-a-plane-tsa.png`, 1200 x 2319), Gate 1 in `editorial/qa/lighters-on-a-plane-tsa.md`: 32 of 32 claims pass as attributed statements; sources re-read after drafting. Four open points reported (checked bags for disposable and Zippo-type lighters, the DOT exemption, number of lighters, torch label). The 2013 FAQ and DOT-SP 14415 are not used in the body; a proposal for one dated sentence is in the QA and awaits the user. Gate 2 not run; not in `content/ready/`; no WordPress upload.
- B: re-checked again on 2026-10-29 (about 08:00 UTC): still no 2026 USPS Veterans Day notice (RSS newest item Oct. 22). Three in-session reminders set for 2026-10-30, 2026-11-03 and 2026-11-05 (each at 02:00 UTC) to re-check; the final one reports and recommends holding or folding into row 12 if there is still no 2026 notice. Nothing drafted.
- Third slot: three non-health candidates researched (rows 20 to 22 of the backlog; table in `docs/next-candidates-2026-10-29.md`): USPS Certified Mail, federal holidays 2027, TSA laptops at the checkpoint. Demand: Trends relative only; volume not measured.

**Waiting for the user.** Gate 2 request after the push; decision on the 2013 FAQ sentence; choice of third candidate; whether to start B drafting if a 2026 notice appears.

## 2026-10-29 — Gate 2 FIX on lighters; Certified Mail brief; 2027 holidays as a late-November candidate

**User decisions.** (1) Start the Certified Mail brief and source notes: legal effect is not covered; no fee until the official USPS price list is confirmed. (2) Record the 2027 federal holidays article as a late-November preparation candidate. (3) Do not add the 2013 FAQ sentence to the lighters article; send the current version to ChatGPT Gate 2. (4) Lighters Gate 2 result: **FIX**, base `50ce2d8`, five items.

**Done (local commits only; no ready move, no WordPress).**
- Lighters FIX applied (commit `318b5b2`): lead and table now show the FAA carry-on guidance first and split the disposable and Zippo-type row into carry-on and checked bags; TSA's checked-bag answer is shown as conditional (without fuel allowed; with fuel prohibited unless the DOT exemption applies, up to two in a DOT approved case) against the FAA chart's "Not allowed in Checked Bags"; the limit that no current DOT permit was confirmed is kept in the lead, table, body, diagram and alt, and the article does not say the exemption applies today; the TSA officer wording is scoped to the checkpoint; the 2013 FAQ stays in the source note and QA only. Diagram redrawn (1200 x 2901) and alt rewritten (497 characters). All eight official pages (five TSA pages, FAA page, FAA chart PDF opened directly, eCFR) were re-read after the edits; 18 of 18 revised statements pass as attributed statements (QA, "Gate 2 FIX round"). Open limits P1 to P4 remain and are stated in the article.
- Certified Mail: brief `research/briefs/usps-certified-mail-how-it-works.md` and source notes `research/sources/usps-certified-mail-how-it-works.md`. Four USPS pages read (FAQ dated May 12, 2026; DMM 503 section 3.0; USPS.com extra-services page; Notice 123 effective October 4, 2026). The Certified Mail fee is recorded in the source note for reference and not used in any draft; Claude recommends the first draft states no number.
- 2027 federal holidays: backlog row 21 marked as a late-November preparation candidate; nothing started.

**Waiting for the user.** Push of `318b5b2` (and the earlier unpushed commits), then ChatGPT Gate 2 round 2 for lighters by SHA; approval of the Certified Mail scope, the fee option (no number recommended) and the go-ahead to draft; B re-checks continue (reminders 2026-10-30, 2026-11-03, 2026-11-05).

## 2026-10-29 — Certified Mail draft and Gate 1

**User decision.** Draft Certified Mail in the proposed scope: no legal effect, no Registered Mail comparison; no fee number in the body (point to the official price list); state the 15-day hold on the basis of the USPS FAQ with its conditions made clear; do not guess what "(PM only)" means. Then source check, Gate 1, records and a local commit; no WordPress upload or publishing. (The user's push `50ce2d8..41ab09f` is also on record.)

**Done (local commit only; no ready move, no WordPress).**
- Draft `content/drafts/usps-certified-mail-how-it-works.md` (about 1,265 words) and diagram (`assets/raw/usps-certified-mail-how-it-works.svg`, `assets/optimized/usps-certified-mail-how-it-works.png`, 1200 x 2697, no price, no logo).
- Gate 1 in `editorial/qa/usps-certified-mail-how-it-works.md`: the four USPS pages were opened again after drafting and tested by script (FAQ 36 of 36, DMM 503 16 of 16, USPS.com 2 of 2, Notice 123 4 of 4); 34 of 34 claims pass as attributed statements or stated limits.
- The 15-day hold is written as the FAQ states it, followed by what the FAQ does not say (what starts the 15 days, a notice, any change of the period); the DMM Certified Mail section does not repeat it; DMM 508 was not read. "(PM only)" is left out of the body and recorded as P3.
- Open points reported: 15-day hold trigger (P1), Priority Mail Express named in one FAQ sentence but not in its eligibility list (P2), "(PM only)" (P3), signature wording across pages (P4), the "Prove you sent it." quote (P5), no revision dates on two pages (P6).

**Waiting for the user.** Push, then ChatGPT Gate 2 by SHA for lighters round 2 and for Certified Mail; whether to read DMM 508 to settle P1 (optional); B re-checks continue (2026-10-30, 2026-11-03, 2026-11-05).

## 2026-10-29 — Gate 2 FIX on lighters (round 2) and Certified Mail (round 1)

**Gate 2 result (base `aa72f32`).** Both articles: FIX. Lighters: the SVG and PNG on GitHub were still the previous diagram; show the conditional checked-bag answer, the FAA chart difference and the unconfirmed DOT permit in the diagram; limit the TSA officer wording to the security checkpoint; open the files as committed and compare with the alt. Certified Mail: check DMM 508.1.1.7 against the FAQ for the 15-day conditions and the sender's shorter period; do not estimate the start of the count; revise body, diagram and alt together and separate ordinary signature from Restricted Delivery scope; fix the "prices must change" sentence; remove "Prove you sent it." and explain the mailing receipt plainly.

**Finding (Claude's error).** The lighters diagram files committed in `318b5b2` and `aa72f32` were the first diagram: the file transfer reused an earlier file under the same name, and the round 1 image check looked at the build folder rather than the repository file. Corrected by writing the files under new transfer names and reading them back from the repository (size, dimensions, pixel comparison with the render, SVG text). The files also carry a provenance manifest added by the transfer (PNG `caBX` chunk, SVG `<metadata>`); the earlier QA statement "no embedded metadata" is withdrawn. New rule: read every image back from the repository file before committing.

**Done (local commit only; no ready move, no WordPress).**
- Lighters: diagram footer "At the security checkpoint, the TSA officer decides whether an item is allowed through."; alt rewritten (521 characters) and matched to the diagram; QA section "Gate 2 FIX round 2".
- Certified Mail: DMM 508 read (1.1.1 to 1.1.8, source S5). 15-day period from the FAQ and DMM 508.1.1.7 together; the start of the count is stated by neither page and is not estimated; the sender may specify fewer days on the piece (how is not stated). Signature (508.1.1.7) and Restricted Delivery (508.1.1.8) scopes separated. "Prove you sent it." removed; fee sentence now "a newer version of the list may show different fees". New diagram (1200 x 3207) and alt (504 characters). 42 of 42 claims pass against the five USPS pages, re-read after the edits.

**Waiting for the user.** Push, then Gate 2 round 3 (lighters) and round 2 (Certified Mail) by SHA. B re-checks continue (2026-10-30, 2026-11-03, 2026-11-05).
