# R251 saniales Workflow Patterns

## Useful Pattern Set

saniales/ai-lesson-planner is useful because it separates course metadata, lesson highlights, discourse, slide artifacts, and export. Because it is GPL-3.0 in the R250 manifest, nothing should be copied.

## `workflow.course_metadata_boundary.v1`

- Source evidence: course-planner owns course outline and metadata, not lesson-level content.
- Xiaobei translation: R240/unit planning may own unit metadata, lesson index, and handoff targets, but cannot write teacher main text.

## `workflow.lesson_handoff_artifact.v1`

- Source evidence: workflow moves from highlights to discourse to slides with explicit artifact locations.
- Xiaobei translation: every stage handoff should carry source status, missing fields, owner, and next artifact target.

## `workflow.slide_artifact_boundary.v1`

- Source evidence: slides-maker derives slide artifacts from existing lesson artifacts and treats templates as guides.
- Xiaobei translation: R230 big-screen page plans must be derived from accepted lesson sections and classroom timeline.

## `workflow.single_artifact_owner.v1`

- Source evidence: saniales separates role responsibilities.
- Xiaobei translation: one stage owns one artifact boundary. This is the core reusable design principle.

## GPL Guard

Do not copy saniales agent files, prompts, scripts, templates, or directory structure. Use independently expressed contracts only.

