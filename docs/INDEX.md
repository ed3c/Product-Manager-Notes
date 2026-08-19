# Documentation & Traceability Index

This file is the human navigation index. Machine/evidence authority remains with exact registry subjects, executable checks, receipts, GitHub metadata, and admitted runtime evidence.

## Start here

```text
README.md
→ AGENTS.md
→ role job contract / competency matrix
→ source + claim + evidence + gap registries
→ exact issue / PR / commit
→ nearest architecture/case/failure artifact
→ evidence receipt
```

## Control planes

| Plane | Canonical owner | Purpose |
|---|---|---|
| Method | `ed3c/skills-shared` | Tech Lead, Shadow Architect, Git Town molecular delivery, verification methods |
| Manager routing | `ed3c/Product-Manager-Notes` | source/requirement/gap graph, stage prompts, cross-repo routing, interview closure |
| Executable evidence | `ed3c/DevOps-Manager-Notes` | CI/CD, runtime, Kubernetes, SLO, failure/recovery, public-safe receipts |
| Human dashboard | Google Sheet | non-authoritative mirror |
| Human narrative | Google Doc | non-authoritative case/interview narrative |

## Trigger-selected support repositories

See `docs/architecture/REPO_INTEGRATION_MAP.md`.

```text
truth-verify-loop          mutable/high-risk external claim verification
openwiki-source-anchoring  source-path/quote anchoring and reproducible documentation verification
runtime-env                secret-free runtime/profile/workload contract when selected
skill-resume-site          public-safe P7 portfolio export only
```

These repositories add evidence/capabilities by trigger; none becomes a second canonical Manager state store.

## Current GitHub subjects

```text
Product bootstrap PR: #5
Product issues: #1 evidence audit, #2 system design, #3 failure library, #4 convergence

DevOps bootstrap PR: #6
DevOps issues: #1 invariants/evidence audit, #2 base delivery,
               #3 observability/load, #4 policy/security/license,
               #5 failure/recovery/postmortem
```

## Architecture

- `docs/architecture/MANAGER_EVIDENCE_GRAPH.md` — cross-repository roles, source→evidence→interview closure, start/completion DAG.
- `docs/architecture/REPO_INTEGRATION_MAP.md` — mandatory planes, trigger-selected support repos, authority boundaries.
- `README.md` — directory→State Machine→DAG ownership, eight-stage program, molecular Stack plan, full data flow.

## Registries

- `registry/sources.yaml` — stable IDs and URL/revision/disclosure state for job/article/PDF/repo/projection sources.
- `registry/claims.yaml` — claim type, real problem, owner, closure state, forbidden promotions.
- `registry/evidence.yaml` — evidence states/ladder; exact evidence records land here.
- `registry/gaps.yaml` — unresolved proof obligations.
- `registry/external-links.yaml` — Google Doc/Sheet projections; URL reachability only.
- `registry/stack-plan.yaml` — planned/observed molecular issue/PR topology.

## Role contract

- `roles/technical-product-manager/job-contract.yaml`
- `roles/technical-product-manager/competency-matrix.yaml`

## Stage prompt pack

- `prompts/README.md` — dispatch rules and handoff schema.
- `prompts/stage-0-subject-authority.md`
- `prompts/stage-1-source-evidence.md`
- `prompts/stage-2-problem-closure-system-design.md`
- `prompts/stage-3-technology-adr.md`
- `prompts/stage-4-tech-lead-stack-plan.md`
- `prompts/stage-5-parallel-implementation.md`
- `prompts/stage-6-shadow-runtime-failure.md`
- `prompts/stage-7-convergence-handoff.md`

Each stage prompt is intended for a fresh ChatGPT session after replacing the exact subject placeholders. A session may not infer branch, commit, issue, path lease, evidence state, predecessor closure, or Human authority from another conversation.

## External projections

- Google Sheet — `https://docs.google.com/spreadsheets/d/18W2xpge7ZgA4WHJd1wsbMOuC5vgCsskCwYeDYPG-twQ/edit`
- Google Doc — `https://docs.google.com/document/d/10qgxR5TxYiZG55cY9wN9ANrkmG_o32vBVrSdd45fgRM/edit`

Canonical routing metadata is `registry/external-links.yaml`. Google state never promotes evidence.

## Evidence closure route

```text
source
→ classified claim
→ requirement / gap
→ architecture + invariant
→ Tech Lead task contract
→ molecular implementation leaf
→ deterministic/runtime oracle
→ failure / negative control
→ corrective change
→ repeated verification
→ exact receipt
→ evidence ceiling review
→ interview-safe narrative
```

A missing link remains visible. Documentation never fills missing proof by assertion.
