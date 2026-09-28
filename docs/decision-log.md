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
