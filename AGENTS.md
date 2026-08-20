# AGENTS.md

## Purpose

This public repository is the canonical **Manager orchestration and evidence-routing control plane** for public-safe Product/DevOps Manager evidence. It owns source/requirement/gap identity, Product/System Design contracts, stage prompts, cross-repository task routing, Google projection links and interview closure.

`ed3c/DevOps-Manager-Notes` owns executable public evidence. `ed3c/skills-shared` owns reusable Tech Lead, Shadow Architect and Git Town procedures.

GitHub repository metadata is the visibility authority. Visibility changes remain Human-owned. If observed visibility disagrees with docs, record `AUTHORITY_DELTA` / `EVIDENCE_DELTA` and repair the documentation contract; never change visibility automatically.

## Mandatory read order

1. `README.md`
2. `docs/PUBLIC_DISCLOSURE_CHECKLIST.md`
3. `docs/INDEX.md`
4. `docs/architecture/MANAGER_EVIDENCE_GRAPH.md`
5. `docs/architecture/REPO_INTEGRATION_MAP.md`
6. `docs/case-studies/INTERNAL_AI_PLATFORM_MVP_DEMO.md`
7. `docs/milestones/PUBLIC_MANAGER_M4_ROUTING.md`
8. `roles/technical-product-manager/job-contract.yaml`
9. `roles/technical-product-manager/competency-matrix.yaml`
10. `roles/technical-product-manager/interviews/M4_MANAGER_DEMO_STORY.md`
11. `registry/sources.yaml`
12. `registry/claims.yaml`
13. `registry/evidence.yaml`
14. `registry/gaps.yaml`
15. `registry/external-links.yaml`
16. `registry/stack-plan.yaml`
17. `registry/public-m4-manager-routing.json`
18. current `prompts/stage-*.md` or `prompts/full-mvp-devops-router.md`
19. exact issue / PR / commit / Actions run / artifact / source subject

When a reusable method is triggered, read the canonical `skills-shared` implementation rather than copying local variants:

```text
skills/agentic-tech-lead-orchestration/
skills/spatial-loop-systems-engineering/
skills/git-town-stacked-pr-worker/
```

Trigger-selected support repositories:

```text
truth-verify-loop          mutable/high-risk external claim verification
openwiki-source-anchoring  exact source/path/quote verification
runtime-env                secret-free runtime/profile/workload contract
skill-resume-site          public portfolio projection after evidence admission
```

No support repository becomes a second Manager-state authority.

## Public disclosure law

Before writing or exporting public material, apply `docs/PUBLIC_DISCLOSURE_CHECKLIST.md`.

Public tracked content must not contain:

```text
credentials / private keys / tokens
customer or user private data
employer/client confidential material
private source document bodies
sensitive prompts from private work
restricted redistribution material
unredacted runtime identity
claims above an admitted evidence ceiling
```

Prefer exact public subjects and bounded paraphrases over copying source bodies. Public reachability does not promote evidence.

## Operating mode

Default `MODE=MONITOR`.

Builder may proceed on reversible notes, architecture, task contracts and bounded repository work. Shadow Architect separately monitors:

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

L3 includes unsafe/irreversible transitions, secret/private exposure, visibility/permission mutation, overlapping mutation authority, semantic conflict, evidence laundering and false production/adoption/tenure claims.

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

Start-readiness and completion-readiness are distinct. A stage may start with bounded unknowns but cannot close before exact completion receipts exist.

Every handoff records:

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

## Current Product checkpoint

```text
PR #9   existing TPM evidence audit         COMPLETE_STAGE
PR #11  public disclosure alignment         PASS_AS_POLICY
PR #12  public Manager M4 routing            PASS_BOUNDED_AS_ROUTING
issue #4 final interview/evidence closure    OPEN
```

PR #12 is a true child of PR #11 because it consumes its public-disclosure contract. Product PR #9 remains a separate exact side input; do not invent a Git multi-parent relationship.

## DevOps M4 executable route

The current exact public executable evidence subject is:

```text
repository      ed3c/DevOps-Manager-Notes
issue           #9
pull request    #44
commit          55d18cdc556ca5d66c67406318ae25196c077fd2
tree            a4ad37d9baf73a5239f79c516c67b0182420336a
milestone       PUBLIC_REMOTE_REVIEWER_CONVERGENCE_FIRST_GREEN
status          PASS_BOUNDED
```

Admitted remote evidence:

```text
Full MVP reviewer convergence
  run       32256802856
  artifact  9366615717
  digest    sha256:e652cdf3ccb8de7a8655f9148bc6471a29bcaeaef2d55f6255bca2cb2b1e19d3
  ceiling   GITHUB_HOSTED_REMOTE_REVIEWER_CONVERGENCE_ONLY

Full MVP public reviewer convergence
  run       32256802554
  artifact  9366596481
  digest    sha256:696f56be2fb637e386941eb313caa7c9448900ad0bad88b3a96119b95315596c
  ceiling   GITHUB_HOSTED_ARTIFACT_REDOWNLOAD_AND_REVIEWER_BUNDLE_ONLY
```

