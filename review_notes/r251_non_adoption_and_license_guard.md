# R251 Non-Adoption And License Guard

## Global Prohibitions

- No copied external code.
- No copied GPL-3.0 saniales agent files, prompts, templates, scripts, or directory structure.
- No external dependency installation.
- No external project execution.
- No provider/model calls.
- No backend/frontend runtime modification.
- No R201/R220/R210/R230/R240/R95 modification.
- No formal apply, database write, Feishu write, memory write, or formal export.

## Project-Specific Guards

| Project | Guard |
| --- | --- |
| Claw-ED | Do not adopt runtime, file writers, provider layer, browser, Drive, Telegram, scheduler, approval DB, or self-modifying tools. |
| saniales/ai-lesson-planner | GPL-3.0 no-copy boundary. Re-express only design ideas as Xiaobei-native contracts. |
| classmin | Do not connect CrewAI, AutoGen, ChromaDB, Ollama, Streamlit, or simulation runtime to mainline. |
| DivanshiJain2005/AI-lesson-planner | Do not adopt Streamlit UI, direct API key/provider handling, old OpenAI SDK, or app.py shape. |

## Future Adoption Gate

Any future ticket using these cards must declare:

```text
pattern_id
target Xiaobei stage
artifact owner
adopt_as
source evidence
no-copy statement
no-runtime statement
teacher review point
rollback path
acceptance test
```

If `adopt_as` is anything like direct code reuse, the ticket fails R251 guard.

