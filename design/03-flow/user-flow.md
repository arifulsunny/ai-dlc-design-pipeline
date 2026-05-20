# User Flow

## Purpose

This file defines how people and AI agents move from repository context to approved, validated, and versioned design artifacts.

## Primary Pipeline Flow

```text
GitHub Repo
-> Main Context File
-> Design Context Intake
-> Requirement to Design Brief
-> User Role and Task Mapping
-> User Flow and Information Architecture
-> UX Strategy and Interaction Model
-> Screen Specs and Layout Planning
-> Style Guide and Design System Mapping
-> Accessibility Review
-> Scalability and Edge Case Review
-> Prototype or Figma Documentation
-> Multi-Agent Design Review
-> Frontend and Backend Handoff
-> Implementation Validation
-> Design Documentation and Version Control
-> Design System Update
```

## Human Review Flow

| Step | Actor | Action | Output |
|---|---|---|---|
| 1 | Product/BA | Provide requirements and repo context | Source inputs |
| 2 | AI agent | Draft context and design brief | Context and brief files |
| 3 | Product/design | Review assumptions and open questions | Approved or revised brief |
| 4 | UX/product design | Define flows, layout, style, states | Design artifacts |
| 5 | Accessibility/QA | Review risks and checklist | Accessibility report |
| 6 | Design/engineering | Prepare handoff | Handoff artifacts |
| 7 | Frontend/backend | Implement against handoff | Working product |
| 8 | QA/design | Audit implementation | Validation report |
| 9 | Design owner | Update change log and version | Version-control artifacts |
| 10 | Design lead | Capture reusable patterns | Design system update |

## Exception Flows

### Missing Context

```text
Context Intake
-> Missing product goal, user role, API, or design system input
-> Add open question with owner
-> Block dependent artifact
-> Resume after answer is documented
```

### Requirement Change During Implementation

```text
Change Request
-> Identify impacted roles, flows, screens, components, APIs, and tests
-> Update design brief and affected files
-> Add design change log entry
-> Add or update design decision record
-> Re-run handoff and validation gates
```

### Design System Gap

```text
Screen Spec
-> Required component or token missing
-> Propose reusable pattern
-> Document temporary implementation rule
-> Add item to design system update log
```

## Quality Gate

- Every flow has a clear entry point, decision point, completion state, and exception state.
- Design changes re-enter the pipeline at the earliest impacted artifact.
- Implementation should not start until primary flow, error flow, and empty state flow are documented for the feature.
