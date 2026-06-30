# SLTD Webnovel Packet Benchmark

Use this prompt when the user asks whether a chapter, packet, or arc has enough reader pull, webnovel momentum, addictive rhythm, or top-tier benchmark strength.

## Read first

1. `prompts/boot_task.md`
2. `rules/sltd_source_preflight.md`
3. `rules/sltd_webnovel_momentum_benchmark.md`
4. `rules/sltd_review_modes.md` if the user used a review mode
5. `rules/sltd_evidence_discipline.md`
6. `AUTHOR_TASTE_EXAMPLES.md`
7. current user request

## Scope routing

```text
1 chapter = chapter benchmark
3-10 chapters = packet benchmark
30 chapters = arc benchmark
100+ chapters = map-level benchmark only
```

If the request uses current/latest/Notion/current manuscript/readiness/lock language, current Notion source is required before verdict.

## Output

```text
WEBNOVEL PACKET BENCHMARK
SCOPE:
SOURCE USED:
REQUEST TYPE:
REVIEW MODE:
CURRENT SOURCE READ: YES / NO
CONTEXT BRIEF:
SCORE TABLE:
CHAPTER / PACKET FINDINGS:
DROP-OFF RISK:
PAYOFF DEBT:
UNDERREACH:
ANTI-AI RISK:
BLOCKERS:
PATCH PRIORITY:
EVIDENCE CHECK:
NODE LEDGER:
NEXT NODE:
```

## Rules

- Score only the source that was opened or provided.
- If source is incomplete, score only the in-context portion and state unread risk.
- Do not claim publication readiness unless the readiness route was requested and evidence exists.
- Do not claim SLTD equals or surpasses any named outside work.
- Use external benchmark language only as pressure-testing vocabulary: pull, payoff, escalation, mystery, reread value.
- Do not rewrite unless the user requests rewrite.
- For patch priority, propose smallest effective patch before full rewrite.
- When paired with REDTEAM, attack the strongest positive finding.
- When paired with PREMORTEM, assume the packet failed a reader binge and explain why.
- When paired with TASTELOCK, apply `AUTHOR_TASTE_EXAMPLES.md` to prose pull and distinctive SLTD flavor.
