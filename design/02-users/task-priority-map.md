# Task Priority Map

## Purpose

This file ranks user and team tasks so the design pipeline focuses first on the work that has the highest product, usability, and implementation impact.

## Priority Levels

| Priority | Meaning | Design Action |
|---|---|---|
| P0 | Must exist for any useful implementation | Block handoff until documented |
| P1 | Important for launch quality | Complete before implementation starts |
| P2 | Useful for polish or future iteration | Capture for backlog or later design pass |

## Pipeline Task Map

| Task | Primary Role | Priority | Why It Matters | Required Artifact |
|---|---|---:|---|---|
| Extract product purpose and constraints | AI agent, product manager | P0 | Prevents generic or wrong design outputs | `00-context/design-context.md` |
| Convert requirements into UX brief | BA, product manager | P0 | Creates design-ready problem framing | `01-requirements/design-brief.md` |
| Identify roles and permissions | BA, UX designer | P0 | Prevents screens without users or access rules | `02-users/user-role-matrix.md` |
| Prioritize tasks | Product manager, UX designer | P0 | Guides screen and flow priority | `02-users/task-priority-map.md` |
| Define primary and exception flows | UX designer | P0 | Reduces implementation ambiguity | `03-flow/user-flow.md` |
| Build navigation map | UX designer, frontend | P1 | Aligns routing and information architecture | `03-flow/navigation-map.md` |
| Inventory screens | Product designer, frontend | P0 | Defines implementation scope | `03-flow/screen-inventory.md` |
| Define interaction and state behavior | UX designer | P0 | Prevents missing loading, error, empty, and success states | `04-ux/*.md` |
| Specify screen layouts | Product designer | P0 | Gives frontend a buildable target | `05-layout/screen-specs.md` |
| Define responsive rules | Product designer, frontend | P1 | Prevents layout breakage across viewports | `05-layout/responsive-layout-rules.md` |
| Map components | Product designer, frontend | P0 | Promotes reuse and design system alignment | `05-layout/component-map.md` |
| Define style guide and tokens | Product designer | P1 | Keeps UI consistent | `06-style-guide/*.md` |
| Complete accessibility review | UX designer, QA | P0 | Reduces compliance and usability risk | `07-accessibility/*.md` |
| Capture scalability and edge cases | BA, engineering, QA | P1 | Reduces production surprises | `08-scalability/*.md` |
| Document prototype behavior | Designer | P2 | Helps stakeholders review realistic behavior | `09-prototype/*.md` |
| Run multi-agent design review | Design lead, AI agents | P1 | Finds gaps before implementation | `10-review/design-review-report.md` |
| Prepare frontend/backend handoff | Design, frontend, backend | P0 | Enables implementation | `11-handoff/*.md` |
| Validate implementation | QA, design, frontend | P0 | Confirms delivered UI matches design | `12-validation/design-implementation-audit.md` |
| Update design version control | Design owner | P0 | Preserves design traceability | `13-version-control/*.md` |
| Update design system notes | Design lead | P1 | Feeds reusable improvements back into the system | `14-design-system-update/*.md` |

## Quality Gate

- All P0 tasks must be complete before implementation handoff.
- P1 tasks must be complete before release unless explicitly deferred.
- P2 tasks must be documented so they are not lost.
