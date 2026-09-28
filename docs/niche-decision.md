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
  until the gate passes.

## 3. Out of scope — subject matter

The following are out of scope for this blog:

- **Company material** — the user's employer, its systems, products, colleagues, or any
  non-public information encountered through work.
- **Development material.**
- **QA material.**

This exclusion covers **anonymized and generalized work-derived cases**. Removing names,
changing numbers, or restating a work situation as a generic example does not bring it into
scope. If the case originates in the user's work, it is out of scope regardless of how it
is presented.

Positioning this blog toward QA teams or operations teams is also out of scope.

## 4. Technical-depth boundary

This blog is a **no-code / low-code** publication. The boundary below governs what articles
may cover.

### Allowed

- n8n workflows built in the **UI**, using no-code / low-code nodes
- **public services** as integration targets
- **synthetic data** in all examples

### Excluded

- Code-node tutorials
- JavaScript
- Docker
- Self-hosting
- Infrastructure
- API implementation
- Authentication and security architecture
- All company-, development-, and QA-derived material (§3)

### What this boundary governs, and what it does not

This boundary applies to **published subject matter**. It does not govern the mechanics of
how the operator runs a tool while producing evidence.

Concretely: running n8n locally via Docker or npx to build gate evidence is **allowed**,
because that is production mechanics, not subject matter. Writing an article that explains
how to run n8n in Docker is **excluded**. The same split applies to self-hosting generally.

### Downstream consequences

| Area | Consequence |
|---|---|
| Proof gate W1 | Normalization must be built with a **no-code node (Set)**, not a Code node. A gate that tested Code-node skill would be measuring a capability the blog is not allowed to use. `docs/proof-gate-n8n.md` §3 is updated accordingly |
| Audience | Excluding self-hosting content skews readership toward hosted/cloud users. This **reduces** the affiliate leakage previously recorded — self-hosted readers do not convert on a cloud referral, and they are no longer the target |
| Entry angle | The "self-hosted environment reproduction conditions" angle recorded in earlier niche research is void. Remaining angles: what actually broke after a version change, undocumented migration traps, and trade-offs between approaches the official docs stay neutral on |

## 5. Evidence standard for operator capability

Operator capability is established only by reproduced evidence.

The following do **not** count as evidence of expertise:

- the presence of a tool's configuration folder or installed files on a machine
- a statement that a tool has been used
- familiarity with a tool's documentation

An earlier revision of the niche comparison inferred the user's expertise from local tool
folders. That reasoning is withdrawn. Installation traces, trial use, sustained operation,
and the ability to diagnose failures are different things, and only the last matters for
this blog's defensibility. The proof gate exists to test it.

## 6. Handling of external traffic statistics

Reported AI Overviews click-through figures — including a −89% figure for news content —
are **directional reference only** and are not used as grounds for a niche decision. That
figure is a single publisher's self-reported number, relayed through secondary coverage,
with no published methodology.

The basis for this blog's direction is that **a new site competes on evergreen
problem-solving content backed by real execution, real errors, and reproduced results** — not on
trend coverage.

That position does not rest on the figures above. It rests on measured results from the
operator's prior publishing work, recorded outside this repository, which found two things
consistently:

- **Weak:** the bare number, the definition, today's current value, and general explanation of
  news — all of it competing directly with the search engine's own answer and with
  higher-authority publishers.
- **Strong:** reproducible, evergreen problem-solving — version-specific behaviour, environment
  and locale-dependent failures, and edge cases where the documented answer and the observed
  answer differ.

Those results belong to separate projects and are deliberately not restated here (see §3). They
are cited as the origin of this position, not reproduced as content.

## 7. NO-GO outcome

If the proof gate returns NO-GO, the outcome is:

**`PAUSED — niche research restart.`**

Explicitly:

- **No automatic pivot to another niche.**
- **No fallback vertical is created**, by Claude or otherwise.
- Work stops. Niche research restarts as a separate, deliberate decision by the user.

This replaces the earlier fallback (a QA automation vertical based on Playwright / Android
testing evidence), which is void under §3.

## 8. Open items

| # | Item | Status |
|---|---|---|
| 1 | Niche confirmation | Blocked on proof gate GO + user approval |

## 9. Approval status

The conditional decision in §1–§7 was approved by the user on 2026-09-28. Confirmation of
the niche itself is not approved and is not implied.
