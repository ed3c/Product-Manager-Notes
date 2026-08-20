# Documentation & Traceability Index

This is a navigation surface. Canonical authority remains with exact registries, issues, PRs, commits, executable checks, GitHub Actions artifacts, and admitted receipts.

## Current route

```text
README.md
→ AGENTS.md
→ docs/PUBLIC_DISCLOSURE_CHECKLIST.md
→ docs/milestones/M8_MERGED_EVIDENCE_ROUTING.md
→ docs/audits/M8_REAL_PROBLEM_CLOSURE_AUDIT.md
→ registry/m8-merged-evidence-routing.json
→ registry/m8-real-problem-closure.json
→ registry/product-closure-matrix.yaml
→ registry/stack-plan.yaml
→ DevOps M8 README
→ DevOps handoff/local-handoff-queue.json
→ exact issue / PR / commit / run / artifact / receipt
```

Historical M4 route:

```text
docs/milestones/PUBLIC_MANAGER_M4_ROUTING.md
→ registry/public-m4-manager-routing.json
→ roles/technical-product-manager/interviews/M4_MANAGER_DEMO_STORY.md
```

## Control planes

| Plane | Owner | Purpose |
|---|---|---|
| Reusable method | `ed3c/skills-shared` | Tech Lead / Shadow Architect / Git Town / Local Handoff |
| Manager routing | `ed3c/Product-Manager-Notes` | sources, requirements, decisions, gaps, interview closure |
| Executable evidence | `ed3c/DevOps-Manager-Notes` | implementation, CI, runtime contracts, failure, receipts |
| Human dashboard | Google Sheet | non-authoritative projection |
| Human narrative | Google Doc | non-authoritative projection |

## Exact current subjects

```text
Product M8 base main
  73bb702447c496ab43428126808b1cac40c9a2d2

DevOps main
  commit 5d0c5db1626bf5c1a83334ea864b6a3eb7613df3
  tree   abd7fa38e9aa7ca720d9f110559a1f05b05c2023

DevOps Local Handoff execution subject
  commit   e7b4e23799a3579572598ebd5864a80831d49db4
  tree     0b72b9f09f73d3829db2f138d457a5691641bf79
  rollback bb940bf7d5a3b1f605b79e9fb8f33c463a8ee5a7
  active   M8-LOCAL-REVIEWER-001
```

## Product State Machine

```text
SOURCE_ADMITTED
→ CLAIM_CLASSIFIED
→ REAL_PROBLEM_CLASSIFIED
→ REQUIREMENT_GAP_BOUND
→ PRODUCT_SYSTEM_CONTRACT_ADMITTED
→ DEVOPS_EVIDENCE_REQUESTED
→ REMOTE_EVIDENCE_BOUND
→ DEVOPS_MAIN_INTEGRATED
→ LOCAL_HANDOFF_PENDING
→ PHYSICAL_EVIDENCE_BOUND
→ COMPETENCY_MATRIX_REVERIFIED
→ HUMAN_ADMIT_REQUIRED | INTERVIEW_PACKET_READY
```

Current frontier:

```text
DESIGN_CLOSED + REMOTE_DETERMINISTIC_CLOSED
→ LOCAL_PHYSICAL_OPEN
```

## Real-problem audit

`docs/audits/M8_REAL_PROBLEM_CLOSURE_AUDIT.md` is the canonical public-safe problem → criterion → evidence → residual map.

It normalizes claims from:

```text
job descriptions
articles
PDFs
repositories
technology candidates
```

Source format is not evidence strength. Article/PDF/README presence cannot substitute for a missing implementation or receipt.

## Molecular Stack

```text
Product PR #5 bootstrap
└─ PR #8 Full Manager MVP contract
   └─ PR #11 public disclosure alignment
      └─ PR #12 M4 routing
           ↑ PR #9 TPM evidence audit                  exact side input
           ↑ DevOps PR #44 reviewer                   external evidence

Merged Product follow-up
├─ PR #13 exact TPM evidence integration
├─ PR #15/#17 M8 audit and closure preparation
└─ M8 durable routing/audit convergence               current owner

Merged DevOps executable route
PR #68 M1–M7 backbone
├─ PR #37 Demo Console
├─ PR #38 Policy / Security / License
├─ PR #39 ML / LLMOps
├─ PR #40 Supply Chain / Fault
├─ PR #69 advanced runner contracts
└─ PR #70 M8 main integration / Local Handoff
```

Cross-repository evidence is a typed process/evidence edge, never Git ancestry.

## Local Handoff

```text
M8-LOCAL-REVIEWER-001          ACTIVE
        ↓ real PASS + trusted advancement
M8-LIVE-KIND-002               BLOCKED_BY_PREDECESSOR
        ↓ real PASS + trusted advancement
M8-COMPILE-ADVANCED-QUEUE-003  BLOCKED_BY_PREDECESSOR
        ↓ canonical assertion + trusted advancement
Argo → Model → Synthetic 1,000 VU → Registry Signing
```

Queue contract PASS is not queue execution PASS.

## Issue route

```text
Product bounded contracts closed:
  #1 #2 #3 #6 #7 #10 #12 #14

Close after durable M8 audit merge:
  #16

Keep open final convergence:
  #4

Open DevOps physical/higher-ceiling owners:
  #2 #3 #4 #5 #7 #9 #10 #54 #67
```

Issue state is workflow metadata, not capability evidence.

## Google projections

- Sheet: `https://docs.google.com/spreadsheets/d/18W2xpge7ZgA4WHJd1wsbMOuC5vgCsskCwYeDYPG-twQ/edit`
- Doc: `https://docs.google.com/document/d/10qgxR5TxYiZG55cY9wN9ANrkmG_o32vBVrSdd45fgRM/edit`

GitHub is canonical. Google reachability and prose cannot promote evidence.

## Residual boundary

```text
local deterministic reviewer                  NOT_EXERCISED
live kind/Kubernetes                          NOT_EXERCISED
Argo / model / 1,000 VU / registry signing    NOT_EXERCISED
real production users / incidents / tenure    OUTSIDE_REPOSITORY_PROOF
formal TPM / people-management tenure         HUMAN_ADMIT_REQUIRED
```
