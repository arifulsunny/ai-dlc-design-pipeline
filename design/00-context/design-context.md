# Design Context

## Purpose

This file is the first design artifact in the AI-DLC design pipeline. It turns a GitHub repository, product context, requirements, existing UI, backend constraints, and previous design documentation into a design-ready source of truth.

No design brief, user flow, layout specification, or implementation handoff should start until this file is complete enough for product, design, frontend, backend, QA, and AI agents to share the same understanding.

## Primary Inputs

Use the most relevant available sources:

- `README.md`
- Main context file, such as `main-context.md`
- Product requirements
- Business requirements
- User stories
- GitHub issues and pull requests
- API specifications
- Existing frontend code
- Existing backend code or service contracts
- Existing UI screenshots or Figma files
- Existing design system documentation
- Previous files under `design/`

When content is generated from multiple repos, branches, documents, or external file sources, follow `design/source-reference-instructions.md`.

## Product Summary

AI-DLC Design Pipeline is a repo-native design process for AI-DLC and agentic software development. It introduces a formal design layer between requirement analysis and frontend/backend implementation so teams can avoid unclear flows, missing UX decisions, weak accessibility coverage, incomplete handoff, and undocumented design changes.

## Pipeline Users

| Role | Primary Need | Design Context Required |
|---|---|---|
| Product manager | Align business goals and scope | Product purpose, success metrics, risks |
| Business analyst | Convert requirements into usable scenarios | Requirements, rules, edge cases |
| UX designer | Define flows, interaction, and usability | User roles, tasks, states, constraints |
| Product designer | Create layouts and visual systems | Screen inventory, design tokens, components |
| Frontend engineer | Build consistent UI | Screen specs, component map, states, accessibility |
| Backend engineer | Support workflows and data needs | API impact, validation rules, permissions |
| QA engineer | Validate behavior and coverage | Acceptance criteria, edge cases, audit checklist |
| AI agent | Generate or review artifacts | Clear inputs, outputs, assumptions, and quality gates |

## Known Product Goals

- Make design a formal part of AI-DLC.
- Keep design documentation inside the repository.
- Create structured artifacts that agents and humans can consume.
- Ensure every feature has context, user flow, layout, accessibility, scalability, handoff, validation, and version history.
- Improve traceability from requirement to design decision to implementation.

## Core Pipeline Stages

1. Design context intake
2. Requirement to design brief
3. User role and task mapping
4. User flow and information architecture
5. UX strategy and interaction model
6. Screen specs and layout planning
7. Style guide and design system mapping
8. Accessibility review
9. Scalability and edge case review
10. Prototype or Figma documentation
11. Multi-agent design review
12. Frontend and backend handoff
13. Implementation validation
14. Design documentation and version control
15. Design system update

## Design Constraints

- All core design artifacts must live in `design/`.
- Artifacts must be readable in GitHub without requiring a design tool.
- Mermaid should be used for flow diagrams when possible.
- Markdown tables should be used for role, task, screen, risk, and audit matrices.
- Design tokens must be machine-readable JSON.
- Every major design change must update version-control artifacts.

## Assumptions

- The repository may start without a dedicated design process.
- The main source of truth is the GitHub repo plus any linked product or design sources.
- Claude or another AI agent may generate first drafts, but humans must review quality gates.
- Design handoff should support both human engineers and implementation agents.

## Open Questions Template

| Question | Owner | Needed Before | Status |
|---|---|---|---|
| What is the primary product or feature being designed? | Product | Design brief | Open |
| Which user roles are in scope for this change? | Product/BA | User role matrix | Open |
| Are there existing UI patterns or design tokens to reuse? | Design/Frontend | Style guide | Open |
| Which backend APIs or data models constrain the flow? | Backend | Handoff | Open |
| What accessibility standard is required? | Design/QA | Accessibility review | Open |

## Quality Gate

Design context is ready when these items are true:

- Product purpose is documented.
- Primary users and tasks are identified.
- Technical constraints are listed.
- Existing UI and design system inputs are referenced.
- Missing information is captured as open questions.
- Source references are documented when multiple files or repos informed the artifact.
