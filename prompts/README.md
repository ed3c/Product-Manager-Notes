# Eight-Stage System Prompt Router

These prompts let separate ChatGPT sessions work on one Manager Evidence Graph without relying on conversational memory.

## Dispatch rule

Before opening a new session, replace the subject block in the selected stage prompt with exact current values:

```yaml
repository: owner/name
branch: exact-branch
commit: 40-char-sha
tree: 40-char-sha
issue: owner/name#N
base_or_parent: exact branch/commit/PR
allowed_paths: [...]
read_only_paths: [...]
forbidden_paths: [...]
```

Never use a branch name or issue state as correctness evidence.

## Stage order

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

Start-readiness is not completion-readiness. P1 source workers may run in parallel; P2 TPM/DevOps design lanes may draft in parallel; P3 candidate families may be evaluated in parallel; P5 path-disjoint implementation leaves may run in parallel. P7 has exactly one convergence owner.

## Required handoff envelope

Every stage returns or commits a handoff record with:

```text
exact subject
state_in / state_out
consumed artifacts
produced artifacts
invariants / negative controls
start DAG edges
completion DAG edges
path/resource leases
evidence state / evidence ceiling
Shadow Architect deltas + L0-L3 intervention
open unknowns / blockers
local runtime boundary
next prompt/stage
Human-owned operations
```

## Shared laws

All stage prompts enforce:

- `MODE=MONITOR` unless a high-risk transition explicitly requires PRECHECK.
- Source material is intent/candidate architecture, not proven truth.
- Contracts before Workers; real dependency edges only; disjoint mutation leases for parallel Workers.
- Worker/LLM/CI/issue self-report is candidate evidence.
- `ABSENT`, `NOT_IMPLEMENTED`, `NOT_EXERCISED`, and `SKIPPED_BY_POLICY` never become `PASS` through prose.
- FIRST_GREEN triggers Shadow review and does not mean done.
- Google Docs/Sheets mirror canonical GitHub state and have zero evidence-promotion authority.
- Synthetic cases remain `DRILL`/`SIMULATION`; virtual load is not adoption; local runtime is not production tenure.
- Merge, force push, semantic conflict resolution, release, promotion, visibility, permission widening, production rollback admission, and real-experience claims remain Human/trusted-owner boundaries.

## Prompt files

- `stage-0-subject-authority.md` — freeze exact subject, authority, objective and evidence ceiling.
- `stage-1-source-evidence.md` — ingest articles/PDFs/repos/job/technology sources and build claim/evidence/gap registries.
- `stage-2-problem-closure-system-design.md` — prove the architecture addresses the real problem; build state machines, invariants and failure matrix.
- `stage-3-technology-adr.md` — select commercially usable candidates only after constraints; record license/ops/lock-in trade-offs.
- `stage-4-tech-lead-stack-plan.md` — compile task DAG, leases, molecular Git Town topology and Worker packets.
- `stage-5-parallel-implementation.md` — execute only admitted leaves, verify independently, preserve exact-head receipts.
- `stage-6-shadow-runtime-failure.md` — run FIRST_GREEN review, failure/load/policy probes, rollback/recovery and repeated verification.
- `stage-7-convergence-handoff.md` — update indexes, Google projections, public-safe narrative and Local Handoff/Human Admit residuals.
