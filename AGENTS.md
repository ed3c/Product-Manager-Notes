# AGENTS.md

## Purpose

This public repository is the canonical **Manager orchestration and evidence-routing control plane** for public-safe Product/DevOps Manager evidence. It owns source/requirement/gap identity, Product/System Design contracts, stage prompts, cross-repository task routing, Google projection links and interview closure. Public executable evidence belongs to `ed3c/DevOps-Manager-Notes`; reusable procedure belongs to `ed3c/skills-shared`.

GitHub repository metadata is the visibility authority. Never assume a repository is private because prose says so. A visibility change is Human-owned; if observed visibility disagrees with documentation, stop publication-sensitive work, record `AUTHORITY_DELTA`/`EVIDENCE_DELTA`, and repair the documentation contract without changing visibility automatically.

## Mandatory read order

1. `README.md`
2. `docs/PUBLIC_DISCLOSURE_CHECKLIST.md`
3. `docs/INDEX.md`
4. `docs/architecture/MANAGER_EVIDENCE_GRAPH.md`
5. `docs/architecture/REPO_INTEGRATION_MAP.md`
6. `docs/case-studies/INTERNAL_AI_PLATFORM_MVP_DEMO.md`
7. `roles/technical-product-manager/job-contract.yaml`
8. `roles/technical-product-manager/competency-matrix.yaml`
9. `registry/sources.yaml`
10. `registry/claims.yaml`
11. `registry/evidence.yaml`
12. `registry/gaps.yaml`
13. `registry/external-links.yaml`
14. `registry/stack-plan.yaml`
15. current `prompts/stage-*.md` or `prompts/full-mvp-devops-router.md`
16. exact issue / PR / commit / source subject

When a reusable method is triggered, read its canonical `skills-shared` implementation rather than copying local variants:

```text
skills/agentic-tech-lead-orchestration/
skills/spatial-loop-systems-engineering/
skills/git-town-stacked-pr-worker/
```

Trigger-selected support repositories:

```text
truth-verify-loop          mutable/high-risk external claim verification
openwiki-source-anchoring  source/path/quote verification for generated docs
runtime-env                secret-free runtime/profile/workload contract
skill-resume-site          public portfolio projection after evidence admission
```

No support repository may become a second Manager-state authority or be copied into this public repository merely to make context convenient.

## Public disclosure law

Before writing or exporting public material, apply `docs/PUBLIC_DISCLOSURE_CHECKLIST.md`. Public tracked content must not contain credentials, customer/user private data, employer/client confidential material, private source documents, sensitive prompts, private repository bodies, restricted redistribution material, or unredacted runtime identity. Prefer exact public links and bounded paraphrases over copying source bodies.

Public reachability does not promote evidence. Real tenure/adoption/production claims remain Human/admissible-production evidence boundaries.

## Operating mode

Default `MODE=MONITOR`.

Builder may proceed on reversible notes, architecture, task contracts and bounded repository work. Shadow Architect separately monitors:

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

Intervention:

```text
L0 OBSERVE
L1 WARN
L2 REVIEW
L3 BLOCK
```

Block unsafe/irreversible transitions, private/secret exposure, repository-visibility changes, overlapping mutation authority, evidence laundering and false production/adoption/tenure claims.

## Eight-stage program

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

Start-readiness and completion-readiness are distinct. A stage may start with bounded unknowns but cannot close before its exact completion receipts exist.

Every handoff contains:

```text
repository / branch / commit / tree / issue
state_in / state_out
goal / non-goals
consumed / produced artifacts
start / completion dependencies
allowed / read-only / forbidden paths
resource leases
evals / negative controls
evidence state / ceiling
Shadow deltas / intervention
unknowns / blockers
Local Handoff requirement
next prompt / stage
Human-owned operations
```

## Full Manager MVP routing

`docs/case-studies/INTERNAL_AI_PLATFORM_MVP_DEMO.md` is the Product acceptance contract. Product issues #6/#7 and PR #8 define the reviewer journey and technology policy; they do not prove runtime execution.

Executable work routes to the public DevOps plane:

