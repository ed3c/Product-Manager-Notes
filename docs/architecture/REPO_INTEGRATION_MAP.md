# Repository Integration Map

The Manager Evidence Graph uses existing repositories by **trigger**, not by default importing every project into one monolith.

## Mandatory planes

| Repository | Role | Trigger | Authority |
|---|---|---|---|
| `ed3c/Product-Manager-Notes` | private Manager routing/control plane | always | source IDs, requirements, gaps, stage prompts, Stack routing, Google links, interview closure |
| `ed3c/DevOps-Manager-Notes` | public executable evidence plane | any DevOps/platform/runtime proof | public implementation, tests, failure/recovery, receipts |
| `ed3c/skills-shared` | reusable method plane | Tech Lead / Shadow / Git Town / shared verification procedure | portable method only; never consumer issue/branch/runtime state |

## Trigger-selected support repositories

| Repository | Use when | Do not use it to claim |
|---|---|---|
| `ed3c/truth-verify-loop` | a mutable/high-risk external technical claim needs fresh source capture and explicit evidence closure | that search/model output itself is truth |
| `ed3c/openwiki-source-anchoring` | generated documentation/source claims need exact path/quote anchoring and reproducible source verification | lexical anchor validity equals semantic correctness |
| `ed3c/runtime-env` | a local/provider runtime needs a secret-free capability/profile/workload/policy contract | declaration/profile presence equals live runtime execution |
| `ed3c/skill-resume-site` | P7 has public-safe evidence ready for portfolio export | private/unverified metrics, adoption, uptime, customer or production claims |

Optional note stores such as `ai-content-notes` or `ai-product-notes` may provide source candidates, but every imported item must receive a stable `registry/sources.yaml` ID and re-enter the same claim/evidence pipeline. They do not become a second canonical Manager state store.

## Routing rule

```text
source candidate
→ Product source ID
→ claim classification
→ requirement / gap
→ trigger-selected method/support repo
→ exact evidence/receipt
→ Product evidence graph
→ optional public export
```

Cross-repository references must bind exact GitHub subjects when used as evidence. Mutable branch URLs are navigation unless a stage explicitly re-verifies and pins the revision.

## Why Product-Manager-Notes is the center

The center must own **management state**, not runtime state. It therefore owns:

```text
what problem is being solved
which source/requirement created it
what is missing
which stage/prompt/issue owns the next action
which DevOps evidence can close the claim
which evidence ceiling applies
which Google/public projection may summarize it
```

`DevOps-Manager-Notes` remains independently reviewable and public-safe; it does not need access to Product private narrative state.

## Authority boundary

No support repository may widen authority. A module or source may add evidence, but it cannot infer merge, release, production acceptance, visibility changes, credentials, real users, real incidents, or management tenure.
