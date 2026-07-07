# R251 Xiaobei Mapping Matrix

## Stage Mapping

| Xiaobei stage | Relevant cards | What they provide | What remains forbidden |
| --- | --- | --- | --- |
| R201 / R220 | `workflow.single_artifact_owner.v1`, `bundle.quality_gate.v1` | Protect artifact ownership and source/teacher review gates | No external code, no new route behavior |
| R240 | `freeprep.minimum_input.v1`, `freeprep.china_art_extension.v1`, `workflow.course_metadata_boundary.v1`, `workflow.lesson_handoff_artifact.v1` | Free-prep intake schema and workflow split | No UI copy, no provider call, no formal generation |
| R252 | `timeline.classroom_timeline_contract.v1`, `timeline.pacing_signal.v1`, `workflow.lesson_handoff_artifact.v1` | Teacher execution map and classroom timeline contract | No simulation runtime |
| R230 | `timeline.big_screen_reference.v1`, `workflow.slide_artifact_boundary.v1`, `bundle.dependency_graph.v1` | Big-screen page plan and page-step binding | No PPT export, no right rail binding until contract |
| R210 | `xiaojiao.in_class_support_boundary.v1`, `timeline.pacing_signal.v1`, `xiaojiao.simulated_student_state.v1` | Xiaojiao support boundaries and advisory signals | No auto-modification, no persisted simulated student data |
| R95 | `bundle.manifest.v1`, `bundle.dependency_graph.v1`, `bundle.approval_policy.v1`, `bundle.quality_gate.v1` | Export readiness contracts | No early export before review and route stability |

## Artifact Ownership Translation

| Artifact | Future owner | Consumed by |
| --- | --- | --- |
| `free_prep_intake` | R240 | R201 / source_understander |
| `single_lesson_template` | R201/R220 line | R252 / R230 / R95 |
| `teacher_execution_map` | R252 | R230 / R210 |
| `classroom_timeline` | R252 | R230 / R210 / R95 |
| `big_screen_page_plan` | R230 | R210 / R95 |
| `lesson_bundle_manifest` | R95 | Export gate |
| `quality_gate_checklist` | Quality sentinel / R95 | Teacher review gate |

## Core Principle

One stage owns one artifact boundary. Other stages may read or propose candidate patches, but cannot silently overwrite the owner artifact.

