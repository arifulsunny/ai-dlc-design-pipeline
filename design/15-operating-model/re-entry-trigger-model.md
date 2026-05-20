# Re-Entry Trigger Model

## Purpose

This file defines which events invalidate prior design artifacts and which stages must be re-run.

## Re-Entry Rules

| Trigger Event | Invalidates | Re-Run Files | Required Action |
|---|---|---|---|
| Requirement changes | Brief, task map, flow, screen specs, acceptance criteria | `01-requirements`, `02-users`, `03-flow`, `05-layout`, `11-handoff`, `13-version-control` | Update affected artifacts and change log |
| API contract changes | State model, backend impact, frontend handoff, acceptance criteria, validation | `04-ux/state-model.md`, `11-handoff/backend-impact.md`, `11-handoff/frontend-handoff.md`, `11-handoff/acceptance-criteria.md`, `12-validation` | Re-score backend/API alignment |
| Permission model changes | Role matrix, flow, state model, backend impact, accessibility risks | `02-users`, `03-flow`, `04-ux`, `07-accessibility`, `11-handoff/backend-impact.md` | Re-check restricted and disabled states |
| New reusable component | Component map, component contract, design system update | `05-layout/component-map.md`, `11-handoff/component-contract.md`, `14-design-system-update`, `17-pattern-governance` | Add pattern candidate or reusable pattern |
| Accessibility issue found | Accessibility checklist, risk report, screen specs, validation | `07-accessibility`, `05-layout/screen-specs.md`, `12-validation` | Fix or accept risk with owner |
| Visual implementation mismatch | Screen specs, tokens, component contract, validation | `05-layout`, `06-style-guide`, `11-handoff/component-contract.md`, `12-validation` | Record audit result and update handoff |
| Design decision reversed | DDR, change log, impacted artifacts | `13-version-control`, affected stage files | Add superseding DDR |
| Multi-source conflict found | Source references, context, affected files | `source-reference-instructions.md`, `00-context`, affected files | Resolve or assign conflict |

## Re-Entry Comment Template

```md
## Design Re-Entry Required

Trigger:
Detected in:
Impacted artifacts:
Required re-run:
Owner:
Due before:
Blocking score category:
Related issue or PR:
```

## Quality Gate

- A trigger cannot be ignored without an owner-approved reason.
- Any re-entry that changes design meaning must update `13-version-control/design-change-log.md`.
- If a re-entry changes the reason behind a decision, update `13-version-control/design-decision-records.md`.
