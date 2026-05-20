# Navigation Map

## Purpose

This file maps the information architecture of the design pipeline repository. It helps humans and agents find the correct artifact at the correct stage.

## Repository Navigation

| Area | Path | Purpose | Depends On |
|---|---|---|---|
| Context | `design/00-context/` | Product and source understanding | Repo and source files |
| Requirements | `design/01-requirements/` | UX-ready brief | Context |
| Users | `design/02-users/` | Role, permission, task priority | Context, requirements |
| Flow | `design/03-flow/` | User journey and IA | Users, requirements |
| UX | `design/04-ux/` | Principles, interactions, states | Flow |
| Layout | `design/05-layout/` | Screen and component structure | UX, flow |
| Style guide | `design/06-style-guide/` | Visual rules and tokens | Layout, design system |
| Accessibility | `design/07-accessibility/` | Checklist and risks | UX, layout, style |
| Scalability | `design/08-scalability/` | Edge cases and risks | Requirements, flow, backend |
| Prototype | `design/09-prototype/` | Prototype notes and interactions | Layout, UX |
| Review | `design/10-review/` | Multi-agent or human review | All prior artifacts |
| Handoff | `design/11-handoff/` | Engineering contracts | Reviewed design |
| Validation | `design/12-validation/` | Implementation audit | Implemented UI |
| Version control | `design/13-version-control/` | Change history and decisions | Any design change |
| Design system update | `design/14-design-system-update/` | Reusable pattern feedback | Finalized design |

## Artifact Dependency Order

```text
00-context
-> 01-requirements
-> 02-users
-> 03-flow
-> 04-ux
-> 05-layout
-> 06-style-guide
-> 07-accessibility
-> 08-scalability
-> 09-prototype
-> 10-review
-> 11-handoff
-> 12-validation
-> 13-version-control
-> 14-design-system-update
```

## Review Navigation

| Reviewer | Start With | Then Check |
|---|---|---|
| Product | Design brief | Task map, review report, release notes |
| UX | User flow | Interaction model, state model, screen specs |
| Frontend | Screen specs | Component map, tokens, frontend handoff |
| Backend | State model | Backend impact, acceptance criteria |
| QA | Acceptance criteria | Accessibility checklist, audit, edge cases |
| AI agent | Context | Source-reference instructions, related files |

## Quality Gate

- Each artifact points to upstream inputs and downstream consumers.
- Reviewers can find the files they need without private context.
- Navigation stays current when new pipeline files are added.
