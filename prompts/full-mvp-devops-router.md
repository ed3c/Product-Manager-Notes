# Full MVP DevOps Router

Use this after Product P4 has frozen the Full Manager MVP task graph. Product owns requirements and evidence requests; implementation prompts remain canonical in `ed3c/DevOps-Manager-Notes/prompts/`.

## Dispatch map

```text
DevOps #11  prompts/issue-11-technology-contract.md
DevOps #1   prompts/issue-1-invariant-evidence-audit.md
DevOps #2   prompts/issue-2-core-platform.md
DevOps #3   prompts/issue-3-observability-load.md
DevOps #4   prompts/issue-4-policy-security.md
DevOps #7   prompts/issue-7-llmops-progressive-delivery.md
DevOps #8   prompts/issue-8-demo-console.md
DevOps #10  prompts/issue-10-supply-chain-fault.md
DevOps #5   prompts/issue-5-failure-recovery.md
DevOps #9   prompts/issue-9-final-convergence.md
local       prompts/local-handoff-compiler.md
```

Before opening a new ChatGPT/Agent session, bind exact repository, branch, commit, tree, issue, path/resource lease, start/completion dependencies, consumed/produced artifacts, evidence ceiling and Human-owned operations. Do not rely on conversation memory.

## Parallel fan-out

#3/#4/#7/#8/#10 may run in separate sessions only after #2 freezes and publishes the shared typed service/artifact/evidence contracts. If any lane consumes another lane's unmerged bytes, Tech Lead must reclassify the actual Git ancestry.

## Return path

```text
DevOps exact receipt / PR / commit
→ Product registry/evidence.yaml
→ competency gap closure or reopen
→ Product #4 interview convergence
```

A DevOps issue/PR state is workflow evidence only. Product may not promote a capability until the exact named evidence lane is admitted.
