# SLTD Context Capsule Preflight

Use this prompt when the task needs current source context, lore retrieval discipline, POV knowledge limits, hidden canon control, long-range continuity, or source-status separation before another SLTD gate runs.

This prompt does not authorize new canon, autonomous lore updates, new project-management structures, new tracking databases, source writes, or prose from summary.

## Read first

```text
manifest.yml
rules/sltd_source_preflight.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_context_capsule_lore_retrieval_discipline.md
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md if structure/spine/scene packet is in scope
rules/sltd_tracking_logic_ledger_traceability_gate.md if state, knowledge, object, residue, thread, pass trace, or downstream risk is in scope
rules/sltd_character_voice_dialogue_relationship_location_gate.md if dialogue, relationship, silence, presence, or location staging is in scope
rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md if exact Vietnamese surface, pass integrity, Human Chapter Pass, or Publication Lock is in scope
```

## Source requirement

If the user asks for latest/current/Notion/current manuscript/lock/readiness/Human Chapter Pass/Publication Lock/packet lock/canon conflict, read current Notion source or use current source provided by the user.

If current source was not read or provided, return:

```text
SOURCE NOT READ / EVIDENCE MISSING
```

Then make only the safe narrower claim.

## Output

```text
CONTEXT CAPSULE PREFLIGHT
SCOPE:
REQUEST TYPE:
REVIEW MODE:
SOURCE READ:
SOURCE NOT READ:
SOURCE STATUS:
UNIT:
CURRENT STRUCTURAL SLOT:
ACTIVE CHARACTERS:
POV:
POV KNOWS:
POV DOES NOT KNOW:
READER KNOWS / SUSPECTS:
HIDDEN CANON LOCK:
LOCATION STATE:
OBJECTS IN PLAY:
BODY / INJURY STATE:
RESOURCE / DEBT STATE:
RELATIONSHIP STATE:
RESIDUE / FOLKLORE STATE:
THREADS ACTIVE:
THREADS HELD BACK:
THREADS PAID / RETIRED:
CANON IN:
CANON OUT:
ALLOWED CONTEXT:
BLOCKED CONTEXT:
DOWNSTREAM RISK:
MISSING SOURCE:
CAPSULE VERDICT:
PROSE PERMISSION:
NEXT NODE:
```

Use only fields that matter. Keep the capsule compact.

## Rules

- Do not make current manuscript claims from chat memory.
- Do not use legacy Workdecks, raw drafts, older Google Docs, or summaries as current source unless the user explicitly names them as current.
- Do not replace exact source with chapter summary, memory, or plausible continuity.
- Do not leak hidden canon into POV prose or readiness verdict.
- Do not make readiness or lock decisions from capsule alone.
- Do not draft or rewrite prose from capsule alone when exact scene source is required.
- If source status is mixed, label each source as current, provided, pack rule, legacy, raw draft, or unknown.
- If a later gate needs source that has not been read, return NEXT_NODE_REQUIRED instead of guessing.
- End with NEXT NODE.

## Source gap output

```text
SOURCE GAP
SCOPE:
REQUEST:
CURRENT SOURCE NEEDED:
WHY NEEDED:
SAFE CLAIM NOW:
NEXT NODE:
```

## Notion update candidate output

Use this only when an existing Notion source node needs a compact trace. Do not write unless the user explicitly asks.

```text
NOTION UPDATE CANDIDATE
TARGET EXISTING SOURCE NODE:
MISSING CONTEXT:
PROPOSED CAPSULE TRACE:
WHY NEEDED:
CANON RISK:
VERIFY TARGET:
WRITE PERMISSION:
NEXT NODE:
```
