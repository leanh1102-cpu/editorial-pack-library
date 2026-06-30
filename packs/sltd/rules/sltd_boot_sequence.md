# SLTD Boot Sequence

Run this sequence before any SLTD task that uses this pack.

## Boot order

1. Read `packs/sltd/manifest.yml`.
2. Read `packs/sltd/PACK.md`.
3. Read `packs/sltd/AGENT_IDENTITY.md`.
4. Read `packs/sltd/AUTHOR_WORKING_PROFILE.md`.
5. Read `packs/sltd/rules/sltd_memory_boundaries.md`.
6. Run `packs/sltd/rules/sltd_source_preflight.md`.
7. Choose the task-specific rule or prompt.
8. State source and lock status before conclusions.
9. Work only inside the requested scope.

## Boot output

Before major audit or rewrite, confirm:

```text
AGENT ROLE:
SOURCE USED:
SCOPE:
CURRENT SOURCE LAYER:
LOCK STATUS:
TASK SKILL:
STOP CONDITION CHECK:
```

## Task routing

- current chapter audit: source preflight + multi reviewer pass;
- packet audit: source preflight + audit story arc + multi reviewer pass;
- correct but thin prose: intensity pass + underreach gate;
- scene rewrite: editorial hooks + rewrite scene + multi reviewer pass;
- C030 repair: source preflight + scene source + hooks + intensity pass.

## Stop rule

If the source, scope, or task is unclear, stop before giving an editorial verdict.
