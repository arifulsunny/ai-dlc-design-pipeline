# Screen Inventory

## Purpose

This file lists the screens, pages, views, dialogs, or document sections required by the design pipeline. For product-specific projects, replace or extend these entries with the actual product screens.

## Pipeline Artifact Inventory

| Screen or Artifact | Type | Primary User | Priority | Status |
|---|---|---|---:|---|
| Design context intake | Documentation view | AI agent, product, design | P0 | Defined |
| Design brief | Documentation view | Product, BA, design | P0 | Defined |
| User role matrix | Matrix | BA, UX, product | P0 | Defined |
| Task priority map | Matrix | Product, UX | P0 | Defined |
| User flow | Flow document | UX, frontend, QA | P0 | Defined |
| Navigation map | IA document | UX, frontend, AI agent | P1 | Defined |
| Screen inventory | Scope matrix | Product, design, frontend | P0 | Defined |
| Flow diagram | Mermaid diagram | All reviewers | P1 | Defined |
| UX principles | Design rules | UX, product, engineering | P1 | Defined |
| Interaction model | Behavior spec | UX, frontend | P0 | Defined |
| State model | State spec | UX, frontend, backend, QA | P0 | Defined |
| Screen specs | Layout specification | Product designer, frontend | P0 | Defined |
| Responsive rules | Layout rules | Product designer, frontend | P1 | Defined |
| Component map | Component inventory | Product designer, frontend | P0 | Defined |
| Style guide | Visual rules | Design, frontend | P1 | Defined |
| Design tokens | Machine-readable tokens | Frontend, design system | P1 | Defined |
| Component usage guidelines | Usage rules | Design, frontend | P1 | Defined |
| Accessibility checklist | QA checklist | UX, QA, frontend | P0 | Defined |
| Accessibility risk report | Risk report | UX, QA, product | P0 | Defined |
| Edge-case matrix | Matrix | BA, QA, engineering | P1 | Defined |
| Scalability notes | Planning document | Engineering, design | P1 | Defined |
| Design risk log | Risk register | Delivery, product, design | P1 | Defined |
| Prototype notes | Prototype documentation | Design, stakeholders | P2 | Defined |
| Interaction spec | Detailed behavior | Design, frontend | P1 | Defined |
| Design review report | Review output | Design lead, product, engineering | P0 | Defined |
| Frontend handoff | Engineering spec | Frontend, AI coding agent | P0 | Defined |
| Backend impact | Engineering impact | Backend, QA | P0 | Defined |
| Component contract | Interface contract | Frontend, design system | P0 | Defined |
| Acceptance criteria | Testable criteria | QA, product, engineering | P0 | Defined |
| Design implementation audit | Audit report | QA, design, frontend | P0 | Defined |
| Design change log | Change history | Design owner, product | P0 | Defined |
| Design decision records | Decision log | Design lead, engineering | P0 | Defined |
| Version history | Version tracking | Delivery, design owner | P0 | Defined |
| Release design notes | Release summary | Product, QA, engineering | P1 | Defined |
| Design system update log | System feedback | Design lead | P1 | Defined |
| Reusable patterns | Pattern library notes | Design system, frontend | P1 | Defined |
| Deprecated patterns | Deprecation notes | Design system, frontend | P1 | Defined |
| Future improvement notes | Backlog notes | Product, design | P2 | Defined |

## Product Screen Template

| Screen | User Role | User Task | Route or Entry Point | Components | States | Priority |
|---|---|---|---|---|---|---:|
| TBD | TBD | TBD | TBD | TBD | Loading, empty, error, success | P0 |

## Quality Gate

- Every screen maps to a user role and task.
- Every P0 screen has states, components, and acceptance criteria.
- Removed or deferred screens are documented in version-control files.
