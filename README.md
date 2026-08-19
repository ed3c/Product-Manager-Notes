# Product Manager Notes

Private Technical Product Manager preparation and control-plane repository.

This repository turns job requirements, articles, PDFs, technical proposals, and repository evidence into a traceable **Manager Evidence Graph**. It is not a notebook dump: every material claim must route to a requirement, decision, implementation/evidence artifact, failure case, or explicit gap.

## Scope

Primary target: Technical Product Manager / Technical Program Manager roles around ML/LLMOps, internal developer platforms, AI infrastructure, and platform products.

The repository owns:

- job-contract and competency extraction;
- product/system-design case studies;
- PRDs, roadmaps, prioritization, build-vs-buy, migration and adoption decisions;
- manager failure drills and postmortem narratives;
- interview-ready evidence mapping;
- private links to Google Docs/Sheets when they exist;
- routing to public executable evidence without copying or inflating claims.

It does **not** convert simulated work into production tenure, real user adoption, people-management history, or customer claims.

## Canonical state machine

```text
SOURCE_BOUND
→ REQUIREMENT_EXTRACTED
→ COMPETENCY_MAPPED
→ CASE_MODELED
→ DECISION_LOGGED
→ IMPLEMENTATION_EVIDENCE_LINKED
→ FAILURE_EXERCISED
→ CLOSURE_EVIDENCE_BOUND
→ INTERVIEW_READY

any stale / contradicted evidence
→ GAP_REOPENED
```

## Repository topology

```text
Product-Manager-Notes/
├── AGENTS.md
├── README.md
├── roles/
│   └── technical-product-manager/
│       ├── job-contract.yaml
│       ├── competency-matrix.yaml
│       ├── gap-analysis.md
│       ├── system-design/
│       ├── product/
│       ├── failures/
│       └── interviews/
├── registry/
│   ├── sources.yaml
│   ├── claims.yaml
│   ├── evidence.yaml
│   ├── external-links.yaml
│   └── gaps.yaml
├── docs/
│   ├── architecture/
│   ├── decisions/
│   └── case-studies/
└── prompts/
    ├── tech-lead.md
    └── shadow-monitor.md
```

Directories are introduced only when their first real artifact lands; this map is the target contract, not proof that every path already exists.

## Data flow

```text
Job / Article / PDF / Repo
→ Source Registry
→ Requirement + Claim Classification
→ Competency Matrix
→ Product/System Design Case
→ Decision + Trade-off
→ Public or private implementation evidence
→ Failure / Incident Drill
→ Corrective Change
→ Verification Receipt
→ Interview Story
```

## Evidence policy

Use explicit evidence states:

```text
PASS
FAIL
ABSENT
NOT_IMPLEMENTED
NOT_EXERCISED
SKIPPED_BY_POLICY
HUMAN_ADMIT_REQUIRED
```

A design document is not runtime proof. A local load test is not real organizational adoption. A simulated incident must be labeled `DRILL` or `SIMULATION`.

## GitHub / Google boundary

GitHub is canonical for versioned requirements, decisions, issues, PRs, evidence status, and traceability.

Google Docs may hold long-form narratives and interview notes. Google Sheets may mirror a dashboard. Their URLs are edges in `registry/external-links.yaml`; they never replace canonical GitHub state. Missing URLs remain `ABSENT` rather than fake placeholders.

## Shadow Architect monitor

At material checkpoints, review deltas in:

```text
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

For each delta ask:

1. What became newly possible?
2. What must now remain true?
3. How would we know it is false?

`FIRST_GREEN` is never equivalent to closure.

## First milestone

M0 is complete only when the current Technical Product Manager job is compiled into a job contract, competency matrix, gap register, system-design case backlog, manager-failure backlog, and evidence-routing contract.
