# AGENTS.md

## Purpose

This public repository is the canonical **Manager requirement, decision, and evidence-routing control plane**. It owns source and claim identity, Product/System Design contracts, competency gaps, cross-repository task routing, stage prompts, Google projection links, and interview closure.

`ed3c/DevOps-Manager-Notes` owns executable public evidence. `ed3c/skills-shared` owns reusable Tech Lead, Shadow Architect, Git Town, and Local Handoff procedures.

GitHub is canonical. Public visibility does not widen evidence. Visibility, permissions, force-push, release, production authority, credentials, semantic conflicts, and real-experience admission remain Human-owned.

## Mandatory read order

1. `README.md`
2. `docs/PUBLIC_DISCLOSURE_CHECKLIST.md`
3. `docs/INDEX.md`
4. `docs/milestones/M8_MERGED_EVIDENCE_ROUTING.md`
5. `docs/audits/M8_REAL_PROBLEM_CLOSURE_AUDIT.md`
6. `docs/architecture/MANAGER_EVIDENCE_GRAPH.md`
7. `docs/architecture/REPO_INTEGRATION_MAP.md`
8. `docs/case-studies/INTERNAL_AI_PLATFORM_MVP_DEMO.md`
9. `roles/technical-product-manager/job-contract.yaml`
10. `roles/technical-product-manager/competency-matrix.yaml`
11. `registry/sources.yaml`
12. `registry/claims.yaml`
13. `registry/evidence.yaml`
14. `registry/gaps.yaml`
15. `registry/m8-merged-evidence-routing.json`
16. `registry/m8-real-problem-closure.json`
17. `registry/product-closure-matrix.yaml`
18. `registry/external-links.yaml`
19. `registry/stack-plan.yaml`
20. current DevOps `main` README and `handoff/local-handoff-queue.json`
21. exact issue / PR / commit / Actions run / artifact / receipt
22. current `prompts/stage-*.md` or `prompts/full-mvp-devops-router.md`

Historical M4 routing remains available through `docs/milestones/PUBLIC_MANAGER_M4_ROUTING.md` and `registry/public-m4-manager-routing.json`; it is not the current frontier.

When a reusable method is triggered, read the canonical `skills-shared` implementation rather than copying a local variant:

```text
skills/agentic-tech-lead-orchestration/
skills/spatial-loop-systems-engineering/
skills/git-town-stacked-pr-worker/
```

Trigger-selected support repositories:

```text
truth-verify-loop          mutable/high-risk public claim verification
openwiki-source-anchoring  exact source/path/quote support verification
runtime-env                secret-free runtime/profile/workload contracts
skill-resume-site          public portfolio projection after admission
```

No support repository becomes a second Manager-state authority.

## Current exact subjects

```text
Product repository        ed3c/Product-Manager-Notes
Product M8 base main      73bb702447c496ab43428126808b1cac40c9a2d2

DevOps repository         ed3c/DevOps-Manager-Notes
DevOps main               5d0c5db1626bf5c1a83334ea864b6a3eb7613df3
DevOps main tree          abd7fa38e9aa7ca720d9f110559a1f05b05c2023

Local Handoff commit      e7b4e23799a3579572598ebd5864a80831d49db4
Local Handoff tree        0b72b9f09f73d3829db2f138d457a5691641bf79
Local Handoff rollback    bb940bf7d5a3b1f605b79e9fb8f33c463a8ee5a7
Local Handoff active      M8-LOCAL-REVIEWER-001
```

A mutable current head and an admitted historical evidence subject are different identities. Never relabel an older artifact as evidence for a newer head.

## Operating mode

Default `MODE=MONITOR`.

Builder may perform reversible notes, architecture, issue/PR routing, bounded repository changes, tests, and candidate evidence generation. Shadow Architect independently monitors:

```text
ASSUMPTION_DELTA
STATE_DELTA
AUTHORITY_DELTA
OWNERSHIP_DELTA
LIFECYCLE_DELTA
CONCURRENCY_DELTA
RESOURCE_DELTA
EXTERNAL_SIDE_EFFECT_DELTA
FAILURE_SURFACE_DELTA
EVIDENCE_DELTA
CONTRACT_DRIFT
```

