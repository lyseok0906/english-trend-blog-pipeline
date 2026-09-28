# Proof Gate — n8n (14 days)

**Status: `NOT STARTED`**

A 14-day gate that must pass before any content backlog work begins. It relates to the
conditional decision in `docs/niche-decision.md`.

## 1. What this gate measures, and who runs it

This gate does **not** measure whether n8n works. That is already known.

It measures whether the operator can **independently reproduce, explain, and diagnose**
workflows. That is the only durable advantage this blog has, and it cannot be established by
assertion.

**The user runs the gate.** If Claude builds the workflows, the measurement is void.
Claude's role is limited to:

- defining this specification
- preparing test inputs in advance (a malformed payload for W1, a deliberately broken
  workflow JSON for T3)
- reviewing submitted evidence against expected results
- recommending GO / NO-GO

## 2. Environment conditions (required)

| Item | Condition |
|---|---|
| Location | Local — Docker or npx. No cloud account needed |
| Credentials | **No production credentials.** No real API keys, no company systems, no live account connections |
| Data | Synthetic data only. No real personal data and no work data |
| External calls | Public, unauthenticated endpoints only |
| Version | Record the n8n version in each workflow's evidence (current stable is the 2.40.x line) |

These conditions also enforce the out-of-scope rule in `docs/niche-decision.md` §3: nothing
in this gate may originate in the user's work.

**Docker / self-hosting note.** Running n8n locally via Docker or npx is permitted here.
The technical-depth boundary (`docs/niche-decision.md` §4) excludes Docker and self-hosting
as *subject matter* for articles; it does not restrict how the operator runs the tool while
producing evidence. Nothing about the local setup becomes publishable content.

