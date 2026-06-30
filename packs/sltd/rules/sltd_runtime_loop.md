# SLTD Runtime Loop

This file connects boot, intake, routing, safety, execution, checkpoint, and report.

Order:

```text
boot_task
source_preflight
task_intake
sltd_task_router
sltd_decision_safety
task-specific prompt
node_checkpoint
result_report
```

Use the smallest route that fits the user request.

If source, scope, source layer, or route is unclear, stop before verdict.

If work suggests a Notion change, return a candidate only unless the user asks for write-back.
