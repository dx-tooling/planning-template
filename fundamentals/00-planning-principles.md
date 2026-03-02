# Planning Principles

These principles define how planning should be created, maintained, and used in LLM-assisted software product work.

## 1) Outcome First

Planning artifacts exist to drive product outcomes, not document volume.

- Every PRD feature must map to a user or business outcome.
- Every ADR must justify why a technical decision supports that outcome.
- Every task must include acceptance criteria tied to outcome quality.

## 2) Traceability by Default

All major artifacts must be linkable and navigable end-to-end.

- PRD features should carry stable IDs (for example: `F-01`).
- ADRs should reference impacted PRD features.
- Tasks should reference source PRD/ADR IDs.
- Memory entries should reference task IDs and source docs when relevant.

## 3) Stable Structure, Flexible Content

Use fixed headings and metadata schemas so humans and LLMs can parse artifacts consistently.

- Keep canonical section names from templates.
- Add detail inside sections, not by inventing new top-level structures.
- Keep one concept per document when possible.

## 4) EARS Requirement Language Standard

All requirements and acceptance criteria must be written in EARS format.

- Use one requirement per line/bullet and assign IDs `R1`, `R2`, ...
- Every requirement must name the explicit system/component and use `shall`.
- Prefer observable behavior and invariants over implementation detail.
- Avoid file/function references unless they are part of an external contract.

Approved EARS patterns:
- Ubiquitous: `The <system> shall <response>.`
- State-driven: `While <precondition(s)>, the <system> shall <response>.`
- Event-driven: `When <trigger>, the <system> shall <response>.`
- Optional feature: `Where <feature/scope applies>, the <system> shall <response>.`
- Unwanted behavior: `If <unwanted condition>, then the <system> shall <mitigation>.`
- Complex: `While <precondition(s)>, when <trigger>, the <system> shall <response>.`

## 5) Decision Quality Over Speed

Fast drafting is useful, but planning quality gates are mandatory for non-trivial work.

- Always include alternatives for meaningful architectural decisions.
- Always capture downside and risk, not only positives.
- Mark assumptions explicitly and convert unresolved assumptions to tasks.

## 6) Small Executable Tasks

Tasks should be independently executable and reviewable.

- Favor small tasks that can be completed in one focused session.
- If acceptance criteria are vague or not EARS-compliant, split or rewrite before implementation.
- Keep no more than one active in-progress task per contributor by default.

## 7) Continuous Feedback Loop

Implementation must update planning artifacts; otherwise, planning becomes stale.

- Each completed task includes PRD/ADR update checks.
- Missing documentation updates block task completion.
- Learnings and gotchas are added continuously, not only at project end.

## 8) Human Accountability

LLMs accelerate drafting and decomposition, but final accountability remains with humans.

- Humans approve final PRDs/ADRs before execution.
- Humans resolve high-impact tradeoffs and scope changes.
- LLM outputs are reviewed against checklist-based quality controls.

## 9) Explicit Scope Management

Scope must be bounded and transparent.

- Every PRD includes out-of-scope boundaries.
- Every change request is categorized: in-scope update, deferred, or rejected.
- Any scope expansion must include impact on timeline and dependencies.

## 10) Documentation as Operational System

These files are not passive docs; they are the operating interface for execution.

- Task folders represent state.
- ADR status represents decision state.
- Memory files represent accumulated execution intelligence.