**Evidence location.** Evidence is kept outside this repository until GO is returned and the
user approves — for example a sibling folder such as `C:\blog\_proofgate-n8n\`. It is moved
into the repository only after that.

**JSON sanitization.** Before an exported workflow is retained, remove or replace:

- credential IDs and names
- real hostnames and URLs that are not public
- tokens, keys, passwords
- any personal data hardcoded in the workflow

## 3. Required workflows

### W1 — webhook input → data normalization → saved output

| Item | Detail |
|---|---|
| Purpose | The basic pipeline: take messy external input, normalize it, store it |
| Minimum shape | Webhook trigger → normalization with a **no-code node (Set)** → file / local output |
| Normalization must cover | Trimming whitespace, unifying date format, coercing types, and **distinguishing `null` from an empty string (`""`)** |
| Required failure case | Send a payload with a required field missing. **A missing field does not fail an execution on its own** — it can resolve to an empty value that passes through while the run reports success, so a green checkmark is not evidence that validation works. The workflow must therefore contain an explicit required-field check (an IF node or equivalent no-code test) that routes invalid submissions off the normal path, and that path must be shown being taken |
| Constraint | **No Code node, no JavaScript.** The technical-depth boundary in `docs/niche-decision.md` §4 makes code-node work out of scope for this blog, so the gate must not measure it. If normalization cannot be done with no-code nodes, that is itself a finding and must be reported rather than worked around |

The edge cases for W1 are supplied to the operator in advance, so W1 does **not** test
unprompted discovery of them — hidden-defect detection is measured by T3, which is sealed. W1 is
judged on three things:

1. Whether the difference between `null`, an empty string and a non-breaking space is explained
   and handled **from actual run results**, not restated from the brief.
2. Whether the required-field validation step was built by the operator and the invalid path
   proven.
3. Whether results that contradicted expectations are recorded rather than quietly fixed.

### W2 — scheduled check → change detection → notification

| Item | Detail |
|---|---|
| Purpose | Check on a schedule, notify only when something changed |
| Minimum shape | Schedule trigger → HTTP Request (public endpoint) → compare against stored previous value → notify only on change |
| Notification | No production credentials, so write to a local file or post to a webhook on the same instance rather than an external messenger |
| Required evidence | **Two consecutive runs** — (1) no change → no notification, (2) change → notification fires. Include the stored previous-state value |
| Required failure case | Establish what happens to the schedule when the endpoint returns 5xx or a malformed response |

### W3 — failure handling / retry / error diagnosis

| Item | Detail |
|---|---|
| Purpose | Handling failure. **The heaviest component of the GO decision** |
| Minimum shape | A node that fails + Retry on Fail configured + an Error Workflow / Error Trigger |
| Required evidence | The **verbatim error message**, an execution log showing each retry attempt with timestamps, evidence that the Error Workflow fired, and a **verified fix** |
| Judgment point | Whether the configured retry count and wait interval match what the log actually shows, and whether the operator can state **why** it failed — not merely that it now works |

## 4. Evidence package (identical for all three workflows)

| # | Evidence | Form |
|---|---|---|
| 1 | Screenshots | Full canvas + key node configuration + execution result. **Capture in English UI** — a non-English UI means the screenshots have to be recaptured before they can be used |
| 2 | Exported workflow JSON | After applying the sanitization rules in §2 |
| 3 | Real failure case | Including the verbatim error message text, not a summary |
| 4 | Verified fix | Before/after comparison plus an execution result showing the fix works |

## 5. Schedule

| Day | Work |
|---|---|
| D1–D2 | Stand up the local environment, record the version, confirm it runs with no credentials |
| D3–D5 | W1 — build, failure case, evidence |
| D6–D8 | W2 — build, two-run evidence, failure case |
| D9–D11 | W3 — build, retry log, diagnosis, fix |
| D12 | **T1 — unaided reproduction test** (§6) |
| D13 | **T2 — technical explanation test** (§6) |
| D14 | **T3 — diagnosis test** (§6), assemble the evidence package, Claude reviews, GO / NO-GO recommendation |

## 6. GO tests

The GO condition — that the operator can reproduce, explain, and diagnose independently — is
specified here as three pass/fail tests. Without stated criteria the condition is not
falsifiable.

| Test | Content | Pass criteria |
|---|---|---|
| **T1 — Reproduce** | Rebuild one of W1–W3, named by Claude on the day, from scratch — without notes, the earlier JSON, or earlier screenshots | Within **40 minutes**, output matches expected |
| **T2 — Explain** | Explain how each of the three workflows works, **in Korean**. Cover each node's role and how the shape of the data changes at each step. Claude then asks **three follow-up questions per workflow**, which must be answered | **Zero technical errors** across the explanations and the follow-up answers. No length requirement |
| **T3 — Diagnose** | Given a workflow JSON that Claude has broken in advance, identify the cause **from what the run produces** and fix it | Within **30 minutes**, the identified cause matches the actual cause |

**GO**: T1, T2 and T3 all pass.
**NO-GO**: any one fails.

Notes on T2:

- The test is in **Korean** because the thing being measured is technical understanding, not
  English writing. Grading a written English sample would confound the two, and English
  drafting quality is handled separately by the QA gates in `config/editorial-policy.md`.
- The follow-up questions, not the written explanation, carry the weight. A prepared
  explanation can be assembled without understanding; unscripted follow-ups cannot.
- An earlier revision required the explanation not to be LLM-generated. That requirement is
  removed: it is not verifiable, and the follow-up questions test the same thing directly.

Notes on T3:

- **An error message is not required.** Depending on the webhook output shape and the n8n
  version, a defect can surface with no error at all. Any of the following is valid evidence:
  a verbatim error message, the execution taking the **wrong branch**, or a **wrong or empty
  output** on a run that reports success.
- What the actual run produces is the final authority. Where a recorded expectation conflicts
  with a measured result, the measured result takes precedence.

No automatic extension is granted for a failed test. Whether to extend is the user's
explicit decision; Claude reports only how an extension affects the reliability of the
result.

## 7. Prohibited until the gate passes

| # | Prohibited |
|---|---|
| 1 | Article writing, including drafts and topic briefs |
| 2 | Publishing, including uploading a WordPress draft |
| 3 | Affiliate program enrollment |
| 4 | Confirming the niche |
| 5 | Entering candidates in `docs/content-backlog.md` |
| 6 | Changing the scope definitions in `README.md` or `docs/operating-model.md` |
| 7 | Buying a domain or creating a site |

## 8. NO-GO outcome

If this gate returns NO-GO, the outcome is:

**`PAUSED — niche research restart.`**

- **No automatic pivot to another niche.**
- **No fallback vertical is created.**
- Work stops. Restarting niche research is a separate, deliberate decision by the user.

The earlier fallback (a QA automation vertical based on Playwright / Android testing
evidence) is void under `docs/niche-decision.md` §3. See `docs/niche-decision.md` §7.
