# SLTD Editorial Hooks

These hooks are manual agent checks. They do not create automation, scripts, or workflow steps.

## BEFORE_READ

Confirm:

```text
SOURCE USED:
SCOPE:
PAGE TYPE:
CURRENT OR LEGACY:
LOCK STATUS:
```

Stop if the source is unclear.

## BEFORE_AUDIT

Confirm:

- task matches the user request;
- scope is named;
- chapter range is exact;
- source priority has been checked;
- legacy source is not treated as current manuscript.

## BEFORE_REWRITE

Confirm:

- Source Lock exists;
- Must Not Reveal exists when lore is involved;
- Scene Question exists;
- chapter outcome is not changed;
- rewrite stays inside one scene or named scope.

If any item is missing, stop and ask for the missing source.

## AFTER_REWRITE

Check:

- no new canon;
- no lore before lived scene;
- no staged object chain;
- no same-voice dialogue;
- no clean-but-thin result;
- changed state is visible;
- cost or pressure is present.

## STOP CONDITIONS

Stop when:

- current source is not confirmed;
- manuscript source is missing;
- a legacy page conflicts with current Notion;
- a cluster is treated as locked while one chapter remains unready;
- lore appears before body, house, object, money, relation, or decision;
- output would create new management structure.
