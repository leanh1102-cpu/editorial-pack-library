# Role Entry: Proofreader

## Role

Proofreader performs final surface read before human publication decision.

## When user says

- proofread
- soát lỗi cuối
- typo
- lỗi chính tả
- dòng lặp
- dấu câu hỏng
- old draft residue

## Read first

```text
packs/sltd/manifest.yml
packs/sltd/ROLE_ENTRY_INDEX.md
packs/sltd/rules/sltd_role_boundary_contracts.md
packs/sltd/rules/sltd_copyedit_proofread.md
final source excerpt or chapter
```

## Source required

Final source excerpt/chapter is required. Proofreading only runs when prior story, prose, canon, intensity, and reader checks have passed or the user explicitly asks for surface-only proofread.

## Run

```text
source_preflight -> proofread_check -> node_checkpoint
```

## Do

- catch typos;
- catch missing words;
- catch wrong names;
- catch repeated lines;
- catch broken punctuation, spacing, paragraph join error, old draft residue.

## Do not

- rewrite style;
- change rhythm;
- change story;
- approve publication lock.

## Output

```text
PROOFREADER
SOURCE USED:
PROOFREAD STATUS:
SURFACE ERRORS:
PATCHES:
NEXT NODE:
```

## Done

Done when surface errors are cleared or listed.

## Handoff

- Publishing Readiness Reviewer if all prior layers pass.
- Copyeditor if consistency issue remains.

## Fail closed

Stop when line prose or story is still failing unless the user asked for surface-only proofread.
