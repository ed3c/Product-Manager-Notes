# AGENTS.md

## Purpose

This repository is the private Technical Product Manager preparation, Manager Evidence Graph, and cross-repository routing control plane.

It owns job/source routing, requirements, competency gaps, stage prompts, Tech Lead task DAGs, Stack planning, external Google links, and interview narrative closure. It does not own public runtime evidence; that belongs to `DevOps-Manager-Notes`.

## Mandatory read order

1. `README.md`
2. `docs/INDEX.md`
3. `roles/technical-product-manager/job-contract.yaml`
4. `roles/technical-product-manager/competency-matrix.yaml`
5. `registry/evidence.yaml`
6. `registry/gaps.yaml`
7. `registry/external-links.yaml`
8. `registry/stack-plan.yaml`
9. current `prompts/stage-*.md` for the admitted stage
10. the exact issue / PR / commit / source subject being acted on
11. the nearest case-study / decision / failure artifact

When reusable procedure is needed, read the canonical owner in `ed3c/skills-shared` rather than copying a divergent local implementation:

```text
skills/agentic-tech-lead-orchestration/
skills/spatial-loop-systems-engineering/
skills/git-town-stacked-pr-worker/
```

Load additional verification/runtime Skills only when their trigger is actually selected.

## Operating mode

Default to `MONITOR`.

Builder work may proceed on reversible notes, cases, tests, prototypes, and bounded implementation. In parallel, maintain a Shadow Architect ledger over material deltas in:

```text
ASSUMPTION
STATE
AUTHORITY
OWNERSHIP
LIFECYCLE
CONCURRENCY
RESOURCE
EXTERNAL_SIDE_EFFECT
FAILURE_SURFACE
EVIDENCE
```

For each material delta ask:

1. What became newly possible?
2. What must now remain true?
3. How would we know it is false?

Intervention levels:

```text
L0 OBSERVE
L1 WARN
L2 REVIEW
L3 BLOCK
```

Use L3 for unsafe/irreversible transitions, evidence laundering, secret/private-data exposure, repository-visibility changes, overlapping mutation authority, or claims that misrepresent simulation/local evidence as production experience.

## Eight-stage execution contract

```text
P0 SUBJECT_AUTHORITY
→ P1 SOURCE_EVIDENCE
→ P2 PROBLEM_CLOSURE_SYSTEM_DESIGN
→ P3 TECHNOLOGY_ADR
→ P4 TECH_LEAD_STACK_PLAN
→ P5 PARALLEL_IMPLEMENTATION
→ P6 SHADOW_RUNTIME_FAILURE
→ P7 CONVERGENCE_HANDOFF
```

Start-readiness and completion-readiness are separate. A stage may start with bounded unknowns, but it may not close until its required exact-subject evidence is admitted.

Every stage handoff must record:

```text
subject: repository / branch / commit / tree / issue
state_in / state_out
consumed artifacts
produced artifacts
invariants / negative controls
start dependencies
completion dependencies
path/resource leases
evidence state + evidence ceiling
Shadow deltas + intervention level
unknowns / blockers
local runtime handoff required?
next prompt/stage
Human-owned operations
```

A new ChatGPT conversation receives one zero-context stage prompt from `prompts/` plus exact current subjects. Do not rely on undocumented context from another conversation.

## Tech Lead laws

- Freeze exact subject, objective, non-goals, invariants, dependencies, acceptance criteria, budgets, authority, and evidence lane before Worker fan-out.
- A dependency exists only when a task consumes another task's unmerged contract/bytes/state or requires its admitted completion receipt.
- Keep start edges and completion edges distinct.
- Parallel writers require disjoint file/resource leases.
- Worker, LLM, issue, branch, CI, or process self-report is candidate evidence only.
- Every claim binds to an exact source and exact evidence subject or remains explicitly missing.
- `ABSENT`, `NOT_IMPLEMENTED`, and `NOT_EXERCISED` never become `PASS` through prose.
- Google Docs/Sheets are narrative/dashboard edges; GitHub remains canonical.
- Public evidence must be sanitized and independently readable; never expose private URLs, credentials, employers, clients, customer data, device IDs, or unverifiable metrics.
- A drill is always labeled `DRILL` or `SIMULATION`.
- Human interview narratives may summarize evidence but may not widen its ceiling.
- One convergence owner updates shared indexes after prerequisite artifacts are stable.

## Git Town / molecular Stack laws

Use the canonical `git-town-stacked-pr-worker` method.

```text
PATH-DISJOINT + no unmerged consumption → SIBLING
consumes parent unmerged bytes/contract   → TRUE_CHILD
smallest behavior + tests + evidence      → TERMINAL_LEAF
shared indexes after prerequisites        → CONVERGENCE
runtime/provider prerequisite only        → EXTERNAL_EVIDENCE / PROCESS_DEPENDENCY
```

Never invent a branch, PR, head SHA, merged state, or ancestry. Until a subject exists, record `PLANNED` and `null` identity in `registry/stack-plan.yaml`.

Workers must not autonomously resolve semantic conflicts, force push, ship, merge, release, promote, change repository visibility, or convert an issue UI state into evidence closure.

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

An article, PDF, diagram, README, or technology README is a source; it is not system truth. Mutable external claims require fresh verification before promotion.

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

Evidence ladder:

```text
L0 SOURCE_CLAIM
L1 STATIC_REASONING
L2 DETERMINISTIC_TEST
L3 LOCAL_INTEGRATION
L4 REAL_SUBSTRATE
L5 ADVERSARIAL_OR_CHAOS
L6 PRODUCTION_OBSERVATION
```

Lower evidence does not promote itself into a higher lane. Virtual users are not real adoption; local Kubernetes is not production tenure; a simulated incident is not a production incident.

## Closure rule

A competency is `INTERVIEW_READY` only when it has:

```text
job requirement
→ system/product case
→ decision/trade-off
→ implementation or explicitly bounded simulation evidence
→ failure/negative case
→ corrective action
→ repeated verification
→ exact evidence subject + ceiling
→ concise interview narrative
```

If any required edge is missing, keep the gap open.

## Cross-repository boundary

```text
Product-Manager-Notes
  canonical requirements / gaps / prompts / routing / narrative state
        ↓ public-safe evidence request
DevOps-Manager-Notes
  executable platform/reliability evidence
        ↓ exact public receipt/PR/commit
Product-Manager-Notes evidence registry
```

`skills-shared` supplies reusable procedures and does not own consumer issue/branch/runtime state. Google Docs/Sheets may mirror canonical GitHub state but may not override it.

## Local Handoff Execution Queue

Compile Local Handoff only after the session reaches a genuine local host/runtime/provider/forge boundary. Each item must bind:

```text
entry exact subject
→ required capabilities
→ concrete argv + cwd + timeout
→ sanitized durable receipt
→ required PASS exit
→ next item
```

Queue validation proves queue shape, not execution. Queue advancement, issue closure, merge, release, promotion, visibility change, permission widening, rollback admission, and semantic conflict resolution remain outside unattended Worker authority.

## Stop conditions

Stop or escalate when any of these occurs:

```text
subject/revision drift
overlapping writer/resource lease
missing required predecessor receipt
unbounded side effect or retry
secret/private disclosure risk
semantic conflict
wrong evidence lane / evidence laundering
runtime required but unavailable
budget exhaustion
Human-owned transition reached
```
