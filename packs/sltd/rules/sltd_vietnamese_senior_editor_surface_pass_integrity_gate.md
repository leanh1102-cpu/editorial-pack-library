# SLTD Vietnamese Senior Editor Surface, Semantic Load & Pass Integrity Protocol

This gate prevents formal passes, checklist passes, or status updates from replacing a real Vietnamese human-surface read.

It is a senior-editor gate: it checks whether the prose breathes in Vietnamese, whether words carry the right semantic load, whether objects are still objects rather than visible functions, and whether pass metadata is trustworthy.

## Core rule

A chapter is not human-ready because it has an Anti-AI Pass, Chapter Reader Pass, Vietnamese Reader Pass, candidate-ready note, Polished status, or formal status update.

A chapter is human-ready only when the exact prose surface has been read at sentence and word level, and the pass metadata does not conflict with notes, Human Chapter Pass, or Publication Lock.

```text
VIETNAMESE_SURFACE = sentence flow, word choice, idiom, rhythm, dialogue breath, bodily action, object handling, and natural Vietnamese syntax
SEMANTIC_LOAD = how much conceptual/workflow meaning a word, object, or sentence is forced to carry
PASS_INTEGRITY = whether status properties, notes, pass labels, and lock state agree
READ_ALOUD_FRICTION = where a Vietnamese reader would stumble, feel stiffness, or hear schema instead of prose
OBJECT_FUNCTION_VISIBILITY = where a prop visibly behaves like an editorial label rather than a lived object
HUMAN_BREATH_SPACE = places where prose lets action, silence, or ordinary life breathe without every item proving a gate
```

Do not confuse cleaner prose with human prose.

Do not confuse anti-AI precheck with Human Chapter Pass.

Do not confuse candidate-ready with ready.

## Use when

- the user asks for senior Vietnamese editor review, human prose pass, từng chữ, đọc như người Việt, văn AI, AI hóa, or publication readiness;
- a chapter has repeated issues: clipped dialogue, static talk, sensory thinness, explanation-heavy phrasing, object-as-label, action/interiority labels, negative explanatory labels, or overdetermined object density;
- pass metadata conflicts with notes, Human Chapter Pass, Publication Lock, or user instruction;
- a chapter has formal status update without prose change;
- a chapter feels correct by gates but still sounds arranged, stiff, translated, or synthetic;
- exact prose excerpt is available and needs read-aloud / semantic load diagnosis before repair.

## Authority

This gate does not rewrite unless exact source excerpt is provided and the task asks for line edit or repair.

This gate does not override Human Chapter Pass or Publication Lock.

If pass status conflicts, report PASS_METADATA_CONFLICT and stop before readiness verdict.

If exact prose is missing, return SOURCE_SURFACE_REQUIRED.

## Output schema

```text
VIETNAMESE SENIOR EDITOR SURFACE / PASS INTEGRITY CHECK
SCOPE:
SOURCE USED:
SOURCE SURFACE:
CHAPTER / SCENE:
CURRENT STATUS:
PASS METADATA:
PASS CONFLICTS:
READ-ALOUD FRICTION:
WORD-CHOICE FRICTION:
SEMANTIC LOAD:
OBJECT FUNCTION VISIBILITY:
NEGATIVE EXPLANATION STACK:
DIALOGUE NATURALNESS:
BODY / ACTION BELIEVABILITY:
SENSORY THINNESS:
STATIC TALK:
VIETNAMESE RHYTHM:
OVERDENSITY:
HUMAN BREATH SPACE:
RECURRING SMELL FROM PRIOR CHAPTERS:
STATUS VERDICT:
SAFE REPAIR:
PROSE PERMISSION:
NEXT NODE:
```

## Pass integrity rule

Treat these as distinct states:

```text
ANTI_AI_PASS = no major synthetic-blocker detected; not a human prose pass
VIETNAMESE_READER_PASS = Vietnamese surface has been read; still not publication lock
HUMAN_CHAPTER_PASS = author/human accepts chapter-level read
PUBLICATION_LOCK = final lock for publication; requires all conflicts closed
CANDIDATE_READY = ready for human review; not a pass
FORMAL_STATUS_UPDATE = metadata update; not prose repair unless exact prose changed
```

A chapter must be marked blocked when:

```text
property says pass but notes say pass remains NO
candidate-ready is treated as ready
formal anti-AI update is treated as prose improvement
Human Chapter Pass is NO but readiness is claimed
Publication Lock is Not Ready but publication readiness is claimed
user instruction and Notion status conflict without reconciliation
```

## Vietnamese surface rule

A Vietnamese senior-editor pass must check at least:

```text
sentence read-aloud friction
word choice and register
idiom and natural syntax
whether action could physically happen as written
whether dialogue belongs to speaker age, power, work, and relation
whether object density makes prose read like a schema
whether negative explanation replaces positive action
whether interiority is named instead of carried by body/object/silence
whether every paragraph has a human breath, not only function
```

## Semantic load rule

A paragraph is overloaded when too many items are forced to prove pressure at once.

Watch especially for repeated clusters:

```text
sương / bùn / dây / vạch / dao / đá / tên / tiếng gọi / nước / thuốc / cân / than / giấy
```

These may all be valid SLTD objects. They fail when each appears with visible editorial purpose and no ordinary life between them.

## Failure labels

```text
VIETNAMESE_SURFACE_NOT_HUMAN
WORD_CHOICE_SEMANTIC_DRIFT
READ_ALOUD_FRICTION
OBJECT_FUNCTION_VISIBLE
NEGATIVE_EXPLANATION_STACK
CLIPPED_DIALOGUE
STATIC_TALK
SENSORY_THINNESS
ACTION_INTERIORITY_LABEL
OVERDETERMINED_OBJECT_DENSITY
HUMAN_BREATH_SPACE_MISSING
FORMAL_PASS_WITHOUT_PROSE_CHANGE
ANTI_AI_PASS_FALSE_CONFIDENCE
PASS_METADATA_CONFLICT
CANDIDATE_READY_MISREAD_AS_READY
PUBLICATION_LOCK_FALSE_POSITIVE
ARC_LABEL_DRIFT
RECURRING_SMELL_NOT_ESCALATED
STATUS_VERDICT_UNSUPPORTED
```

## Safe repair

Safe repair may:

- report exact friction points and recurring smells;
- downgrade a readiness claim when pass metadata conflicts;
- require line edit on exact excerpt;
- propose a Notion update candidate to reconcile pass metadata;
- mark a recurring smell as packet-level blocker;
- identify where the prose needs ordinary-life breath rather than more symbolic pressure.

Safe repair must not:

- rewrite from summary;
- mark a chapter ready from formal metadata alone;
- hide status conflict;
- add more objects to fix object-function prose;
- polish sentences while ignoring wrong status, missing outline, or missing source surface.

## Output labels

```text
VIETNAMESE_SURFACE_OK
VIETNAMESE_SURFACE_PARTIAL
VIETNAMESE_SURFACE_BLOCKED
PASS_INTEGRITY_OK
PASS_METADATA_CONFLICT
SOURCE_SURFACE_REQUIRED
HUMAN_READER_PASS_REQUIRED
```