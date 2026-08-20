# M8 — REAL PROBLEM CLOSURE AUDIT

Status: `PASS_BOUNDED`

This audit classifies claims from the role description, articles, PDFs, repositories, and technology candidates by the **real problem they imply**. Source format is not evidence strength.

## Closure scale

```text
DESIGN_CLOSED
  invariants, architecture, Product contract, or ADR admitted

REMOTE_DETERMINISTIC_CLOSED
  executable CI, deterministic oracle, or bounded hosted receipt admitted

LOCAL_PHYSICAL_OPEN
  bounded runner exists but a real local receipt is absent

PRODUCTION_OPEN
  no production observation or organizational admission

HUMAN_ADMIT_REQUIRED
  employment, people, real-user, or real-incident evidence must be supplied by the owner
```

A problem can be closed at one ceiling while remaining open at a higher ceiling.

## Real-problem closure matrix

| Real problem derived from sources | Falsifiable closure criterion | Merged evidence | Current verdict | Residual owner |
|---|---|---|---|---|
| Product requirements drift from implementation | requirement → issue → PR → exact evidence subject → residual is traceable | Product registries plus DevOps M1–M8 indexes | `REMOTE_DETERMINISTIC_CLOSED` | Product #4 |
| Architecture remains slideware | typed API, persistence/migration, immutable artifact identity, business oracle, and test receipt exist | FastAPI/Pydantic/PostgreSQL/SQLAlchemy/Alembic/Docker/K8s contracts | remote closed; live K8s open | DevOps #2 |
| Infrastructure green hides business failure | liveness/readiness and business correctness are separate; planted business failure is visible | forced business FAIL while infrastructure remains healthy | `REMOTE_DETERMINISTIC_CLOSED` | DevOps #2/#5 |
| Delivery lacks SLI/SLO and capacity proof | telemetry identity, named workload/window, percentile/failure gates, saturation evidence | OTel/Prometheus and bounded remote load; 1,000-VU runner contract | remote closed; `LOCAL_PHYSICAL_OPEN` | DevOps #3/#54 |
| Policy and security gates are decorative | planted invalid input must be rejected by fail-closed gates | OPA positive/negative controls, Trivy, license metadata rejection | checked scope closed | DevOps #4; Human/legal for wider clearance |
| Model changes lack lifecycle and rollback | model/prompt/config/data identities, offline eval, promotion decision, rejection, exact rollback | MLflow lifecycle and seeded canary/business rejection | deterministic closed; local model/live delivery open | DevOps #7/#54 |
| GitOps is claimed without controllers | exact manifests/digests, scoped ownership, cleanup, controller readiness receipt | self-contained ephemeral-kind Argo runner contract | `LOCAL_PHYSICAL_OPEN` | DevOps #7/#54 |
| Progressive delivery lacks real reconciliation/canary proof | Argo Application observed at target revision and Rollout analysis visibly accepts/rejects | contracts only | `NOT_EXERCISED` | DevOps #7/#9 |
| Supply-chain proof ends before registry storage | SBOM, digest, scan, sign/verify, tamper rejection, and registry-stored signature | Syft/Cosign/tamper evidence plus local registry runner | remote closed; registry physical open | DevOps #10/#54 |
| Incident handling stops at mitigation | trigger → detect → authority → recover → postmortem → corrective change → same-failure re-test | seven deterministic DRILL scenarios and runbooks | `REMOTE_DETERMINISTIC_CLOSED_AS_DRILL` | DevOps #5 |
| Reviewer cannot understand scattered receipts | one public reviewer route, UI, exact evidence packet, explicit ceilings | Manager Demo Console and reviewer convergence | remote closed | DevOps #9 |
| Parallel Agent work loses ownership and dependencies | path/resource leases, Git ancestry ≠ task DAG, molecular Stack, single convergence owner | `skills-shared` method and merged Stack indexes | design/repository-exercised | DevOps #67 for hygiene only |
| Local capability is falsely marked complete | one ACTIVE queue item, exact predecessor receipt admission, cleanup and trusted advancement | canonical M8 Local Handoff queue | contract closed; `LOCAL_PHYSICAL_OPEN` | DevOps #2/#9/#54 |
| Commercial-use selection is treated as blanket legal clearance | permissive default plus separate transitive/image/model/service admission | Product technology ADR and DevOps license/policy checks | design and checked metadata closed; blanket clearance forbidden | Product/DevOps #4 + Human/legal |
| Manager experience is inferred from portfolio code | technical evidence and Human employment/people evidence remain distinct | competency/evidence registries keep tenure/adoption residuals open | `HUMAN_ADMIT_REQUIRED` | Product #4 / owner |

