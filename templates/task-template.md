---
id: TASK-XX
title: <Short descriptive title>
source: PRD-XX:F-YY | ADR-XX
priority: high | medium | low
created: YYYY-MM-DD
started: YYYY-MM-DD
completed: YYYY-MM-DD
owner: <name/role>
---

# <Task Title>

## Description

Describe what should be implemented and why this task exists.

## Acceptance Criteria

- [ ] R1: When <trigger>, the <system> shall <response>.
- [ ] R2: While <state>, the <system> shall <response>.
- [ ] R3: If <unwanted condition>, then the <system> shall <mitigation>.

## Implementation Notes

Capture decisions, constraints, and relevant execution details as work progresses.

## Verification

- [ ] Unit/automated tests updated or created
- [ ] Manual verification steps run
- [ ] Logs/metrics checked (if relevant)

## Dependencies

- Blocking dependency:
- Related task(s):

## ADR/PRD Updates

Changes that must be fed back into planning artifacts:
- [ ] Update ADR-XX: <what changed>
- [ ] Update PRD-XX: <what changed>
- [ ] Add memory entry in `memory/learnings.md` or `memory/gotchas.md`

## Follow-Up Tasks

- [ ] Optional follow-up task proposal

---

## Notes for Template Users

- Keep tasks small enough to complete in one focused implementation cycle.
- If acceptance criteria become ambiguous or non-EARS, pause and rewrite before coding.
- Do not move task to `done` with unresolved ADR/PRD update checkboxes.
