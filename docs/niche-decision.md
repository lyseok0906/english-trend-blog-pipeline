# Niche Decision

**Status: `CONDITIONAL — NOT FINALIZED`**

This document records a conditional decision. The niche is not settled. It becomes settled
only when the proof gate in `docs/proof-gate-n8n.md` returns GO and the user approves that
result. Until then, `README.md`, `docs/operating-model.md`, and `docs/content-backlog.md`
are not changed on the basis of this document.

## 1. Candidate vertical

**Workflow automation for small teams.**

Small teams that run recurring manual work — intake, checking, reformatting, notifying —
and have no engineer assigned to automate it.

## 2. n8n is a first-tool pilot, not the site identity

n8n is the first tool being evaluated. It is not what this site is about.

This distinction is an operating constraint, not a framing preference:

- The domain, site name, and category structure do not contain `n8n`.
- The site's promise is not "we explain n8n." It is: *here is how a small team automates a
  recurring task, and here is what to do when it breaks — shown with real execution
  results.*
- If n8n proves unsuitable, the tool is replaced and the site continues. Make, Zapier,
  Activepieces and similar tools can occupy the same slot.
- No affiliate program is joined for any single tool. Affiliate enrollment is prohibited
  until the gate passes (see `docs/proof-gate-n8n.md`, prohibitions).

## 3. Out of scope

The following are out of scope for this blog:

- **Company material** — the user's employer, its systems, products, colleagues, or any
  non-public information encountered through work.
- **Development material.**
- **QA material.**

This exclusion covers **anonymized and generalized work-derived cases**. Removing names,
changing numbers, or restating a work situation as a generic example does not bring it into
scope. If the case originates in the user's work, it is out of scope regardless of how it
is presented.

Positioning this blog toward QA teams or operations teams is also out of scope, and has
been removed from every niche document.

**Consequence for the proof gate:** the gate's workflows must be built from synthetic data
in a personal environment, with no production credentials. That requirement already exists
in `docs/proof-gate-n8n.md` §2 and is consistent with this exclusion.

## 4. Evidence standard for operator capability

Operator capability is established only by reproduced evidence.

The following do **not** count as evidence of expertise:

- the presence of a tool's configuration folder or installed files on a machine
- a statement that a tool has been used
- familiarity with a tool's documentation

An earlier revision of the niche comparison inferred the user's expertise from local tool
folders. That reasoning is withdrawn. Installation traces, trial use, sustained operation,
and the ability to diagnose failures are different things, and only the last matters for
this blog's defensibility. The proof gate exists to test it.

## 5. Handling of external traffic statistics

Reported AI Overviews click-through figures — including a −89% figure for news content —
are **directional reference only** and are not used as grounds for a niche decision. That
figure is a single publisher's self-reported number, relayed through secondary coverage,
with no published methodology.

The basis for this blog's direction is that **a new site competes on evergreen
problem-solving content backed by real execution, real errors, and reproduced results** —
not on trend coverage. The primary support for that is this project's own measured history:

| Source | Finding |
|---|---|
| Blog A market validation (2026-09-04) | Weak: the number itself, the definition itself, today's value, general explanation of news. Strong: official data + differences between systems/indicators + time lag + effect on the reader's own money |
| Blog B Pilots A–G (7/7 PASS) | What worked was reproducible evergreen problem-solving — version-specific behavior, a locale bug, a `null` vs `""` trap, edge cases |

## 6. Open items

| # | Item | Status |
|---|---|---|
| 1 | **NO-GO alternative is void.** The previously recorded fallback was a QA automation vertical based on Playwright / Android testing evidence. §3 places QA and development material out of scope, so that fallback no longer exists. A NO-GO result currently has no successor vertical | **Needs user decision.** Not filled in by Claude |
| 2 | **Technical-depth boundary.** §3 excludes development material. The candidate vertical still involves technical mechanics (webhooks, retries, error handling). The boundary between "technical automation content for a small team" and "development material" is not yet defined in writing | Needs user decision before the first topic brief |
| 3 | Niche confirmation | Blocked on proof gate GO + user approval |

## 7. Approval status

The conditional decision in §1–§5 was approved by the user on 2026-09-28 with the revisions
applied here. Confirmation of the niche itself is not approved and is not implied.
