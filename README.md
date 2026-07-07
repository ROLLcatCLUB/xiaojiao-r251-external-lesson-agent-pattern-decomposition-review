# R251 External Lesson Agent Pattern Decomposition Review

This is a narrow GPT/human review package for `1013R_R251_EXTERNAL_LESSON_AGENT_PATTERN_DECOMPOSITION`.

## Review conclusion wanted

Please audit whether R251 correctly decomposes the four external teacher-prep projects into Xiaobei-native design pattern cards, while preserving the current main-chain boundary:

```text
single_lesson_template + source policy + teacher review gate + R220F readonly route
```

## What this package contains

- `review_notes/`: card index, per-project pattern summaries, mapping matrix, non-adoption guard, and next-stage recommendation.
- `source/r251_pattern_cards.json`: 16 structured pattern cards.
- `source/r250_source_evidence_map.json`: source evidence inherited from R250.
- `source/external_reference_manifest.json`: local downloaded repo manifest.
- `validation/validate_1013R_R251_external_lesson_agent_pattern_decomposition_result.json`: validation result.
- `README_R251_LOCAL_SOURCE.md`: copied local R251 README.

## What this package does not contain

- No external repository source code.
- No copied GPL-3.0 saniales content.
- No Xiaobei backend/frontend runtime code.
- No dependencies, model calls, generated lesson output, database export, Feishu data, memory data, or formal export.

## Suggested audit questions

1. Are the 16 pattern cards specific enough to become future contracts?
2. Does every card correctly avoid direct source-code adoption?
3. Are R240/R252/R230/R210/R95 mappings in the right order?
4. Are the saniales GPL boundary, classmin heavy-stack boundary, Divanshi provider/UI boundary, and Claw-ED no-early-R95 boundary strict enough?
5. Should the next stage be R240 free-prep recovery or R252 teacher_execution_map/classroom_timeline contract?
