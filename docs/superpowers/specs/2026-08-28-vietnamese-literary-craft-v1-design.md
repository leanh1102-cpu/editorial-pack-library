# Vietnamese Literary Craft v1 Migration Design

## Goal

Materialize the validated Notion staging stack as a portable `vietnamese-literary-craft/` Agent Skill candidate in this repository, without mixing SLTD-specific canon/taste into the general skill.

## Validated source state

- Runtime source: Operational Layer v0.1.
- Foundation: `FOUNDATION-INTEGRATED v0.5`.
- Intermediate: `INTERMEDIATE-INTEGRATED v0.5`.
- Advanced: `ADVANCED-INTEGRATED v0.3`; A6 remains narrow/source-gated.
- Writer Self Review: `WRITER_SELF_REVIEW-INTEGRATED v0.3.1`, composite evidence `31/32 + targeted closure 12/12`, hard fail 0.
- Cross-layer audit: staging-consistent, no extra Notion-only blind regression required.

## Package boundary

This migration creates a usable v1 behavioral/curriculum package, not a claim that the entire frozen knowledge architecture is complete. Specialized `theory/`, `forms/`, `register/`, `analysis/`, `craft/`, and `corpus/` coverage remains source-gated where content has not been validated.

## Target root

`vietnamese-literary-craft/`

The initial physical package contains:

- `SKILL.md`
- `CONSTITUTION.md`
- `curriculum/FOUNDATION.md`
- `curriculum/INTERMEDIATE.md`
- `curriculum/ADVANCED.md`
- `curriculum/WRITER_SELF_REVIEW.md`
- `runtime/runtime-protocol.md`
- `runtime/mode-routing.md`
- `runtime/stop-conditions.md`
- `evaluation/ai-writing-rubric.md`
- `glossary/TERMS.md`
- `drills/recognition/README.md`
- `drills/diagnosis/README.md`
- `drills/revision/README.md`
- `drills/composition/README.md`
- `drills/transfer/README.md`
- `harness/INDEX.md`
- `maintenance/promotion-rules.md`

## Runtime contract

Router: `TASK → MODE → LEVEL → FORM → REGISTER → MODULES → EXECUTION → SELF-CHECK`.

Revision spine: `TASK → CLASSIFY → DIAGNOSE → DECIDE → EXECUTE → PRESERVATION CHECK → STOP`.

Actions: `PRESERVE / MIN_EDIT / REVISE / HOLD-INSUFFICIENT_EVIDENCE`.

Core invariants:

1. Evidence before conclusion.
2. Function before correction.
3. Preserve living voice/register/form/ambiguity/reader inference.
4. Keep fact, claim, belief, memory, lie, inference, and reader belief distinct.
5. Use the smallest defensible intervention.
6. No fabricated source/canon/history/textual evidence.
7. No polish for polish's sake.
8. Dynamic self-revision hard cap 5; pass 6 forbidden.
9. `SENSORY-MEDIATION v0.1` remains narrow and contact-bound; it is not a global show-don't-tell rule.

## Source-scope locks

- F2 does not become a universal Vietnamese grammar theory.
- Historical/register/form claims remain source-gated where evidence is incomplete.
- Advanced A6 broad genre taxonomy remains gated.
- WSR W2 deeper taxonomy remains narrow.
- WSR W8 stop/release behavior remains internal operational policy, not an externally attributed universal law.
- Copyrighted full-text corpus is not packaged unless lawful/user-provided.

## Migration and verification

1. Create the exact Markdown package on an isolated feature branch.
2. Verify required files, frontmatter, internal references, forbidden SLTD leakage, pass-5 cap, sensory-mediation scope, and source-scope locks with deterministic static checks.
3. Review the branch diff before runtime testing.
4. Load the physical candidate in the actual PAI Linux runtime.
5. Run `BASELINE-36`, sensory-mediation repair regressions, routing sentinels, and compact cross-layer load sentinels.
6. Reject the candidate if any new preservation, epistemic, voice/register, routing, source-attribution, pass-cap, or curriculum-routing regression appears.
7. Only after physical runtime regression passes may the package be called v1 usable/install-ready.

## Non-goals

- No GitHub Actions, project boards, issues, automation files, or new Notion databases.
- No SLTD manuscript copy or SLTD-specific taste/canon inside the general skill.
- No claim of complete classical-form/corpus coverage.