For every material delta ask:

1. What became newly possible?
2. What must remain true?
3. Which oracle proves it false?

Intervention:

```text
L0 OBSERVE
L1 WARN
L2 REVIEW
L3 BLOCK
```

L3 includes unsafe or irreversible behavior without rollback, secrets/private disclosure, visibility/permission widening, unbounded load/fault/download/resource behavior, overlapping mutation ownership, semantic conflict, failed cleanup, stale exact subjects, fixture/live laundering, or unsupported public career claims.

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

Start-readiness and completion-readiness are separate. A readable contract may make a task startable; only the owning evidence lane and admitted completion receipts can close it.

Every zero-context handoff records:

```text
repository / branch / commit / tree / issue
state_in / state_out
goal / non-goals
consumed / produced artifacts
start / completion dependencies
allowed / read-only / forbidden paths
path and resource leases
oracles / negative controls
resource budgets / cleanup / rollback
evidence state / ceiling
Shadow deltas / intervention
unknowns / blockers
Local Handoff requirement
next prompt / stage
Human-owned operations
```

## Current Product checkpoint

```text
M4 public Manager routing                         PASS_BOUNDED_AS_ROUTING
M8 merged DevOps evidence routing                PASS_BOUNDED
M8 real-problem closure audit                    PASS_BOUNDED
Product issue #4 final convergence               KEEP_OPEN
Product issue #16 audit integration              CLOSE_AFTER_M8_MERGE
```

M8 closes only Product routing/audit obligations. Physical local execution and Human-admitted facts remain separate.

## M8 source-closure law

Before declaring an Article, PDF, repository, technology candidate, or job-description claim closed:

1. classify the **real problem**, not only the source format;
2. bind a falsifiable closure criterion;
3. bind the exact Product and DevOps evidence lane;
4. name the highest proven ceiling;
5. preserve local, production, legal, and Human residuals;
6. identify the owning open issue for every missing edge.

Read `docs/audits/M8_REAL_PROBLEM_CLOSURE_AUDIT.md`.

```text
SOURCE_LINK       != COMPLETION_RECEIPT
ARTICLE_SUMMARY   != IMPLEMENTATION
PR_MERGED         != PHYSICAL_RUNTIME
ISSUE_CLOSED      != CAPABILITY_PASS
GOOGLE_PROJECTION != EVIDENCE_AUTHORITY
```

Mutable or high-risk public claims require fresh verification. Protected source bodies must be linked or paraphrased unless redistribution is explicitly admitted.

## Product → DevOps contract

Product owns:

```text
source and claim identity
job requirement and competency gap
Product/System Design and ADR
success metrics / rollout / migration / build-vs-buy
bounded interview narrative
```

DevOps owns:

```text
implementation
CI and exact artifacts
ML lifecycle and policy gates
failure/recovery drills
runtime runner contracts
Local Handoff and physical receipts
```

Product may admit only the exact DevOps evidence ceiling. Cross-repository evidence is a typed process/evidence edge, not Git ancestry.

## Molecular Git Town laws

Follow `git-town-stacked-pr-worker`:

```text
PATH-DISJOINT + no unmerged consumption → SIBLING
consumes parent unmerged bytes/contract → TRUE_CHILD
smallest behavior + tests + evidence    → TERMINAL_LEAF
shared multi-input closure              → CONVERGENCE
physical/local prerequisite             → PROCESS_DEPENDENCY / LOCAL_HANDOFF
```

Observed Product route:

```text
PR #5 bootstrap
└─ PR #8 Full Manager MVP contract
   └─ PR #11 public disclosure alignment
      └─ PR #12 M4 routing
           ↑ PR #9 evidence audit                     exact side input
           ↑ DevOps PR #44 reviewer                  external evidence

Merged follow-up:
PR #13 exact TPM evidence
PR #15/#17 M8 audit/closure preparation
M8 durable routing/audit convergence                current Product owner
```

Observed DevOps route:

