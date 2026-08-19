# AGENTS.md

## Purpose

This repository is the private Technical Product Manager preparation and evidence-routing control plane.

## Read order

1. `README.md`
2. `roles/technical-product-manager/job-contract.yaml`
3. `roles/technical-product-manager/competency-matrix.yaml`
4. `registry/evidence.yaml`
5. `registry/gaps.yaml`
6. the nearest case-study / decision / failure artifact

## Operating mode

Default to `MONITOR`.

Builder work may proceed on reversible notes, cases, tests, and prototypes. In parallel, maintain a Shadow Architect ledger over material deltas in state, authority, ownership, lifecycle, concurrency, resources, external side effects, failure surface, and evidence.

For each material delta ask:

1. What became newly possible?
2. What must now remain true?
3. How would we know it is false?

Use intervention levels:

```text
L0 OBSERVE
L1 WARN
L2 REVIEW
L3 BLOCK
```

Use L3 only for unsafe or irreversible transitions, evidence laundering, secret/private-data exposure, repository-visibility changes, or claims that would misrepresent simulation/local evidence as production experience.

## Tech Lead laws

- Contracts before task fan-out.
- Dependencies must be real consumption edges, not topic similarity.
- Parallel writers must have disjoint file/resource scopes.
- Worker or LLM self-report is candidate evidence only.
- Every claim binds to an exact source and exact evidence subject.
- `ABSENT` and `NOT_EXERCISED` never become `PASS` through prose.
- Google Docs/Sheets are external narrative/dashboard edges; GitHub remains canonical.
- Public evidence must be sanitized and independently readable; never expose private URLs, credentials, employers, clients, customer data, or unverifiable metrics.
- A drill is always labeled `DRILL` or `SIMULATION`.
- Human interview narratives may summarize evidence but may not widen what that evidence proves.

## Source classification

Classify every significant source statement as exactly one of:

```text
REQUIREMENT
DESIGN_PROPOSAL
ASSUMPTION
OBSERVATION
MEASURED_FACT
EXTERNAL_CLAIM
UNKNOWN
```

## Evidence states

```text
PASS
FAIL
ABSENT
NOT_IMPLEMENTED
NOT_EXERCISED
SKIPPED_BY_POLICY
HUMAN_ADMIT_REQUIRED
```

## Closure rule

A competency is `INTERVIEW_READY` only when it has:

```text
job requirement
→ system/product case
→ decision/trade-off
→ implementation or bounded simulation evidence
→ failure/negative case
→ corrective action
→ verification
→ concise interview narrative
```

If any required edge is missing, keep the gap open.

## Cross-repository boundary

`DevOps-Manager-Notes` may provide public executable platform/reliability evidence. This private repository may reference that public evidence. The public repository must not depend on private URLs or private repository state to remain understandable.

Repository visibility is a Human-owned boundary and must never be changed by an agent.
