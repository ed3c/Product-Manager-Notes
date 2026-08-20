# Documentation & Traceability Index

This is a navigation surface. Canonical authority remains with exact registries, issues/PRs/commits, GitHub Actions artifacts, executable checks and admitted receipts.

## Start here

```text
README.md
→ AGENTS.md
→ docs/PUBLIC_DISCLOSURE_CHECKLIST.md
→ docs/case-studies/INTERNAL_AI_PLATFORM_MVP_DEMO.md
→ docs/milestones/PUBLIC_MANAGER_M4_ROUTING.md
→ roles/technical-product-manager/job-contract.yaml
→ roles/technical-product-manager/competency-matrix.yaml
→ roles/technical-product-manager/interviews/M4_MANAGER_DEMO_STORY.md
→ registry/public-m4-manager-routing.json
→ registry/stack-plan.yaml
→ exact Product/DevOps issue / PR / commit / Actions run / artifact / Local Handoff receipt
```

## Control planes

| Plane | Owner | Purpose |
|---|---|---|
| Reusable method | `ed3c/skills-shared` | Tech Lead / Shadow Architect / Git Town procedures |
| Manager routing | `ed3c/Product-Manager-Notes` | sources, requirements, gaps, Product/System Design, task routing, interview closure |
| Executable proof | `ed3c/DevOps-Manager-Notes` | CI/runtime/ML lifecycle/security/failure/reviewer evidence |
| Human dashboard | Google Sheet | non-authoritative mirror |
| Human narrative | Google Doc | non-authoritative mirror |

## Observed Product Stack

```text
PR #5 bootstrap
└─ PR #8 Full Manager MVP Product contract
   └─ PR #11 public disclosure alignment
      └─ PR #12 public Manager M4 routing                  PASS_BOUNDED_AS_ROUTING
           ↑ PR #9 existing evidence audit                EXACT SIDE INPUT
           ↑ DevOps PR #44 M4 reviewer evidence           EXTERNAL EVIDENCE
           ↑ DevOps PR #45 Local Handoff state            PROCESS DEPENDENCY
           ↓
         issue #4 final interview/evidence convergence    OPEN
```

Cross-repository evidence does not create Git ancestry.

## Exact DevOps M4 evidence

```text
repository        ed3c/DevOps-Manager-Notes
PR                #44
source commit     55d18cdc556ca5d66c67406318ae25196c077fd2
source tree       a4ad37d9baf73a5239f79c516c67b0182420336a
status            PASS_BOUNDED
```

Deterministic reviewer lane:

```text
run               32256802856
artifact          9366615717
digest            sha256:e652cdf3ccb8de7a8655f9148bc6471a29bcaeaef2d55f6255bca2cb2b1e19d3
ceiling           GITHUB_HOSTED_REMOTE_REVIEWER_CONVERGENCE_ONLY
```

Artifact re-verification lane:

```text
run               32256802554
artifact          9366596481
digest            sha256:696f56be2fb637e386941eb313caa7c9448900ad0bad88b3a96119b95315596c
ceiling           GITHUB_HOSTED_ARTIFACT_REDOWNLOAD_AND_REVIEWER_BUNDLE_ONLY
```

The second lane re-downloads and verifies the six exact M2/M3 GitHub Actions archives before admitting required public-safe files into the reviewer packet.

## Local Handoff state

```text
DevOps PR         #45
head              a697c74a11d5d6492eaddb44aabd1a331899ee32
contract run      32257928774 PASS
active item       M4-LOCAL-REVIEWER-001
local execution   NOT_EXERCISED
next substrate    M4-LIVE-SUBSTRATE-002 = BLOCKED_UNRESOLVED
```

Queue-contract PASS is workflow evidence only; it does not prove the local command ran.

## Product M4 artifacts

- `docs/milestones/PUBLIC_MANAGER_M4_ROUTING.md` — role requirement → exact DevOps M4 evidence → Product issue #4 route.
- `registry/public-m4-manager-routing.json` — machine-readable exact M4 subjects and Human/runtime residuals.
- `roles/technical-product-manager/interviews/M4_MANAGER_DEMO_STORY.md` — bounded 90-second, System Design, failure and TPM/DevOps interview narrative.
- `registry/stack-plan.yaml` — Product PR #5/#8/#9/#11/#12 and final #4 convergence topology.

## Closure route

```text
Job / Article / PDF / Repo / Technology
→ source ID / claim classification
→ requirement / gap
→ Product/System Design / ADR
→ Tech Lead DAG / Worker contract
→ molecular DevOps implementation
→ deterministic/runtime/fault receipts
→ failure/recovery/retest
→ exact M4 reviewer convergence
→ Product PR #12 bounded evidence routing
→ Product issue #4 human-facing convergence
→ Google / portfolio projection only after disclosure review
```

## Google projections

- Sheet: `https://docs.google.com/spreadsheets/d/18W2xpge7ZgA4WHJd1wsbMOuC5vgCsskCwYeDYPG-twQ/edit`
- Doc: `https://docs.google.com/document/d/10qgxR5TxYiZG55cY9wN9ANrkmG_o32vBVrSdd45fgRM/edit`

GitHub is canonical. Google reachability and prose cannot promote evidence.

## Residual boundary

```text
live kind/Kubernetes                       NOT_EXERCISED
real Argo CD/Rollouts                      NOT_EXERCISED
local Qwen/llama.cpp                       NOT_EXERCISED
1,000-VU capacity/recovery                 NOT_EXERCISED
real 1,000-user adoption                   OUTSIDE_REPOSITORY_PROOF
production incident history                OUTSIDE_REPOSITORY_PROOF
formal TPM / people-management tenure      HUMAN_ADMIT_REQUIRED
```

Any missing edge remains explicitly open.
