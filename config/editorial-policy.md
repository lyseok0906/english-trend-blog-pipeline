# Editorial Policy

Standards every article in this repository must meet. An article that fails any
requirement here goes back to `content/drafts/`.

## Audience and language

- Audience: English-speaking readers, primarily US.
- Language: US English. US spelling, US date format (September 28, 2026), US number
  formatting, and US-reader-first framing.
- Do not write content that only makes sense in a Korean context, and do not translate
  Korean-market content into English to fill the backlog.
- Plain, direct prose. No filler openings, no padding to reach a word count, no
  repeating the keyword to game a score.

## Sourcing

1. Every factual claim — a figure, a date, an attribution, a quote, a mechanism — must
   trace to a source recorded in `research/sources/<slug>.md` with a link and the date it
   was retrieved.
2. Prefer primary sources: the organisation's own publication, official documentation,
   the original data release, the original statement. Reporting about a primary source is
   a pointer to it, not a substitute for it.
3. A secondary source may be cited only when the primary source is unavailable, and the
   article must say which claim rests on it.
4. Never state a figure or date that no recorded source supports. If it cannot be
   sourced, cut it. Do not hedge an unsourced claim into vagueness to keep it.
5. Time-sensitive claims carry their as-of date in the article text, not only in the
   source notes.
6. Each article ends with a Sources section listing the sources actually used.

## Trend content specifics

Trend articles go stale and are easy to get wrong. Additional requirements:

- Say when the trend was observed and over what period.
- Distinguish what is measured from what is inferred. An observation and an explanation
  of it are separate sentences, and the explanation is labelled as such.
- Do not assert causation from a correlation, and do not present a single source's
  interpretation as established fact.
- No prediction stated as fact. A forecast is attributed to whoever made it.
- Where a claim is contested, say so and give the competing view.

## Structure

- One search intent per article. If a draft serves two intents, it is two articles.
- Title states the specific thing the article answers.
- The answer appears near the top; the reader does not scroll past background to get it.
- Headings describe content, not the template.
- Front matter on every draft: title, slug, meta description, category, focus keyword,
  status, date, and internal-link candidates.

## SEO

- One focus keyword per article, used naturally. No stuffing, no near-duplicate articles
  targeting keyword variants of the same question.
- Meta description written for a human reader, under 160 characters.
- Slug: lowercase, hyphenated, stable. Once an article is published its slug does not
  change.
- Descriptive alt text on every image — what the image shows, not the keyword.
- Internal links only to articles that exist.

## Images

- Screenshots and captured images go in `assets/raw/`; the versions used in the post go
  in `assets/optimized/`.
- Capture in English UI. A non-English interface in a screenshot means recapture, not
  cropping around it.
- Do not present a generated or illustrative image as a real capture.

## What this blog does not publish

- Content that imitates another site, publication, or person.
- Fabricated data, quotes, reviews, testimonials, or case studies.
- Financial, legal, or medical advice. Explaining what a source says is fine;
  recommending an action is not.
- Bulk-generated content that does not answer a distinct reader question.

## QA gates

Two gates, both recorded in `editorial/qa/<slug>.md`.

**Gate 1 — Factual QA.** Every claim checked against the recorded sources, claim by
claim. Result per claim: supported / unsupported / needs revision. Unsupported claims are
removed or sourced before the article moves on.

**Gate 2 — English + SEO QA.** US-English reading pass, search-intent match, title and
meta check, heading structure, internal and external links resolved, alt text present.

Both gates must pass before an article enters `content/ready/`. Passing both is not
approval to publish — that is the user's separate decision.
