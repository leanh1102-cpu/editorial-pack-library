# SLTD Vietnamese Register & Viet Dao Gate

This gate controls Vietnamese register, Sino-Vietnamese load, and Viet Dao prose color.

It prevents two opposite failures:

- prose that reads like translated Chinese xianxia or wuxia;
- prose that strips all Sino-Vietnamese weight and loses the Dao / old-world register.

## Core rule

Use Vietnamese life for the scene body. Use Sino-Vietnamese for the concept layer.

```text
VIET LIFE = body, work, food, illness, debt, weather, mud, smoke, dog, door, bowl, hand, breath
SINO-VIETNAMESE = law, Dao, rank, taboo, rite, old object, formal title, inherited concept
VIET DAO = Vietnamese scene life carrying a controlled Dao register without becoming translated Chinese prose
```

Do not let terminology replace scene pressure.

Do not purge all Sino-Vietnamese if the scene needs ritual, law, rank, old fear, or Dao weight.

## Use when

- the user says the prose is too Chinese, too translated, too Han-Viet, too xianxia, or lacks Vietnamese naturalness;
- the user says the prose has lost Viet Dao flavor because it became too plain or modern;
- a passage uses many terms such as khi tuc, tam than, co xua, co duyen, van menh, nhan qua, huyen co, dao van without scene pressure;
- sentence order feels translated rather than written in Vietnamese;
- dialogue sounds like wuxia subtitle speech;
- line surgery can identify smell but needs a register target.

## Authority

This gate sits below:

```text
current user instruction
current Notion source or user-provided source packet
source fidelity gate
canon guard
evidence discipline
role boundary contracts
```

It must not change canon terms, rename established concepts, flatten Dao register, or invent new terminology.

## Register target by scene layer

Use this split:

```text
HOUSEHOLD / BODY / SURVIVAL:
- prefer plain Vietnamese and concrete verbs
- hands, bowl, door, stove, dog, debt, cough, mud, cold, cloth, needle

VILLAGE / SOCIAL PRESSURE:
- mostly Vietnamese, with occasional formal or old words when social distance requires it
- avoid everyone speaking like sect elders

DAO / LAW / RITE / FORBIDDEN KNOWLEDGE:
- controlled Sino-Vietnamese allowed
- terms must be anchored by scene pressure before explanation

FORMAL TITLE / LINEAGE / OLD PAPER / CULTIVATION CONCEPT:
- use established canon terms
- do not multiply synonyms for elegance
```

## Sino-Vietnamese load test

Ask:

```text
Which words must stay Sino-Vietnamese for canon, Dao weight, rank, law, or rite?
Which words can be lowered to plain Vietnamese without losing meaning?
Which terms are only decoration?
Does the paragraph still move if all abstract terms are removed?
Does the scene pressure appear before the term?
```

If the paragraph depends on terms rather than action, mark overload.

## Chinese-translation syntax test

Flag sentence shapes that sound translated:

```text
- modifier stack before action
- abstract noun chain before body/action
- character reacts with polished mental labels
- every beat uses khẽ, chợt, dường như, trong lòng, ánh mắt, khí tức
- sentence explains state before showing movement
```

Repair by moving action earlier, cutting generic intensifiers, and grounding through scene-native objects.

## Failure labels

Use these labels:

```text
HANVIET_OVERLOAD
HANVIET_UNDERCUT
CHINESE_TRANSLATION_SYNTAX
FAKE_CLASSICAL_VIETNAMESE
MODERN_FLAT_PROSE
DAO_REGISTER_MISSING
VIET_LIFE_ANCHOR_MISSING
DIALOGUE_WUXIA_TRANSLATION
ABSTRACT_QI_PRESSURE
TERMS_BEFORE_SCENE
TERM_SYNONYM_SPRAWL
REGISTER_MISMATCH
```

## Safe repair

Safe repair may:

- lower decorative Sino-Vietnamese into concrete Vietnamese action;
- keep canon terms but delay explanation until pressure earns it;
- preserve one sharp Dao term instead of three ornamental terms;
- replace translated mental-state formulas with body, object, or practical action;
- make dialogue shorter, more evasive, more work-bound, and less subtitle-like;
- restore old-world weight through silence, taboo, formal address, object handling, or ritual behavior instead of term density.

Safe repair must not:

- remove established canon terms;
- invent new Vietnamese replacements for locked terms;
- make Dao scenes sound purely modern;
- turn rural/household scenes into sect-court speech;
- remove all Hán Việt as a rule;
- add lore or new titles to create flavor.

## Vietnamese register audit

Use:

```text
VIETNAMESE REGISTER CHECK
SCOPE:
SOURCE USED:
SOURCE SURFACE:
SCENE TYPE:
REGISTER TARGET:
HAN-VIET LOAD:
CHINESE-TRANSLATION SYNTAX:
VIET LIFE ANCHOR:
DAO / HUYEN REGISTER:
DIALOGUE NATURALNESS:
PROSE SAMPLE MATCH:
FAILURE LABELS:
PATCH PRINCIPLE:
ROLE HANDOFF:
NEXT NODE:
```

## Patch rule

If exact source text is available:

```text
OLD:
REGISTER FAILURE:
WHY IT MISREADS:
NEW:
WHAT STAYS SINO-VIETNAMESE:
WHAT IS LOWERED TO VIETNAMESE LIFE:
RISK:
```

If exact source text is missing, do not patch. Run Source Surface Check.

## Handoff

If line rhythm is the main problem, hand off to Vietnamese Line Surgery.

If prose lacks scene pressure, hand off to First-Pass Editorial Workflow or Scene-First Prose Judgment.

If terms are canon-locked, hand off to Canon Guard.

If the assembled chapter changes register between scenes, hand off to Chapter Assembly & Split Check.

## Output labels

```text
VIETNAMESE_REGISTER_OK
REGISTER_PARTIAL
HANVIET_OVERLOAD_DETECTED
CHINESE_TRANSLATION_SYNTAX_DETECTED
DAO_REGISTER_MISSING
VIET_DAO_RECALIBRATION_REQUIRED
SOURCE_SURFACE_REQUIRED
```