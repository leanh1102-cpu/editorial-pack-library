# SLTD Multi-Constraint Instruction Check

Use this prompt before rewrite, author-aligned drafting, line patch, human surface polish, readiness, or packet review when multiple requirements must be preserved together.

This is a constraint ledger and drift check, not a prose draft and not a readiness pass.

## Read first

```text
manifest.yml
rules/sltd_source_preflight.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_context_capsule_lore_retrieval_discipline.md if current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope
rules/sltd_narrative_claim_verification_clipper_discipline.md if a constraint depends on status/canon/continuity evidence
rules/sltd_multi_constraint_instruction_ledger_suri_discipline.md
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md if scene/chapter function or prose permission is unclear
rules/sltd_tracking_logic_ledger_traceability_gate.md if state, object, debt, residue, thread, or downstream risk is affected
rules/sltd_character_voice_dialogue_relationship_location_gate.md if dialogue or character voice is in scope
rules/sltd_author_writing_sheet_claim_evidence_discipline.md if style constraints are in scope
rules/sltd_human_surface_polish_anti_synthetic_gate.md if surface polish is the next node
```

## Source requirement

Read current source or the user-provided current packet before granting rewrite/readiness permission.

If source is missing, return:

```text
CONSTRAINT_LEDGER_NEEDS_SOURCE
```

If exact prose/output needs checking, read exact surface or exact output excerpt.

## Output

```text
SLTD MULTI-CONSTRAINT INSTRUCTION LEDGER
SCOPE:
SOURCE USED:
SOURCE STATUS:
TASK TYPE:
PRIMARY USER INSTRUCTION:
CONSTRAINT LIST:
- ID:
  TYPE:
  MUST SATISFY:
  MUST NOT:
  CORRUPTED CONSTRAINT:
  PRIORITY:
  EVIDENCE / OUTPUT ANCHOR:
  STATUS: SATISFIED / PARTIAL / NOT SATISFIED / UNCERTAIN
CONSTRAINT CONFLICTS:
LOW-LEVEL DETAIL RISK:
DRAFT / REWRITE PERMISSION:
REPAIR TARGET:
NEXT NODE:
```

## Rules

- No rewrite or author-aligned draft without named constraints.
- Every high-risk constraint needs a corrupted twin.
- If constraints conflict, stop before drafting.
- If source/current status is missing, status is UNCERTAIN.
- If exact output anchor is missing, status is UNCERTAIN.
- Do not use AI constraint satisfaction as Human Chapter Pass.
- Do not call readiness or Publication Lock from this prompt.
- Do not repair by smoothing prose over a broken constraint.

## Minimal ledger

For small line work:

```text
PRIMARY INSTRUCTION:
CONSTRAINTS:
HIGH-RISK DRIFT:
CORRUPTED CONSTRAINT:
PERMISSION:
NEXT NODE:
```

## Source gap output

```text
MULTI-CONSTRAINT SOURCE GAP
SCOPE:
REQUEST:
SOURCE NEEDED:
CONSTRAINTS THAT CANNOT BE VERIFIED:
SAFE CLAIM NOW:
NEXT NODE:
```