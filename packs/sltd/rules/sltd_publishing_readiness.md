# SLTD Publishing Readiness

Use this rule to decide whether a chapter or packet may move toward human final review.

## Readiness is not publication

AI may say a chapter is ready for human final review.

AI must not say a chapter is publishable as final authority.

## Required checks

A chapter needs evidence for:

- source confirmed;
- chapter status checked in Notion;
- Human Chapter Pass status checked;
- Publication Lock status checked;
- canon guard clear;
- story function clear;
- reader pull present;
- underreach gate clear;
- Vietnamese prose pass clear;
- copyedit or proofread stage appropriate.

## Stop conditions

Stop if:

- current source is unclear;
- one source says locked and another says not ready;
- linked Scene Bank scenes are not ready;
- chapter pass labels are green but Human Chapter Pass is missing;
- Publication Lock is Not Ready;
- a packet depends on a failed chapter.

## Readiness labels

```text
NOT_READY
READY_FOR_REWRITE
READY_FOR_READER_PASS
READY_FOR_HUMAN_FINAL_REVIEW
LOCKED_BY_HUMAN
```

## Packet rule

A packet cannot be called locked if any chapter inside it is not ready.

If one chapter blocks the packet, name the blocker first.
