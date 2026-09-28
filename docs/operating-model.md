# Operating Model

This document defines how work happens in this repository. It applies to every
contributor — human or AI. When any other document conflicts with this one, this one
wins until it is amended here and the amendment is recorded in `docs/decision-log.md`.

## 1. GitHub `main` is the single source of truth

The authoritative state of this project is the latest commit on `main` at
`https://github.com/lyseok0906/english-trend-blog-pipeline`.

- Conclusions that live only in a chat transcript are not project state.
- A local commit is not project state until it is pushed to `main`.
- When a chat and the repository disagree, the repository is correct.

## 2. Cowork (Claude) researches, drafts, updates QA documents, and commits locally

Cowork is the only actor that writes files in this repository. Its remit:

- topic research and search-intent investigation
- writing briefs, drafts, and QA records
- updating `docs/` and `config/`
- running `git add` and `git commit` locally

Cowork does not push, and does not publish.

## 3. ChatGPT provides editorial direction and review, and does not overwrite files

ChatGPT's remit:

- topic direction and prioritisation
- search-intent and SEO review
- US-English quality review

ChatGPT reads the repository and returns feedback. It does not write, edit, or commit
files here. This is a deliberate operating rule, not a tooling limitation: a single
writer avoids version conflicts between two assistants.

Feedback from ChatGPT reaches the repository by being handed to Cowork, which applies it
and records the round in the article's QA file.

## 4. The user reviews changes and performs the final `git push`

After Cowork commits, the user reviews the diff and runs `git push`. Nothing reaches
`main` without the user doing this.

## 5. No public release without explicit human approval

WordPress publishing, scheduling a post, or any other public posting requires the user's
explicit approval for that specific article. Blanket or prior approval of the project
does not count as approval of an individual article. Automated publishing is not part of
this project and will not be added.

## 6. Every article follows one fixed sequence

```
topic brief
   ↓
evidence / source review
   ↓
draft
   ↓
factual QA
   ↓
English + SEO QA
   ↓
ready
   ↓
publish approval
```

Each stage has a required artifact, and a stage is not complete until its artifact
exists in the repository:

| Stage | Required artifact | Location |
|---|---|---|
| Topic brief | Brief covering topic, search intent, audience, angle, why now | `research/briefs/<slug>.md` |
| Evidence / source review | Source notes with links and retrieval dates | `research/sources/<slug>.md` |
| Draft | Article draft | `content/drafts/<slug>.md` |
| Factual QA | Claim-by-claim check against the recorded sources | `editorial/qa/<slug>.md` |
| English + SEO QA | US-English and search-intent check, in the same QA file | `editorial/qa/<slug>.md` |
| Ready | Draft moved, front matter complete | `content/ready/<slug>.md` |
| Publish approval | Approval recorded, then article moved with its live URL | `content/published/<slug>.md` |

Stages are not skipped, reordered, or merged. A failed QA sends the article back to
`content/drafts/`; it does not proceed with a noted exception.

## 7. The Excel blog and the economic blog stay completely separate

Three blogs exist and each has its own repository:

| Blog | Repository | Language / audience |
|---|---|---|
| English trends blog | `english-trend-blog-pipeline` (this one) | English |
| Excel data cleanup (CleanSheetHQ) | `excel-data-cleanup-pipeline` | English, Excel niche |
| Economic / markets blog | `economic-blog-pipeline` | Korean |

Do not copy topics, drafts, assets, policies, or decisions between them. A topic that
belongs to another blog is rejected here rather than adapted — including a
locale-specific topic that would not match this blog's audience.

## Commit conventions

- One logical change per commit.
- Conventional-commit prefixes: `chore:`, `docs:`, `feat:`, `fix:`, `content:`.
- Reference the article slug when the commit concerns one article.
- Never commit secrets, credentials, or `.env` files.
