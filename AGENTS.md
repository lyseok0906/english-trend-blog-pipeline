# AGENTS.md

Instructions for AI agents working in this repository. Read this together with
`docs/operating-model.md` and `config/editorial-policy.md` before making any change.

## What this repository is

The editorial repository for an English-language trends blog. Scope is that blog only.

## Hard rules

1. **`main` on GitHub is the single source of truth.** Do not treat a chat transcript as
   project state. If your understanding disagrees with the files here, the files are
   correct.
2. **Do not push.** Commit locally and stop. The user runs `git push`.
3. **Do not publish.** No WordPress upload, no scheduling, no public posting — not even a
   draft upload — without explicit human approval for that specific article.
4. **Stay in scope.** This repository is not for the Excel blog
   (`excel-data-cleanup-pipeline`) or the Korean economic blog
   (`economic-blog-pipeline`). Do not import their topics, content, or policies.
5. **Follow the lifecycle.** topic brief → evidence/source review → draft → factual QA →
   English + SEO QA → ready → publish approval. No stage is skipped or reordered.
6. **Never invent a fact, figure, quote, date, or source.** Every factual claim must
   trace to a source recorded in `research/sources/<slug>.md`. If a claim cannot be
   sourced, remove the claim — do not soften it.
7. **Do not commit secrets.** No credentials, tokens, API keys, or `.env` files.

## Role boundaries

- **Cowork (Claude)** — the only writer. Research, briefs, drafts, QA records, `docs/`
  and `config/` updates, local commits.
- **ChatGPT** — reviewer only. Editorial direction, SEO/search-intent review, US-English
  QA. Does not write or commit files here.
- **User** — reviews, pushes, approves publication.

## Where things go

| Content | Path |
|---|---|
| Topic brief | `research/briefs/<slug>.md` |
| Source notes | `research/sources/<slug>.md` |
| Draft | `content/drafts/<slug>.md` |
| QA record | `editorial/qa/<slug>.md` |
| Cleared, awaiting approval | `content/ready/<slug>.md` |
| Live | `content/published/<slug>.md` |
| Images as captured | `assets/raw/` |
| Images used in the post | `assets/optimized/` |

Use one lowercase, hyphenated slug per article and reuse it across every path above.

## Before you finish a task

- State plainly what you changed and what you did not.
- If you were blocked, say what blocked you rather than working around a rule.
- Record any decision that changes how the blog is run in `docs/decision-log.md`.
- Leave the working tree in a state the user can review: committed, not pushed.

## Things that are deliberately not in this project

- Automated publishing or auto-login to any platform.
- Generating articles in bulk to hit a page count.
- Two assistants writing to this repository at the same time.