```text
PR #68 M1–M7 backbone
├─ PR #37 Demo Console
├─ PR #38 Policy / Security / License
├─ PR #39 ML / LLMOps
├─ PR #40 Supply Chain / Fault
├─ PR #69 advanced runner contracts
└─ PR #70 M8 main integration / Local Handoff
```

Do not invent a multi-parent Git relation for typed side inputs.

## Canonical Local Handoff law

The current queue is owned by DevOps and bound to one exact execution subject:

```text
commit   e7b4e23799a3579572598ebd5864a80831d49db4
tree     0b72b9f09f73d3829db2f138d457a5691641bf79
rollback bb940bf7d5a3b1f605b79e9fb8f33c463a8ee5a7
```

Current order:

```text
M8-LOCAL-REVIEWER-001          ACTIVE
M8-LIVE-KIND-002               BLOCKED_BY_PREDECESSOR
M8-COMPILE-ADVANCED-QUEUE-003  BLOCKED_BY_PREDECESSOR
```

After an admitted compile receipt, the advanced queue is sequential:

```text
Argo controllers
→ local model
→ synthetic 1,000 VU
→ registry-stored image signing
```

No Agent may:

- execute a blocked item;
- advance the queue without trusted receipt review;
- accept a fixture as a live predecessor;
- claim cleanup when cleanup is absent or failed;
- infer production evidence from any local receipt.

## Issue closure law

Close an issue only when **its own bounded acceptance criteria** are met. Keep it open when a named completion edge still needs physical, production, legal, or Human evidence.

Current Product classification:

```text
CLOSED bounded contracts:
  #1 #2 #3 #6 #7 #10 #12 #14

CLOSE AFTER durable M8 audit merge:
  #16

KEEP OPEN final convergence:
  #4
```

Product #4 remains open until both categories are separately handled:

```text
Physical portfolio evidence
  local reviewer / kind / Argo / model / 1,000 VU / signing

Human-admitted evidence
  employment dates and scope
  formal TPM/program tenure
  direct-report history
  real users/adoption
  real production incidents
```

## Evidence states and ladder

```text
PASS
FAIL
ABSENT
NOT_IMPLEMENTED
NOT_EXERCISED
SKIPPED_BY_POLICY
OUTSIDE_REPOSITORY_PROOF
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

Lower evidence never self-promotes.

Forbidden promotions:

```text
DRILL_COMPLETE        → PRODUCTION_INCIDENT_HISTORY
1000_VU_PASS          → 1000_REAL_USERS
PUBLIC_REPO           → PRODUCTION_ADOPTION
LOCAL_K8S_PASS        → PRODUCTION_INFRA_EXPERIENCE
ARGO_CONTROLLER_PASS  → APPLICATION_RECONCILIATION_PASS
LOCAL_MODEL_PASS      → PRODUCTION_LLM_TRAFFIC
LOCAL_SIGNING_PASS    → PRODUCTION_KEY_CUSTODY
PORTFOLIO_IMPLEMENTED → FORMAL_TPM_TENURE
MANAGEMENT_DOCS       → PEOPLE_MANAGEMENT_TENURE
LICENSE_METADATA      → BLANKET_LEGAL_CLEARANCE
```

## Google / GitHub boundary

GitHub is canonical for sources, requirements, decisions, issues, PRs, Stack state, and evidence subjects.

Google URLs in `registry/external-links.yaml` are non-authoritative projections. A URL proves reachability only. Every projected M8 claim must point to an exact GitHub subject and retain all `NOT_EXERCISED`, `DRILL`, `OUTSIDE_REPOSITORY_PROOF`, and `HUMAN_ADMIT_REQUIRED` states.

## Stop / Human boundaries

Stop on stale or wrong subject, overlapping lease, missing predecessor receipt, semantic conflict, public-disclosure risk, unbounded side effect, invalid evidence, unavailable physical runtime, unresolved redistribution/license boundary, failed cleanup, or Human-owned transition.

Human/trusted-owner operations include:

```text
semantic conflict resolution
force-push
merge / release
repository visibility / permissions
production promotion / rollback admission
credential/provider enrollment
queue advancement after receipt review
claims of real users / production / incidents
claims of employment / formal TPM / people-management tenure
```
