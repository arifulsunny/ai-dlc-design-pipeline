# Command: /handoff

## Purpose

Generate implementation handoff artifacts for frontend, backend, QA, and AI coding agents.

## Inputs

- `design/03-flow/`
- `design/04-ux/`
- `design/05-layout/`
- `design/06-style-guide/`
- `design/07-accessibility/`
- `design/08-scalability/`
- API specs or backend notes

## Output Files

- `design/11-handoff/frontend-handoff.md`
- `design/11-handoff/backend-impact.md`
- `design/11-handoff/component-contract.md`
- `design/11-handoff/acceptance-criteria.md`

## Required Sections

- Frontend screen and component plan
- Backend/API impact
- Component contracts
- Required states
- Responsive requirements
- Accessibility requirements
- Acceptance criteria
- Source references, when multi-source
- Quality gate

## Quality Score Criteria

| Category | 5 Means |
|---|---|
| Frontend readiness | Screens, states, components, tokens, and responsive behavior are clear |
| Backend readiness | Data, permission, validation, and errors are clear |
| QA readiness | Acceptance criteria are testable |
| Traceability | Handoff links back to source artifacts |

## Pass Threshold

- Standard: 4.0
- Full: 4.25

## Failure Re-Entry

If score is below threshold, return to the lowest-scoring upstream artifact before implementation starts.
