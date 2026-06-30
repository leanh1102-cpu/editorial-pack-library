# SLTD Context Brief

Use this prompt before a task that touches several source nodes or may exceed the context window.

## Read first

1. `prompts/boot_task.md`
2. `EDITORIAL_CONTEXT_PROTOCOL.md`
3. `rules/sltd_context_window_strategy.md`
4. `rules/sltd_retrieval_budget.md`
5. current user request

## Output

```text
CONTEXT BRIEF
SCOPE:
REQUEST TYPE:
SOURCE USED:
IN CONTEXT:
- ...
NOT IN CONTEXT:
- ...
ASSUMPTIONS:
- ...
RISK IF WRONG:
- ...
ACTIVE SKILLS:
- ...
BLOCKERS:
- ...
NEXT STEP:
- ...
```

## Rule

Do not proceed to verdict or rewrite if the brief shows a missing current source.

If the task is too large, split by node and say which node should be handled first.
