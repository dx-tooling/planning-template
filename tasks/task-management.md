# Task Management Process

This document defines the execution workflow for task files.

## Directory Structure

```text
planning-template/tasks/
├── task-management.md
├── todo/
├── in-progress/
└── done/
```

## Task Lifecycle

```text
todo/ -> in-progress/ -> done/
                     \
                      -> ADR/PRD + memory updates (required before done)
```

## Lifecycle Rules

1. `todo/`: task is defined and ready.
2. `in-progress/`: task is actively executed.
3. `done/`: implementation complete and documentation feedback loop closed.

Move files between folders to represent state changes. Do not duplicate task files.

## Task File Requirements

- Use the frontmatter and sections from [../templates/task-template.md](../templates/task-template.md).
- `source` must include at least one PRD or ADR reference.
- Acceptance criteria must be EARS-formatted, measurable, and checked before completion.

## Working Agreement

- Prefer one active task per contributor by default.
- If a task is too large, split it before execution.
- Keep implementation notes current while working, not after.

## Completion Gate (Required)

A task can move to `done/` only when all are true:

- [ ] Acceptance criteria checked.
- [ ] EARS compliance checked (`shall`, explicit system/component, correct pattern).
- [ ] Verification checklist addressed.
- [ ] `ADR/PRD Updates` checkboxes resolved.
- [ ] Relevant memory entry added if new insight/pitfall exists.

## Backlog Hygiene

- Re-prioritize `todo/` regularly.
- Archive nothing from `done/`; preserve project history.
- If a task is invalidated, keep it and mark clearly as canceled in the file.
