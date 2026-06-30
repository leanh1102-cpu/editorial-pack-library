# SLTD Retrieval Budget

This rule prevents context overload.

## Budget levels

### Small task

Use up to:

- 1 source page;
- 1 to 3 rule files;
- 1 prompt;
- 1 node checkpoint.

### Medium task

Use up to:

- 3 source pages;
- 3 to 6 rule files;
- 2 prompts;
- 1 context brief;
- 1 result report.

### Large task

Use:

- source preflight;
- mindmap review;
- context brief;
- staged node traversal;
- separate result reports by node.

Do not attempt one-pass full rewrite or full audit if the source exceeds the active context window.

## Retrieval order

Retrieve in this order:

1. current user instruction;
2. manifest and boot task;
3. source preflight;
4. current Notion source;
5. task-specific rules;
6. node ledger or checkpoint;
7. legacy sources only if needed.

## Drop order

When context is crowded, drop first:

1. old discussion;
2. legacy source;
3. examples not used by the current task;
4. non-active roles;
5. broad packet summary.

Do not drop:

- current source;
- scope;
- canon constraints;
- lock status;
- blockers;
- user instruction.
