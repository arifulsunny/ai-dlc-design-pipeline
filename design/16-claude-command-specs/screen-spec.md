# Command: /screen-spec

## Purpose

Generate implementation-ready screen specifications.

## Inputs

- `design/03-flow/user-flow.md`
- `design/03-flow/navigation-map.md`
- `design/03-flow/screen-inventory.md`
- `design/04-ux/interaction-model.md`
- `design/04-ux/state-model.md`
- `design/05-layout/component-map.md`
- `design/06-style-guide/design-tokens.json`

## Output File

`design/05-layout/screen-specs.md`

## Required Sections

- Screen name
- Route or entry point
- User role
- Primary task
- Layout structure
- Components
- Data requirements
- States
- Responsive behavior
- Accessibility notes
- Acceptance criteria
- Source references, when multi-source
- Quality gate

## Quality Score Criteria

| Category | 5 Means |
|---|---|
| Layout clarity | Regions, hierarchy, and actions are buildable |
| Component clarity | Components, states, and contracts are known |
| Responsive readiness | Desktop and mobile rules are explicit |
| Accessibility readiness | Focus, labels, headings, and state communication are covered |

## Pass Threshold

- Standard: 4.0
- Full: 4.25

## Failure Re-Entry

If score is below threshold, return to flow, state model, component map, or design tokens.
