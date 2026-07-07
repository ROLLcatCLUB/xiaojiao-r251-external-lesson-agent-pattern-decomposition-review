# R251 Next Stage Recommendation

## Decision

Do not open R95 next. Do not connect classmin or any external runtime. Do not build UI from Divanshi. Do not copy saniales prompts or agents.

## Recommended Order

1. `R240A_FREE_PREP_LINE_RECOVERY_AUDIT`
   - Goal: inspect current free-prep entry points and identify what can safely produce `free_prep_intake`.
   - Uses cards: `freeprep.minimum_input.v1`, `freeprep.china_art_extension.v1`, `workflow.course_metadata_boundary.v1`.

2. `R240B_FREE_PREP_INTAKE_SCHEMA_AND_WORKFLOW_CONTRACT`
   - Goal: define free-prep intake schema and handoff into `single_lesson_template`.
   - Uses cards: `workflow.lesson_handoff_artifact.v1`, `workflow.single_artifact_owner.v1`.

3. `R252_TEACHER_EXECUTION_MAP_AND_CLASSROOM_TIMELINE_CONTRACT`
   - Goal: define `teacher_execution_map` and `classroom_timeline` as Xiaobei-native contracts.
   - Uses cards: `timeline.classroom_timeline_contract.v1`, `timeline.pacing_signal.v1`, `timeline.big_screen_reference.v1`.

4. R230 big-screen/right-rail work
   - Goal: page references and display plans after R252 exists.
   - Uses cards: `workflow.slide_artifact_boundary.v1`, `timeline.big_screen_reference.v1`.

5. R95 export readiness
   - Goal: bundle manifest and export policy only after route, review, timeline, and big-screen contracts are stable.
   - Uses cards: `bundle.manifest.v1`, `bundle.dependency_graph.v1`, `bundle.approval_policy.v1`, `bundle.quality_gate.v1`.

## Immediate Recommendation

The next best engineering artifact is not code. It is the R252 contract for `teacher_execution_map` and `classroom_timeline`, unless the user wants to recover free-prep entry first. If choosing product sequence, R240 should come first; if choosing classroom execution sequence, R252 should come first.

