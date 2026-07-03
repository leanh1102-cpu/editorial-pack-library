# SLTD Pack Healthcheck

Use this rule to check SLTD pack health after version changes.

This is a manual agent check. It does not create management artifacts.

## Check manifest

Verify version, required files, allowed tasks, source priority, and fail-closed status.

## Check source fidelity

Verify source fidelity rule and source surface prompt exist and exact prose/status routes require source surface before patching or verdict.

## Check general + chapter feedback matrix

Verify:

- `rules/sltd_general_chapter_feedback_matrix_output_protocol.md` exists and is listed in manifest;
- `prompts/general_chapter_feedback_matrix_check.md` exists and is listed in manifest;
- `samples/general_chapter_feedback_matrix_calibration.md` exists and is listed in manifest;
- general_chapter_feedback_matrix_check is listed in allowed_tasks;
- matrix route ends with node checkpoint;
- matrix output requires source used, source status, general feedback, chapter feedback, evidence check, node ledger, and next node;
- the matrix does not authorize readiness claims, source writes, canon changes, or prose edits without relevant gates.

## Check tracking, logic ledger, and traceability

Verify tracking rule/prompt/sample exist, task is allowed, route ends with node checkpoint, and the gate blocks missing tracking surface, untracked state change, unclear knowledge state, missing object/residue/thread ledger, pass trace conflict, downstream dependency risk, and missing verify target.

## Check structural spine, Vietnamese surface, supernatural residue, and protagonist route

Verify these gates remain listed and routed when their scope is in play.

## Check route governance

Verify one primary route before secondary gates, evidence-backed secondary gates, explicit stop conditions, and no gate cascade.

## Check orphan risk

Mark a file as possible orphan when it exists but is not listed in manifest, is listed but cannot be fetched, defines a task with no route, duplicates another rule without reason, or is missing from its route.

## Output labels

```text
PACK_HEALTH_OK
PACK_HEALTH_WARN
PACK_HEALTH_FAIL
```
