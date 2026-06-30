# SLTD Command Recipes

Copy these recipes when asking an AI to work on SLTD.

## Boot any SLTD task

```text
Use editorial-pack-library/packs/sltd.
Read prompts/boot_task.md first.
Confirm agent role, source, scope, source layer, lock status, task skill, and stop condition check.
Then choose the task-specific prompt.
```

## Audit current Notion chapter

```text
Use editorial-pack-library/packs/sltd.
Read prompts/boot_task.md first.
Use current Notion Story SLTD Proser as source.
Read Chapter Index for [CHAPTER].
Read linked Scene Bank scenes if needed.
Do not use legacy Google Doc or old Workdeck as current manuscript.
Run multi_reviewer_pass.
```

## Audit C001-C030 packet

```text
Use editorial-pack-library/packs/sltd.
Read prompts/boot_task.md first.
Use Notion Story SLTD Proser.
Read Series Manuscript for packet read.
Read Chapter Index lock status for C001-C030.
If any chapter is not ready, say the packet is not locked.
Run audit_story_arc + multi_reviewer_pass.
```

## Rewrite one scene

```text
Use editorial-pack-library/packs/sltd.
Read prompts/boot_task.md first.
Run BEFORE_REWRITE hook.
Use only the named Notion Scene Bank scene: [SCENE].
Read Scene Question, Must Show, Must Not Reveal, Reader Effect.
Rewrite only this scene.
Run AFTER_REWRITE hook.
Return rewrite plus reviewer findings.
```

## Fix underreach

```text
Use editorial-pack-library/packs/sltd.
Read prompts/boot_task.md first.
Run intensity_pass.
Set CURRENT INTENSITY and TARGET INTENSITY.
Use sltd_underreach_gate.
Strengthen only through cost, body, object, relation, witness, debt, choice, or concrete mystery pressure.
Do not add new canon.
```

## C030 repair

```text
Use editorial-pack-library/packs/sltd.
Read prompts/boot_task.md first.
Use current Notion C030 page and linked Scene Bank scenes.
C030 is not locked until SC-030-01 to SC-030-05 pass real reading.
Rewrite one scene at a time.
Keep lore behind kitchen, medicine, sewing, dog, paper, ash, breath, and hiding choice.
```
