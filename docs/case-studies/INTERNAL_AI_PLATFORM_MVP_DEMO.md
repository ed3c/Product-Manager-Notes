# Internal AI Platform — Full Manager MVP Demo Contract

## Objective

Build one coherent, reviewer-facing demo that proves the *technical* parts of the Technical Product Manager and DevOps Manager job requirements without inventing tenure, production adoption, or people-management history.

The demo is an internal AI platform for a potential 1,000+ internal-user environment. The executable public evidence lives in `ed3c/DevOps-Manager-Notes`; this private repository owns the product contract, requirement mapping, trade-offs, and interview narrative.

## Job requirement → demo capability

| Requirement | Demo capability | Executable owner |
|---|---|---|
| TPM: ML/LLMOps lifecycle | model/prompt/config version → offline eval → promotion → canary → monitoring → rollback | `DevOps-Manager-Notes#7` |
| TPM: internal platform scale | typed control plane, quotas/backpressure design, reproducible 1,000-VU load evidence | `DevOps-Manager-Notes#2`, `#3` |
| TPM: technical communication / product judgment | PRD, ADRs, build-vs-buy, evidence ceilings, failure decisions | Product `#2`, `#3`, `#7` |
| DevOps: Python / Git / Docker / Kubernetes | Python control plane, GitHub CI, OCI image, kind/Kubernetes | `DevOps-Manager-Notes#2` |
| DevOps: CI/CD / deployment best practices | GitHub Actions → policy/security → Argo CD → Argo Rollouts | `#2`, `#4`, `#7`, `#10` |
| DevOps: data-driven ownership | SLI/SLO, rollout analysis, load/capacity, incident decision record | `#3`, `#5` |
| DevOps: leadership/management | ownership/on-call/delegation/incident-command design and explicit decision log | `#5`; tenure remains outside repo proof |

## Reviewer user journey

```text
1. Open Demo Console
2. Inspect exact source/model/prompt/deployment identity
3. Run or inspect offline evaluation
4. Promote a candidate that passes the frozen threshold
5. Observe immutable image/model evidence and supply-chain gates
6. Deploy to local Kubernetes through GitOps
7. Watch canary analysis with SLO/business metrics
8. Inject one bounded fault / seeded bad candidate
9. Observe automatic/manual rollback and incident state
10. Read corrective change and same-failure re-test receipt
11. Open exact GitHub/receipt evidence from the console
```

The deterministic demo path must not require paid API keys. A real-provider or GPU lane is optional evidence and must remain a distinct subject.

## Mandatory technology set

The default distribution path avoids dependencies that force source disclosure of this project. Top-level license status is not a blanket legal clearance for transitive packages, images, plugins, hosted services, or model artifacts.

### Application and persistence

- Python + FastAPI — API/service plane; MIT.
- Pydantic — typed API/evidence contracts; MIT.
- PostgreSQL — durable control-plane state; PostgreSQL license.
- SQLAlchemy — persistence abstraction; MIT.
- Alembic — schema migration; MIT.

### Demo UI

- React — reviewer-facing console; MIT.
- Vite — frontend build; MIT.
- TanStack Query — typed server-state synchronization; MIT.
- Apache ECharts — SLO/eval/rollout/incident visualizations; Apache-2.0.

### ML/LLMOps

- MLflow — experiment/evaluation/model registry lifecycle; Apache-2.0.
- llama.cpp — deterministic local LLM serving option; MIT.
- Qwen2.5-0.5B-Instruct-GGUF — initial tiny demo model candidate; Apache-2.0 model license. Model digest/license remain a separate artifact contract.

A production-shaped GPU lane may later use vLLM (Apache-2.0) and/or KServe (Apache-2.0), but the core demo does not depend on GPU availability.

### Delivery and runtime

- Docker CLI + Moby — container workflow; Apache-2.0 at the named repos.
- Colima (MIT) or Rancher Desktop (Apache-2.0) — local engine options; Docker Desktop terms are a separate subject.
- kind + Kubernetes — local substrate/orchestration; Apache-2.0.
- Argo CD — GitOps desired/observed reconciliation; Apache-2.0.
- Argo Rollouts — canary/progressive delivery; Apache-2.0.

### Observability and reliability

- OpenTelemetry Collector — telemetry plane; Apache-2.0.
- Prometheus — SLI/SLO/rollout analysis; Apache-2.0.
- Jaeger — distributed tracing UI/store for the demo; Apache-2.0.
- Locust — reproducible synthetic load; MIT.
- Toxiproxy — bounded dependency/network fault injection; MIT.

### Policy, security, and supply chain

- OPA — deployment/admission policy; Apache-2.0.
- Trivy — vulnerability/license scanning; Apache-2.0.
- Syft — SBOM generation; Apache-2.0.
- Cosign — image/artifact signing and verification; Apache-2.0.

### Test and CI

- pytest — deterministic/unit/integration/failure tests; MIT.
- GitHub Actions — CI/publication service; commercial/service terms are separate from repository dependency licenses.

## State machine

```text
SOURCE_BOUND
→ CANDIDATE_REGISTERED
→ EVAL_RUNNING
→ EVAL_REJECTED | PROMOTION_ELIGIBLE
→ ARTIFACT_VERIFIED
→ DEPLOYMENT_PENDING
→ CANARY_RUNNING
→ CANARY_REJECTED | PROMOTED
→ OBSERVED
→ FAILURE_INJECTED
→ DEGRADED
→ MITIGATING
→ RECOVERED
→ CORRECTIVE_CHANGE_BOUND
→ REVERIFIED
→ DEMO_EVIDENCE_READY
```

Illegal transitions:

```text
EVAL_PASS → PRODUCTION_PROVEN
LOCAL_K8S_PASS → PRODUCTION_INFRASTRUCTURE_EXPERIENCE
1000_VU_PASS → 1000_REAL_USERS
DRILL_COMPLETE → PRODUCTION_INCIDENT_HISTORY
MODEL_REPO_LICENSE → ALL_MODEL/IMAGE/TRANSITIVE_LICENSES_CLEARED
UI_GREEN → BACKEND_EVIDENCE_PASS
```

## Product success metrics

The demo uses *evidence metrics*, not fabricated business metrics:

- 100% of visible claims link to an exact requirement/evidence subject or an explicit missing state.
- 100% of deployment candidates bind Git SHA, container digest, model/prompt/config version, and evidence lane.
- seeded bad candidate is detected before full promotion.
- rollback returns to a known previous-good identity.
- same planted failure is prevented or detected after corrective change.
- 1,000-VU experiment reports p50/p95/p99/error/resource metadata when the admitted local environment supports it.

## Build-vs-buy rule

The demo remains runnable without proprietary SaaS. Managed services may be documented as production alternatives when they reduce operational burden, but they cannot become hidden prerequisites for CI or local reproduction.

## Evidence convergence

```text
Product requirement / decision
        ↓
DevOps issue + exact implementation subject
        ↓
unit/integration/runtime/fault receipt
        ↓
public Demo Console
        ↓
Product evidence registry
        ↓
interview narrative
```

Final executable convergence owner: `ed3c/DevOps-Manager-Notes#9`.
Product-side acceptance/evidence contract: `ed3c/Product-Manager-Notes#6`.
Technology ADR owner: `ed3c/Product-Manager-Notes#7`.
