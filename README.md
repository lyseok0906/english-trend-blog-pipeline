# english-trend-blog-pipeline

Editorial repository for an **English-language trends blog**. This repository holds the
operating model, topic backlog, research briefs, article drafts, and QA records for that
blog and nothing else.

## Scope

- In scope: English-language trend content — topic selection, research, drafting, QA,
  publish preparation.
- Out of scope: the Excel data-cleanup blog (`excel-data-cleanup-pipeline`) and the
  Korean economic/markets blog (`economic-blog-pipeline`). These are separate projects
  with separate repositories. Do not mix their topics, drafts, assets, or decisions in
  here.

## Source of truth

`main` on GitHub is the single source of truth. Anything not committed and pushed to
`main` is a work in progress, not a decision.

## Who does what

| Role | Responsibility |
|---|---|
| **Cowork (Claude)** | Research, drafting, QA document updates, local commits |
| **ChatGPT** | Editorial direction, SEO / search-intent review, US-English QA. Does not overwrite repository files |
| **User** | Reviews changes, performs the final `git push`, approves public release |

Public release — WordPress publishing or any other public posting — requires explicit
human approval. No exceptions, and no automated publishing.

## Article lifecycle

```
topic brief → evidence / source review → draft → factual QA → English + SEO QA → ready → publish approval
```

A file's location in the repository tells you which stage it is in:

| Path | Meaning |
|---|---|
| `research/briefs/` | Topic briefs: what the article is, who searches for it, why it is worth writing |
| `research/sources/` | Captured evidence — source notes, data extracts, links with retrieval dates |
| `content/drafts/` | Drafts that have not cleared QA |
| `content/ready/` | Drafts that cleared both QA gates and await human publish approval |
| `content/published/` | Articles that are live, with their published URL recorded |
| `editorial/qa/` | QA records: one per article, factual + English/SEO results |
| `assets/raw/` | Original screenshots and images as captured |
| `assets/optimized/` | Cropped / compressed images actually used in posts |

## Documents

| File | Purpose |
|---|---|
| `docs/operating-model.md` | The operating rules — roles, source of truth, lifecycle, approval gates |
| `docs/blog-c-site-structure.md` | Active standard for the initial 4-week pilot — site promise, lanes, selection and exclusion criteria, official-source re-check rule, cadence. Not a permanent niche confirmation |
| `docs/content-backlog.md` | Topic candidates and their current stage |
| `docs/decision-log.md` | Dated record of decisions and why they were made |
| `config/editorial-policy.md` | Writing, sourcing, and SEO standards every article must meet |
| `AGENTS.md` | Instructions for AI agents working in this repository |

## Working in this repository

1. Read `docs/operating-model.md` and `config/editorial-policy.md` first.
2. Add or pick a topic in `docs/content-backlog.md`.
3. Write the brief, gather evidence, draft, then record QA — in that order.
4. Commit locally with a clear message. Do not push; the user pushes.
5. Record anything that changes how the blog is run in `docs/decision-log.md`.
