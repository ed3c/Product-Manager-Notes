# M4 Manager Demo Interview Story

Use this as a **bounded evidence narrative**, not as a claim of employment tenure or production incident history.

## 90-second version

I designed the demo around an internal AI platform rather than a chatbot because the target problem is lifecycle and platform reliability: version model/prompt/config state, evaluate before promotion, make deployment identity immutable, observe both infrastructure and business correctness, reject a bad canary, recover to a previous-good state, and preserve exact evidence of what actually ran.

The implementation is split into a Tech Lead DAG: Core platform, observability/load, policy/security, ML lifecycle, reviewer UI, and supply-chain/fault lanes. A failure/recovery convergence then executes seven bounded incident drills, each with detection, authority, mitigation, recovery, postmortem, corrective change, and same-failure re-test.

The final M4 reviewer convergence has two independent checks. One rebuilds and executes the bounded reviewer path with no paid model API. The other re-downloads the exact prior GitHub Actions artifacts and verifies their SHA-256 identities before assembling one public reviewer packet. This prevents a green README or UI from becoming evidence by assertion.

The important limitation is explicit: live Kubernetes/Argo/model runtime, 1,000-VU recovery, real users, production incidents and management tenure are not claimed. Those require Local Handoff or human employment evidence.

## System-design walkthrough

```text
Requirement
→ Invariant
→ Typed contract
→ Implementation lane
→ Oracle / negative control
→ Exact CI artifact
→ Failure
→ Recovery
→ Corrective change
→ Same-failure re-test
→ Reviewer convergence
→ Evidence ceiling
```

### Key decisions

| Decision | Why | Trade-off |
|---|---|---|
| Internal AI platform as demo domain | covers ML/LLMOps + platform/DevOps requirements in one system | broader than a CRUD demo, so evidence ceilings must be strict |
| deterministic CI before real model/runtime | lets reviewers reproduce the control path without GPU/API keys | real model/substrate remains separate `NOT_EXERCISED` evidence |
| business oracle separated from liveness | prevents `HTTP 200` from meaning product correctness | requires an explicit business metric and failure case |
| one Git parent per convergence | preserves real Stack ancestry | other dependencies must be exact side inputs, not fake parents |
| artifact re-download + SHA-256 check at M4 | proves prior evidence is still the exact artifact admitted | still bounded by Actions retention and does not prove production artifacts |
| Local Handoff after remote M4 | physical runtime cannot be manufactured by repo prose | local evidence remains pending until receipt returns |

## Failure story template

### Situation

A candidate change can pass an offline or infrastructure-level check but still fail the business oracle. The demo treats that as a first-class failure rather than letting CI green imply product correctness.

### Task

Design a release/evaluation process where failure can be detected, bounded, recovered and re-verified without overstating evidence.

### Action

```text
seed bad behavior
→ keep service liveness green
→ detect business oracle FAIL
→ activate incident authority
→ mitigate / return to previous-good behavior
→ record postmortem + corrective change
→ repeat the same failure case
→ require PASS on the corrected path
```

The failure/recovery lane also covers timeout, queue pressure, duplicate-side-effect, permission, observability and restore assumptions.

### Result

The exact M3/M4 GitHub Actions artifacts prove the deterministic drills and reviewer flow at their declared ceilings. They do not prove a historical production incident.

## Technical Product Manager questions

### How did you prioritize the MVP?

I prioritized the shortest path that demonstrates lifecycle decision quality rather than framework count: typed state, evaluation gate, immutable artifact identity, business correctness, observable failure, rollback/recovery, and exact evidence. Optional high-cost substrate features remain separate until they can produce a real receipt.

### How would you scale this to 1,000 internal users?

I would treat 1,000 users as an adoption/capacity requirement with separate evidence lanes: onboarding and active-user metrics for adoption, plus workload/latency/error/resource metrics for capacity. A Locust 1,000-VU result would prove synthetic load only; it cannot prove 1,000 real users.

### How would you manage model lifecycle?

```text
REGISTERED
→ EVALUATED
→ PROMOTION_ELIGIBLE | REJECTED
→ CANARY
→ PROMOTED | CANARY_REJECTED
→ ROLLED_BACK
```

The promotion decision needs model/prompt/config/dataset identity plus eval and business-oracle evidence. Offline PASS is insufficient if canary/business correctness fails.

### How did you handle build-vs-buy?

The MVP uses permissive/commercial-use-friendly components where practical and separates top-level license metadata from real transitive/legal clearance. Technologies are selected after the required state/failure/evidence contracts, not before them.

## DevOps Manager questions

### How do you know a release is safe?

I do not use one green signal. The demo requires a chain of independent evidence: tests, migration checks, immutable artifact identity, policy/security controls, business oracle, telemetry, fault/recovery evidence, and exact artifact receipts.

### What did FIRST_GREEN reveal?

FIRST_GREEN repeatedly found issues that a green job alone would hide: source-map/resource bloat, moving Action/image references, a shell heredoc defect, a false DAG dependency, and later a mismatch between a mutable PR head and the historical commit that produced an artifact. Each caused a corrective contract or CI change before the milestone was admitted.

### How do you approach incidents?

```text
trigger
→ detection
→ incident authority
→ mitigation
→ recovery
→ postmortem
→ corrective change
→ same-failure re-test
```

The public demo proves this process through DRILL/SIMULATION only. Production incident history must come from real employment evidence.

## Evidence links to cite in an interview

```text
DevOps PR #44 — reviewer convergence
DevOps PR #46 — M4 traceability/index
DevOps PR #45 — Local Handoff queue
Product registry/public-m4-manager-routing.json
Product docs/milestones/PUBLIC_MANAGER_M4_ROUTING.md
```

When discussing any result, state its evidence ceiling and unresolved residuals. Do not turn a demo result into a claim about real customers, production scale, formal management tenure or production incidents.
