# SLTD Source Surface Check

Use this prompt before any line edit, line surgery, rewrite, copyedit, proofread, readiness verdict, or exact OLD/NEW patch when source surface may be missing or compressed.

This prompt prevents editing from summary, digest, memory, or inferred source.

## Read first

```text
packs/sltd/manifest.yml
packs/sltd/rules/sltd_source_preflight.md
packs/sltd/rules/sltd_decision_safety.md
packs/sltd/rules/sltd_source_fidelity_anti_compression.md
packs/sltd/rules/sltd_evidence_discipline.md
packs/sltd/rules/sltd_context_window_strategy.md
user request
```

## Output

```text
SOURCE SURFACE CHECK
REQUEST:
SCOPE:
TASK LEVEL: map / packet / chapter / scene / excerpt / line
SOURCE USED:
SOURCE TYPE:
SURFACE AVAILABLE: YES / NO / PARTIAL
COMPRESSION RISK: LOW / MEDIUM / HIGH / BLOCKING
ALLOWED ACTION:
FORBIDDEN ACTION:
SAFE DOWNGRADE:
NEEDED SOURCE:
NEXT NODE:
```

## Rules

- If the task is line-level, exact source text is required.
- If the task is rewrite, source scene or current scene packet is required.
- If the task is readiness or lock, current Notion source is required.
- If only digest or chat memory is available, do not patch prose.
- If scope is packet or arc, do not line edit unless exact excerpts are opened.
- If exact OLD text is missing, do not produce OLD/NEW patch.
- Label every digest as `DERIVED DIGEST — NOT SOURCE TEXT`.
- End with NEXT NODE or STOP.

## Safe downgrade examples

```text
LINE TASK OVER PACKET SCOPE
SAFE DOWNGRADE: packet risk scan only
NEEDED SOURCE: exact excerpt or scene text
```

```text
REWRITE WITHOUT SCENE SOURCE
SAFE DOWNGRADE: rewrite plan only
NEEDED SOURCE: current scene packet or exact source scene
```

```text
READINESS WITHOUT CURRENT NOTION
SAFE DOWNGRADE: no current verdict
NEEDED SOURCE: current Chapter Index / Chapter Review / Publication Lock fields
```
