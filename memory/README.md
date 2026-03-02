# Project Memory

This folder stores practical knowledge discovered during execution.

## Purpose

- Preserve non-obvious implementation insights.
- Prevent repeated mistakes.
- Keep human and LLM collaborators aligned with real project behavior.

## Files

| File | Purpose |
|---|---|
| `conventions.md` | Stable terminology and project-specific standards |
| `learnings.md` | Positive insights, successful patterns, useful discoveries |
| `gotchas.md` | Pitfalls, failure modes, and how to avoid them |

## Contribution Rules

Add memory entries:
- after completing meaningful tasks
- after resolving tricky bugs/issues
- when you discover a reusable pattern or recurring failure mode

## Entry Format

```markdown
### <Short Title> (YYYY-MM-DD)

What happened:
Why it matters:
How to apply/avoid:
Source: TASK-XX, ADR-XX, PRD-XX (as relevant)
```

## Quality Guidelines

- Keep entries concise and actionable.
- Prefer concrete examples over generic advice.
- Reference source artifacts for traceability.
