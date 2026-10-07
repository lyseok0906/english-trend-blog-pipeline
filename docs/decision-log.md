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
