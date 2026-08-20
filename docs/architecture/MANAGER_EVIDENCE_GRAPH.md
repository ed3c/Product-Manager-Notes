# Manager Evidence Graph

## Repository roles

```text
Product-Manager-Notes (private)
  job requirements / competency gaps / product decisions / interview narratives
        │
        │ evidence request + public-safe claim contract
        ▼
DevOps-Manager-Notes (public)
  executable platform / CI-CD / Kubernetes / SLO / failure / recovery evidence
        │
        │ exact public evidence reference
        └──────────────────────────────► Product-Manager-Notes
```

There is no mutable shared database between the repositories. Cross-repository edges are exact GitHub subjects (issue, PR, commit, file, evidence receipt) and must name their evidence lane.

The private repository may consume public evidence. The public repository must remain independently understandable and must never require private repository access.

## Canonical flow

```text
Job / Article / PDF / Repo
→ source ID
→ requirement / claim classification
→ competency gap
→ product/system-design case
→ decision + trade-off
→ implementation evidence request
→ DevOps/public executable evidence
→ failure / negative control
→ corrective change
→ verification receipt
→ evidence ceiling review
→ interview narrative
```

Google Docs and Google Sheets are optional edges:

```text
GitHub canonical state
   ├──► Google Doc: long-form narrative
   └──► Google Sheet: human dashboard mirror

Google URL
   └──X──► cannot promote evidence state
```

## Product Manager issue DAG

Two edge classes are kept distinct.

### Start-readiness

```text
bootstrap contract
├── #1 evidence audit
├── #2 product/system-design drafting may begin with claims marked unverified
├── #3 failure-drill drafting may begin as explicit simulation
└── #4 dashboard schema may be designed with null URLs
```

### Completion-readiness

```text
bootstrap contract
→ #1 audited evidence
→ #2 flagship product/system-design case
→ #3 decision/failure/postmortem library
→ #4 external dashboard + interview-ready graph
```

A task being startable does not make it completable. Completion requires its own exact evidence.

## Shadow Architect checkpoints

```text
SOURCE_BOUND
REQUIREMENT_CLASSIFIED
ARCHITECTURE_CHOICE
FIRST_CASE_COMPLETE
IMPLEMENTATION_EVIDENCE_LINKED
FAILURE_DRILL_COMPLETE
FIRST_GREEN
BEFORE_INTERVIEW_EXPORT
```

At each checkpoint compare intended versus observed state and record any new assumption, evidence promotion, authority change, hidden lifecycle, or public/private boundary change.

## Closure invariant

For each interview claim `C`:

```text
C.source != null
C.requirement != null
C.evidence_subject != null OR C.state in {ABSENT, NOT_IMPLEMENTED, NOT_EXERCISED}
C.evidence_ceiling is explicit
C.simulation != production
C.virtual_load != real_adoption
```

The graph is closed only when missing proof stays visible rather than being filled by narrative.
