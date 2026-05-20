# Screen Specs

## Purpose

This file defines how screens should be specified before frontend implementation. In this repository, it acts as a template for product-specific screen documentation.

## Required Screen Spec Fields

| Field | Description |
|---|---|
| Screen name | Human-readable screen or view name |
| Route or entry point | URL, app route, modal trigger, or flow step |
| User role | Role that uses the screen |
| Primary task | Task the screen helps complete |
| Layout structure | Major regions and hierarchy |
| Components | Required reusable components |
| Data requirements | Fields, lists, counts, filters, API needs |
| States | Loading, empty, error, success, disabled, permission |
| Responsive behavior | Desktop, tablet, mobile layout rules |
| Accessibility notes | Focus order, labels, keyboard, announcements |
| Acceptance criteria | Conditions for implementation approval |

## Pipeline Screen Spec Template

| Screen | Entry Point | Primary Task | Core Regions | Components | States |
|---|---|---|---|---|---|
| Design context | `design/00-context/design-context.md` | Understand product and source context | Purpose, inputs, product summary, open questions, quality gate | Tables, checklists | Draft, blocked, approved |
| Design brief | `design/01-requirements/design-brief.md` | Convert requirements into design brief | Problem, goals, requirements, risks, metrics | Requirement table, risk table | Draft, review needed, approved |
| User flow | `design/03-flow/user-flow.md` | Explain journey sequence | Primary flow, exception flows, gate | Text flow, table | Draft, approved |
| Handoff | `design/11-handoff/` | Prepare engineering build | Frontend, backend, components, criteria | Contracts, checklist | Review needed, approved |
| Validation audit | `design/12-validation/design-implementation-audit.md` | Confirm implementation quality | Audit scope, results, issues, signoff | Audit table | Pass, fail, partial |

## Product Screen Spec Template

```md
## Screen: [Name]

Status: Draft | Review needed | Approved | Superseded
Owner: [Name or role]
Source references: [Files, issues, PRs, Figma links]

### User and Task

- User role:
- Primary task:
- Secondary tasks:
- Business rule:

### Layout

- Header:
- Main content:
- Secondary content:
- Actions:
- Footer or persistent controls:

### Components

| Component | Purpose | Data | States |
|---|---|---|---|
| TBD | TBD | TBD | TBD |

### Responsive Behavior

- Desktop:
- Tablet:
- Mobile:

### Accessibility

- Keyboard:
- Screen reader:
- Contrast:
- Focus management:

### Acceptance Criteria

- [ ] TBD
```

## Quality Gate

- No P0 screen is handed off without layout, components, states, responsive behavior, accessibility, and acceptance criteria.
- Every screen spec references source context or lists assumptions.
