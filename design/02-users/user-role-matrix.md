# User Role Matrix

## Purpose

This file identifies who uses the pipeline and what each role needs from the design process. No screen, flow, or component should exist without a role and task behind it.

## Role Matrix

| User Role | Main Goal | Key Tasks | Access Level | UX Concern | Pipeline Outputs Used |
|---|---|---|---|---|---|
| Product manager | Ensure the feature solves the right business problem | Define scope, approve priorities, review risks | Full product context | Needs clear tradeoffs and measurable outcomes | Design brief, review report, release notes |
| Business analyst | Preserve requirement accuracy | Map requirements, clarify rules, document edge cases | Requirements and business rules | Needs traceability from requirement to task | Design brief, task map, edge-case matrix |
| UX designer | Create coherent user journeys | Define flows, interactions, states, error handling | Design artifacts | Needs role-specific tasks and constraints | User flow, interaction model, state model |
| Product designer | Create screen and visual specifications | Layout screens, define components, align style | Design system and UI artifacts | Needs reusable patterns and tokens | Screen specs, style guide, component map |
| Frontend engineer | Implement UI reliably | Build screens, states, components, responsive behavior | Frontend code and handoff docs | Needs precise contracts and acceptance criteria | Frontend handoff, component contract, tokens |
| Backend engineer | Support user workflows | Expose APIs, validation, permissions, state transitions | Backend code and API contracts | Needs data and permission impact | Backend impact, state model, acceptance criteria |
| QA engineer | Validate product behavior | Test flows, edge cases, accessibility, regressions | QA artifacts and implementation | Needs testable acceptance criteria | Accessibility checklist, audit, acceptance criteria |
| AI agent | Generate or review artifacts | Read sources, draft docs, update changes, check consistency | Repo files and permitted external sources | Needs stable structure and explicit source references | All pipeline files |
| Design lead | Approve design quality | Review UX, consistency, accessibility, design system impact | Full design artifacts | Needs decision traceability | Review report, decision records, update log |
| Delivery lead | Coordinate delivery readiness | Track blockers, handoff, validation, release readiness | Pipeline summary | Needs clear status and ownership | Risk log, acceptance criteria, release notes |

## Permission and Ownership Notes

| Artifact Area | Primary Owner | Reviewers |
|---|---|---|
| Context and requirements | Product manager, business analyst | Design lead, engineering lead |
| Users and flows | UX designer | Product manager, QA, engineering |
| Layout and style guide | Product designer | Frontend, design lead |
| Accessibility | UX designer, QA | Frontend, design lead |
| Scalability and edge cases | BA, engineering, QA | Product manager |
| Handoff | Design, frontend, backend | QA, delivery lead |
| Validation | QA, frontend | Design, product |
| Version control | Design lead or assigned design owner | Product, engineering |

## Quality Gate

- Every role has a goal and key task.
- Every task has at least one pipeline output that supports it.
- Permission-sensitive screens or actions are documented before screen specs.
- Ownership is clear for each artifact group.
