# Public Disclosure Checklist

Use this checklist before any P7 export, recruiter-facing publication, Google projection, or public evidence update from `Product-Manager-Notes`.

## Observed authority boundary

- GitHub repository metadata is the source of truth for repository visibility. This repository is currently public.
- This checklist does **not** authorize changing repository visibility, permissions, branch protection, merge state, release state, or production authority.
- Public reachability does not raise an evidence lane or convert `ABSENT`, `NOT_IMPLEMENTED`, `NOT_EXERCISED`, `DRILL`, `SIMULATION`, or `HUMAN_ADMIT_REQUIRED` into `PASS`.

## Must be absent from public commits

- credentials, access tokens, API keys, cookies, private keys, passwords, signed URLs, session material;
- customer/user personally identifiable information or private business data;
- employer/client confidential code, architecture, logs, datasets, contracts, incident material, screenshots, or internal URLs;
- proprietary source documents, private PDFs, private prompts, private model artifacts, paid-content bodies, or restricted-license material unless redistribution is explicitly admitted;
- unredacted local paths, account identifiers, environment dumps, provider secrets, or private repository content copied for convenience;
- claims of employment tenure, people-management tenure, production outages, real adoption, or production infrastructure experience that are not supported by admissible Human/production evidence.

## Required checks before publication

1. Bind the exact source/branch/commit/PR/issue being exported.
2. Confirm every visible claim points to an exact evidence subject or an explicit missing state.
3. Re-run secret/private-data scan on all newly public artifacts.
4. Check that external Article/PDF/Repo excerpts are source-anchored and redistribution-safe; otherwise link or paraphrase instead of copying protected content.
5. Verify that load-test numbers are labeled synthetic and name workload/environment/duration/percentiles.
6. Verify that failure cases are labeled `DRILL`/`SIMULATION` unless they are admissible real production events.
7. Verify local/CI Kubernetes, MLflow, llama.cpp, canary, security, or supply-chain evidence is not described as production tenure.
8. Verify top-level dependency licenses are not represented as recursive legal/commercial clearance.
9. Verify Google Doc/Sheet mirrors contain only public-safe information and do not become evidence authorities.
10. Require Human Admit for merge/release/visibility/permission changes and for real-experience claims.

## Stop conditions

Stop publication and reopen the evidence gap if any source is private/confidential, any evidence identity is stale or ambiguous, any secret/private-data detector fires, any license/redistribution right is unresolved, or any prose widens the exact evidence ceiling.
