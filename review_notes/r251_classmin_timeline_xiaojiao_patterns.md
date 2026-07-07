# R251 classmin Timeline And Xiaojiao Patterns

## Useful Pattern Set

classmin is valuable as a classroom execution reference. It should not be used for mainline code or dependencies.

## `timeline.classroom_timeline_contract.v1`

- Source evidence: classmin has a classroom timeline parser and time-bounded stage/step logic.
- Xiaobei translation: R252 should define stage IDs, time ranges, teacher actions, student actions, purpose, and source refs.

## `timeline.big_screen_reference.v1`

- Source evidence: classmin uses teacher PPT page references during simulation.
- Xiaobei translation: R230 should define stable `page_id -> timeline_step_id` references.

## `timeline.pacing_signal.v1`

- Source evidence: classmin models time budget and teacher `[用时]` style pacing.
- Xiaobei translation: Xiaojiao can suggest pacing, but not auto-advance, rewrite, or apply.

## `xiaojiao.simulated_student_state.v1`

- Source evidence: classmin tracks simulated understanding, attention, and frustration with rules.
- Xiaobei translation: simulation diagnostics can help rehearsal only.
- Hard boundary: never store simulated state as real student profile or learning evidence.

## `xiaojiao.in_class_support_boundary.v1`

- Source evidence: classmin combines timeline, PPT references, activity types, and state signals.
- Xiaobei translation: Xiaojiao's classroom role is support, reminder, pacing suggestion, and confirmation surface, not autonomous plan mutation.

## Dependency Guard

Do not connect CrewAI, AutoGen, ChromaDB, Ollama, or Streamlit runtime to Xiaobei mainline in this stage.