The second lane independently re-downloads the six bound M2/M3 Actions artifacts and verifies their archive SHA-256 identities before reviewer admission.

## Local Handoff boundary

DevOps PR #45 owns the current Local Handoff child.

```text
head            a697c74a11d5d6492eaddb44aabd1a331899ee32
contract run    32257928774 PASS
active item     M4-LOCAL-REVIEWER-001
command         bash scripts/demo/run_reviewer_demo.sh evidence/local-reviewer
expected receipt evidence/local-reviewer/reviewer-demo-receipt.json
```

The GitHub workflow proves queue shape only. Local execution is still `NOT_EXERCISED`. The next live-substrate item remains `BLOCKED_UNRESOLVED` and has no executable command.

Product may link a queue or returned receipt but must never infer local/runtime PASS from queue existence.

## Evidence subject law

A mutable PR head and an artifact evidence head are separate subjects. Product must consume the exact artifact-producing commit/digest recorded by the DevOps evidence registry, not whichever commit happens to be current later.

Do not perform:

```text
CURRENT_PR_HEAD → HISTORICAL_ARTIFACT_EVIDENCE
README_TEXT     → EXECUTION_PASS
ISSUE_CLOSED    → RUNTIME_PASS
QUEUE_EXISTS    → LOCAL_EXECUTION_PASS
```

## Tech Lead laws

- Freeze exact subject, objective, non-goals, invariants, dependencies, acceptance criteria, budgets, evidence lane and Human authority before fan-out.
- A dependency exists only for real artifact/state consumption or an admitted receipt.
- Keep task-DAG dependencies separate from Git ancestry.
- Parallel writers require disjoint path/resource leases.
- Worker/LLM/issue/branch/CI self-report is candidate evidence only.
- Every material claim binds an exact public source/evidence subject or remains missing.
- `ABSENT`, `NOT_IMPLEMENTED`, `NOT_EXERCISED`, `SKIPPED_BY_POLICY` and `HUMAN_ADMIT_REQUIRED` never become PASS through prose.
- One convergence owner updates shared indexes after prerequisites stabilize.
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

Observed Product-side relation:

```text
PR #5 bootstrap
└─ PR #8 Full Manager MVP contract
   └─ PR #11 public disclosure alignment
      └─ PR #12 M4 public Manager routing
           ↑ PR #9 evidence audit        EXACT SIDE INPUT
           ↑ DevOps PR #44 M4 evidence  EXTERNAL EVIDENCE
           ↑ DevOps PR #45 handoff       PROCESS DEPENDENCY
           ↓
         issue #4 final convergence      OPEN
```

Cross-repository evidence never becomes Git ancestry.

## Source classification

Classify significant claims exactly as:

```text
REQUIREMENT
DESIGN_PROPOSAL
ASSUMPTION
OBSERVATION
MEASURED_FACT
EXTERNAL_CLAIM
UNKNOWN
```

Article/PDF/README/diagram presence is not system truth. Mutable/high-risk claims require an admitted fresh verification route.

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

Lower evidence never self-promotes.

Forbidden Manager claim promotions:

```text
DRILL_COMPLETE        → PRODUCTION_INCIDENT_HISTORY
1000_VU_PASS          → 1000_REAL_USERS
PUBLIC_REPO           → PRODUCTION_ADOPTION
LOCAL_K8S_PASS        → PRODUCTION_INFRA_EXPERIENCE
PORTFOLIO_IMPLEMENTED → FORMAL_TPM_TENURE
MANAGEMENT_DOCS       → PEOPLE_MANAGEMENT_TENURE
```

## Interview closure

A technical capability becomes bounded-interview-ready only through:

```text
job requirement
→ real problem / product-system case
→ decision / trade-off
→ implementation or explicit simulation
→ failure / negative control
→ corrective action
→ repeated verification
→ exact evidence subject + ceiling
→ concise interview narrative
```

Use `roles/technical-product-manager/interviews/M4_MANAGER_DEMO_STORY.md` only with the exact M4 subjects in `registry/public-m4-manager-routing.json`.

Employment/tenure requirements remain `HUMAN_ADMIT_REQUIRED` until real user-provided evidence is admitted.

## Google / GitHub boundary

GitHub is canonical for requirements, source IDs, decisions, issues, PRs, Stack and evidence.

Google Sheet/Doc URLs in `registry/external-links.yaml` are non-authoritative human mirrors. A URL proves reachability only. Any M4 narrative projected there must point back to exact GitHub subjects and retain all `NOT_EXERCISED` / `DRILL` / Human-admit states.

## Stop / Human boundaries

Stop on stale subject, overlapping lease, missing predecessor receipt, semantic conflict, public-disclosure risk, unbounded side effect, invalid evidence, unavailable physical runtime, unresolved redistribution/license boundary or Human-owned transition.

Human/trusted-owner operations include:

```text
semantic conflict resolution
force push
merge / release
repository visibility / permission changes
production promotion / rollback admission
claims of real users / production / incidents
claims of people-management or formal TPM tenure
```
