# R251 External Lesson Agent Pattern Decomposition

Stage ID: `1013R_R251_EXTERNAL_LESSON_AGENT_PATTERN_DECOMPOSITION`

R251 decomposes the four external teacher-prep reference projects from R250 into Xiaobei/师维-compatible design pattern cards. It does not study source for reuse, copy code, run external projects, install dependencies, call providers, or modify the current chain.

## Purpose

Turn external references into contract-ready design patterns:

- Products: what artifacts a mature prep system produces.
- Flow: how one artifact hands off to the next.
- Roles: which stage owns which boundary.
- Quality: where teacher review and validation must happen.
- Input/output: what minimum input is enough, and where it is insufficient.

## Protected Chain

R251 preserves the current priority:

```text
single_lesson_template
source policy
teacher review gate
R220F readonly route
```

No R251 card is allowed to become direct runtime implementation. Every card is `contract_only`, `naming_reference`, or `future_design`.

## Files

- `r251_pattern_card_index.md`
- `r251_pattern_cards.json`
- `r251_claw_ed_bundle_patterns.md`
- `r251_saniales_workflow_patterns.md`
- `r251_classmin_timeline_xiaojiao_patterns.md`
- `r251_divanshi_free_prep_input_patterns.md`
- `r251_xiaobei_mapping_matrix.md`
- `r251_non_adoption_and_license_guard.md`
- `r251_next_stage_recommendation.md`
- `validate_1013R_R251_external_lesson_agent_pattern_decomposition_result.json`

## Boundary

R251 is docs-only. It creates design cards for future R240, R252, R230, R210, and R95 planning, but it does not open those lines.