```text
DevOps #11 / PR #12  Full MVP technology/routing contract
→ DevOps #1 / PR #13 invariant/evidence audit
→ DevOps #2 / PR #14 Core remote FIRST_GREEN
→ parallel remote lanes:
   #3  / PR #36 observability/load
   #4  / PR #38 policy/security
   #7  / PR #39 ML/LLMOps/rollouts
   #8  / PR #37 Demo Console
   #10 / PR #40 supply-chain/fault
→ #5 failure/recovery convergence
→ #9 final reviewer convergence
```

Remote FIRST_GREEN is lane-bounded. Local kind/Kubernetes, local model/llama.cpp, live Argo Rollouts and later failure convergence remain separate proof obligations.

## Tech Lead laws

- Freeze exact subject, objective, non-goals, invariants, task dependencies, acceptance criteria, budgets, evidence lane and Human authority before fan-out.
- A dependency exists only for real artifact/state consumption or an admitted completion receipt.
- Keep task-DAG dependencies separate from Git ancestry.
- Parallel writers require disjoint path/resource leases.
- Worker/LLM/issue/branch/CI self-report is candidate evidence only.
- Every material claim binds an exact source and exact evidence subject or remains explicitly missing.
- `ABSENT`, `NOT_IMPLEMENTED`, `NOT_EXERCISED` and `SKIPPED_BY_POLICY` never become PASS through prose.
- One convergence owner updates shared indexes after prerequisite evidence stabilizes.
- Google Doc/Sheet URLs have zero evidence-promotion authority.

## Molecular Git Town laws

Use `git-town-stacked-pr-worker`:

```text
PATH-DISJOINT + no unmerged consumption → SIBLING
consumes parent unmerged bytes/contract → TRUE_CHILD
smallest behavior + tests + evidence    → TERMINAL_LEAF
shared multi-input closure              → CONVERGENCE
runtime prerequisite                    → PROCESS_DEPENDENCY / LOCAL_HANDOFF
```

Never invent branch/PR/head/merged identities. `registry/stack-plan.yaml` records observed identities and leaves nonexistent subjects `PLANNED`/null.

## Source classification

Classify each significant source claim exactly as one of:

```text
REQUIREMENT
DESIGN_PROPOSAL
ASSUMPTION
OBSERVATION
MEASURED_FACT
EXTERNAL_CLAIM
UNKNOWN
```

Article/PDF/README/diagram presence is not system truth. Mutable/high-risk claims require fresh verification through an admitted verification route.

## Evidence states / ladder

```text
PASS
FAIL
ABSENT
NOT_IMPLEMENTED
NOT_EXERCISED
SKIPPED_BY_POLICY
HUMAN_ADMIT_REQUIRED
```

```text
L0 SOURCE_CLAIM
L1 STATIC_REASONING
L2 DETERMINISTIC_TEST
L3 LOCAL_INTEGRATION
L4 REAL_SUBSTRATE
L5 ADVERSARIAL_OR_CHAOS
L6 PRODUCTION_OBSERVATION
```

Virtual load is not real adoption; local/CI K8s is not production experience; synthetic incident is not production incident; UI/docs do not promote evidence.

## Interview closure

A capability is `INTERVIEW_READY` only through:

```text
job requirement
→ real problem / product-system case
→ decision / trade-off
→ implementation or explicitly bounded simulation
→ failure / negative control
→ corrective action
→ repeated verification
→ exact evidence subject + ceiling
→ concise interview narrative
```

Missing edges keep the gap open.

## Google / GitHub boundary

GitHub is canonical for requirements, source IDs, decisions, issues, PRs, Stack state and evidence. Existing Google Sheet and Doc are non-authoritative human mirrors listed in `registry/external-links.yaml`. Never mirror secret/private/confidential content into public GitHub or a public projection.

## Local Handoff

Only the executable evidence plane compiles local runtime commands. Product may route/link the resulting queue and receipt, but must not infer runtime PASS from queue existence.

## Stop / Human boundaries

Stop on stale subject, overlapping lease, missing predecessor receipt, semantic conflict, private disclosure risk, unbounded side effect, invalid evidence, unavailable physical runtime, unresolved redistribution/license boundary, or Human-owned transition.

Human/trusted-owner operations include semantic conflict resolution, force push, merge/release, production promotion/rollback admission, visibility/permission changes and claims of real production/users/incidents/people-management tenure.
