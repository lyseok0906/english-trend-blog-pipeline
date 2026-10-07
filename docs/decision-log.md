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

