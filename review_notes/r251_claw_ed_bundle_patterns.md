# R251 Claw-ED Bundle Patterns

## Useful Pattern Set

Claw-ED should be read as a product-shape reference: it shows that a teacher-prep system eventually needs more than a single generated lesson body. The cards below translate that into Xiaobei contracts.

## `bundle.manifest.v1`

- Source evidence: Claw-ED README and R250 evidence describe complete lesson bundles, teacher DOCX, student DOCX, PPTX, differentiated artifacts, and multi-format export.
- Xiaobei translation: define `lesson_bundle_manifest` before any R95 export.
- Current boundary: no R95 now.

## `bundle.dependency_graph.v1`

- Source evidence: Claw-ED compiles teacher/student/slides from shared master content.
- Xiaobei translation: every future artifact should know whether it depends on accepted lesson body, classroom timeline, source ledger, teacher confirmation, or accepted patch.
- Current boundary: no compile/export.

## `bundle.quality_gate.v1`

- Source evidence: Claw-ED README describes quality checks such as Bloom progression, assessment, differentiation specificity, and diversity audit.
- Xiaobei translation: quality gate becomes a checklist around source grounding, objectives, assessment, differentiation, pacing, readability, and export readiness.
- Current boundary: no auto-retry into teacher main text.

## `bundle.approval_policy.v1`

- Source evidence: Claw-ED risk/approval model classifies read-only, local write, network call, and package install actions.
- Xiaobei translation: action policy must distinguish preview, candidate patch, accepted preview, formal apply, export, provider call, and external publish.
- Current boundary: no standing approval behavior copied.

## Non-Adoption

Do not adopt Claw-ED runtime, provider handling, local writers, browser/web search, Drive integration, Telegram transport, scheduler, or self-modifying tools.

