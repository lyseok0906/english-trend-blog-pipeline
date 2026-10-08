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