## Closure State Machine

```text
SOURCE_CLAIM
→ REAL_PROBLEM_CLASSIFIED
→ CLOSURE_CRITERION_BOUND
→ PRODUCT_CONTRACT_BOUND
→ DEVOPS_EVIDENCE_REQUESTED
→ DESIGN_CLOSED | REMOTE_DETERMINISTIC_CLOSED
→ LOCAL_PHYSICAL_OPEN
→ LOCAL_RECEIPT_ADMITTED
→ PRODUCTION_OPEN | HUMAN_ADMIT_REQUIRED
→ INTERVIEW_CLAIM_ADMITTED
```

Current portfolio frontier:

```text
DESIGN_CLOSED + REMOTE_DETERMINISTIC_CLOSED
→ LOCAL_PHYSICAL_OPEN
```

## Article / PDF / Repo admission law

A source may establish a requirement, proposal, observation, or external claim. It cannot establish system closure by itself.

```text
Article/PDF/README/diagram presence
  != implementation
  != runtime observation
  != production experience
```

For every material source claim, record:

```text
source identity
claim type
real problem
closure criterion
owner
falsifier
exact evidence subject or missing state
highest evidence ceiling
```

Mutable or high-risk public claims require fresh verification. Protected content must be linked or paraphrased unless redistribution is explicitly admitted.

## Directory and evidence flow

```text
registry/sources.yaml
→ registry/claims.yaml
→ real-problem audit
→ roles/technical-product-manager/*
→ registry/gaps.yaml
→ DevOps issue / PR / receipt
→ registry/evidence.yaml
→ Product #4 final convergence
```

## Residual evidence

```text
local deterministic reviewer             NOT_EXERCISED
live kind/Kubernetes application smoke   NOT_EXERCISED
Argo controllers                         NOT_EXERCISED
Argo CD Application reconciliation       NOT_EXERCISED
live Rollouts canary                     NOT_EXERCISED
llama.cpp/model inference                NOT_EXERCISED
synthetic 1,000 VU                       NOT_EXERCISED
registry-stored signing                  NOT_EXERCISED
real production users/adoption           OUTSIDE_REPOSITORY_PROOF
real production incidents/tenure         OUTSIDE_REPOSITORY_PROOF
formal TPM tenure                        HUMAN_ADMIT_REQUIRED
people-management tenure                 HUMAN_ADMIT_REQUIRED
```

## Source and mirror law

- GitHub exact issues, merged PRs, executable checks, and admitted receipts are canonical.
- Google Doc and Sheet may mirror URLs and narratives but cannot promote a verdict.
- A closed issue records completion of its own bounded contract, not every higher evidence level.
- A merged PR records repository integration, not physical runtime.
- A DRILL remains a DRILL.

## Audit verdict

```text
Product source/problem/requirement routing    CLOSED_AT_M8_BOUNDED_CEILING
DevOps remote deterministic evidence          CLOSED_AT_NAMED_CEILINGS
Local physical evidence                       OPEN
Production observation                        OPEN
Human employment/people evidence              HUMAN_ADMIT_REQUIRED
```
