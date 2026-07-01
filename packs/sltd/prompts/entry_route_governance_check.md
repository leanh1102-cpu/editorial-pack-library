# SLTD Entry Route Governance Check

Use this prompt when a task risks route overload, gate cascade, checklist-first repair, or unclear primary route selection.

This prompt selects routes. It does not replace source preflight, source surface check, canon guard, readiness evidence, or user-requested modes.

## Read first

```text
manifest.yml
ENTRY_FAST_PATH.md
rules/sltd_task_router.md
rules/sltd_entry_route_governance_gate_budget_protocol.md
rules/sltd_source_preflight.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_decision_safety.md
rules/sltd_evidence_discipline.md
rules/sltd_role_boundary_contracts.md
```

## Output

```text
ENTRY ROUTE GOVERNANCE CHECK
SCOPE:
SOURCE USED:
REQUEST TYPE:
SOURCE REQUIREMENT:
PRIMARY BLOCKER:
PRIMARY ROUTE:
SECONDARY GATES ALLOWED:
SECONDARY GATES USED:
GATE BUDGET:
STOP CONDITION:
NO-CASCADE CHECK:
CHECKLIST-FIRST RISK:
FAILURE LABELS:
ROUTE DECISION:
NEXT NODE:
```

## Rules

- Choose one primary route.
- Add secondary gates only when the primary route exposes a real blocker.
- Do not run a gate because it is adjacent.
- Stop when source is missing, the requested answer is complete, the patch is complete, readiness is blocked, or the gate budget is spent.
- If current status, lock, readiness, or canon is requested, require current Notion or exact provided source before verdict.
- If three or more gates seem necessary, create a context brief or prioritized node ledger instead of running a cascade.
- Do not use this prompt to skip required source, canon, evidence, or user-requested review modes.
- End with NEXT NODE.
