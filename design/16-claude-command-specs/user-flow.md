# Command: /user-flow

## Purpose

Generate user flow, navigation map, screen inventory, and Mermaid diagram from approved context and requirements.

## Inputs

- `design/00-context/design-context.md`
- `design/01-requirements/design-brief.md`
- `design/02-users/user-role-matrix.md`
- `design/02-users/task-priority-map.md`
- API and permission notes, if available

## Output Files

- `design/03-flow/user-flow.md`
- `design/03-flow/navigation-map.md`
- `design/03-flow/screen-inventory.md`
- `design/03-flow/flow-diagram.mmd`

## Required Sections

- Primary flow
- Secondary flow
- Empty state flow
- Error flow
- Permission restricted flow
- First-time user flow, if applicable
- Returning user flow, if applicable
- Screen inventory
- Navigation structure
- Mermaid diagram
- Source references, when multi-source
- Quality gate

## Quality Score Criteria

| Category | 5 Means |
|---|---|
| Flow completeness | Primary, exception, empty, and restricted paths are clear |
| Role alignment | Every path maps to a user role and task |
| Implementation usefulness | Frontend and backend can infer routes, states, and data needs |
| Reviewability | Diagram and text flow are easy to inspect |

## Pass Threshold

- Standard: 4.0
- Full: 4.25

## Failure Re-Entry

If score is below threshold, return to user role matrix, task priority map, or design brief.
