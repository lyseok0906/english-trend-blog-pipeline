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
