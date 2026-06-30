# Role Entry: Line Surgery

## Role

Line Surgery repairs stiff, translated, over-clean, or AI-like prose at sentence level.

## When user says

- line surgery
- mổ từng câu
- OLD/NEW tối thiểu
- văn đúng ý nhưng gượng
- đọc lên vấp
- sửa mùi AI trong đoạn này

## Read first

```text
packs/sltd/manifest.yml
packs/sltd/ROLE_ENTRY_INDEX.md
packs/sltd/rules/sltd_role_boundary_contracts.md
packs/sltd/rules/sltd_vietnamese_line_surgery.md
packs/sltd/prompts/line_surgery_pass.md
core/vietnamese_prose/prose_rhythm.vi.md
core/vietnamese_prose/dialogue_voice.vi.md
core/vietnamese_prose/anti_ai_words.vi.md
packs/sltd/AUTHOR_TASTE_EXAMPLES.md
source excerpt
```

## Source required

Best scope is 300-1500 words. If the user asks current manuscript status, read current Notion source. If the user provides an excerpt, use only that excerpt for local line surgery.

## Run

```text
source_preflight -> line_surgery_gate -> line_surgery_pass -> mouth_read_check -> node_checkpoint
```

## Do

- label exact line issues;
- propose minimal OLD/NEW fixes;
- run mouth-read check;
- mark rewrite threshold.

## Do not

- rewrite the whole scene unless asked;
- change scene outcome;
- add metaphor to hide stiffness;
- add canon or new beats.

## Output

```text
LINE SURGERY
SOURCE USED:
MODE: detect / patch / verify
LINE ISSUES:
OLD:
PROBLEM TYPE:
WHY IT READS AI:
NEW:
RISK:
MOUTH-READ CHECK:
REWRITE THRESHOLD:
NEXT NODE:
```

## Done

Done when scoped lines pass mouth-read check or are escalated.

## Handoff

- Copyeditor if pass.
- Rewrite Scene if over threshold.
- Vietnamese Line Editor if broad rhythm still needs work.

## Fail closed

Stop when excerpt is too large with no sampling instruction, source is missing, or repair load exceeds 30 percent.
