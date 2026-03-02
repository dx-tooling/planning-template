# LLM-First Software Planning Template

This template provides a structured, reusable planning system for software product projects executed in a human + LLM workflow.

It is optimized for:
- clear decision quality
- high traceability from goals to execution
- low documentation drift during implementation
- easy context handoff across sessions

## Start Here

1. Read [fundamentals/00-planning-principles.md](fundamentals/00-planning-principles.md).
2. Read [fundamentals/01-document-map.md](fundamentals/01-document-map.md).
3. Read [fundamentals/02-traceability-model.md](fundamentals/02-traceability-model.md).
4. Copy templates from [templates/](templates/) into project artifacts.
5. Run task execution with [tasks/task-management.md](tasks/task-management.md).
6. Capture learnings continuously in [memory/](memory/).
7. Operate sessions with [llm-workflow/agent-operating-guide.md](llm-workflow/agent-operating-guide.md).

## Directory Layout

```text
planning-template/
├── fundamentals/
├── templates/
├── tasks/
│   ├── todo/
│   ├── in-progress/
│   └── done/
├── memory/
└── llm-workflow/
```

## Planning Stack

The planning stack is intentionally layered:

- **Fundamentals** define principles, terminology, and constraints.
- **PRDs** define product outcomes and scope.
- **ADRs** define key technical decisions and tradeoffs.
- **Tasks** define executable work and EARS-formatted acceptance criteria.
- **Memory** records implementation learnings and pitfalls.

Each layer references the layer above it, and implementation feeds back into source docs.

## First-Run Sequence (Under 5 Minutes)

1. Define project context and vocabulary in `memory/conventions.md`.
2. Create first PRD from `templates/prd-template.md`.
3. Create required ADRs from `templates/adr-template.md`.
4. Decompose into small tasks from `templates/task-template.md`.
5. Start execution by moving one task into `tasks/in-progress/`.
6. On completion, update PRD/ADR and add a memory entry.

## Daily Workflow

1. Pick the highest-value task from `tasks/todo/`.
2. Move it to `tasks/in-progress/` and add a `started` date.
3. Execute with EARS-formatted acceptance criteria as the definition of done.
4. Capture implementation notes during execution.
5. Complete ADR/PRD updates before moving task to `tasks/done/`.
6. Add learnings or gotchas to memory files.

## Template Quality Rules

- Keep section headings stable across all artifacts.
- Use explicit IDs (`PRD-01`, `ADR-03`, `TASK-12`).
- Use EARS-formatted, measurable, testable requirements/acceptance criteria over open-ended prose.
- Record alternatives and risks for non-trivial decisions.
- Never delete completed tasks; preserve planning history.

## Recommended Usage Pattern

- Use this repository as a source template.
- For a new product/project, copy it into a dedicated planning folder.
- Keep examples as examples; replace placeholders with project-specific values.
