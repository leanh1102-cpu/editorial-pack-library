# SLTD Chapter Readiness Check

Use this prompt to check whether a chapter can move to the next human review step.

## Read first

1. `prompts/boot_task.md`
2. `EDITORIAL_COMPETENCY_MAP.md`
3. `rules/sltd_source_preflight.md`
4. `rules/sltd_publishing_readiness.md`
5. current Notion Chapter Index page
6. linked Scene Bank scenes when needed

## Check

- source layer;
- chapter status;
- human pass status;
- publication lock status;
- scene readiness;
- canon risk;
- story function;
- reader pull;
- underreach risk;
- prose surface.

## Output

```text
SCOPE:
SOURCE USED:
PACK: sltd@1.6.0
READINESS LABEL:
BLOCKERS:
PASSING AREAS:
NEXT ACTION:
```

## Labels

```text
NOT_READY
READY_FOR_REWRITE
READY_FOR_READER_PASS
READY_FOR_HUMAN_REVIEW
LOCKED_BY_HUMAN
```

If any chapter in a packet is not ready, the packet is not locked.
