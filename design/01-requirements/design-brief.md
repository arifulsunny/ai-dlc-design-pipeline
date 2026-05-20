# Design Brief

## Purpose

This file converts product and business requirements into a UX-ready design brief. It should explain what problem the design must solve before any screens are specified.

## Source Inputs

- `design/00-context/design-context.md`
- Product requirements
- Business requirements
- User stories
- GitHub issues
- API constraints
- Existing design documentation

## Problem Statement

AI-DLC and agentic development workflows often move directly from requirement analysis to frontend and backend implementation. Without a design pipeline, teams risk building fast but with incomplete user flows, unclear UX decisions, inconsistent layouts, weak accessibility, and missing design traceability.

This design pipeline solves that gap by turning repository context into structured design artifacts that are reviewable, versioned, and useful for both people and AI agents.

## Target Users

| User | Goal | Need From This Pipeline |
|---|---|---|
| Product manager | Control product scope and outcomes | Clear design brief, success metrics, risks |
| Business analyst | Preserve requirement intent | Requirement-to-task mapping |
| UX/product designer | Design coherent experiences | Flow, UX principles, layout specs |
| Frontend engineer | Implement UI reliably | Screen specs, component contracts, tokens |
| Backend engineer | Support feature behavior | API impact and validation notes |
| QA engineer | Verify user-facing quality | Acceptance criteria and audit checklist |
| AI coding agent | Generate implementation safely | Structured, referenced, current design artifacts |

## User Goals

- Understand what must be designed before implementation starts.
- Convert requirements into role-specific tasks and flows.
- Reduce ambiguity for frontend and backend work.
- Preserve design decisions after every change.
- Keep artifacts close to the codebase.

## Business Goals

- Improve delivery quality in AI-DLC workflows.
- Reduce rework caused by missing design decisions.
- Make design traceable through Git history.
- Support cross-functional collaboration across product, design, engineering, QA, and AI agents.
- Reuse design patterns across future projects.

## Functional Requirements

| Requirement | Design Implication | Output Artifact |
|---|---|---|
| Analyze repo context | Extract users, tasks, constraints, UI patterns | `00-context/design-context.md` |
| Map roles and tasks | Identify permissions and priorities | `02-users/*.md` |
| Define flows | Show primary, secondary, error, and empty flows | `03-flow/*.md` |
| Specify UX behavior | Document interaction, states, feedback | `04-ux/*.md` |
| Specify screens | Describe layout and component needs | `05-layout/*.md` |
| Define style rules | Capture tokens and component usage | `06-style-guide/*.md` |
| Review accessibility | Identify checklist and risks | `07-accessibility/*.md` |
| Plan scalability | Capture edge cases and design risks | `08-scalability/*.md` |
| Prepare handoff | Align frontend and backend expectations | `11-handoff/*.md` |
| Validate implementation | Audit final UI against design | `12-validation/*.md` |
| Version design | Track changes, decisions, and releases | `13-version-control/*.md` |

## Non-Functional Requirements

- Documentation must be readable in Markdown.
- Diagrams must be text-based where possible.
- Artifacts must be stable enough for AI agents to reference.
- Each stage must include quality gates.
- Design changes must be traceable to issues, PRs, decisions, and affected files.
- Accessibility and scalability must be considered before implementation handoff.

## Key User Scenarios

1. A product manager adds a new feature requirement and needs design artifacts before engineering starts.
2. A Claude or Codex agent reads repo context and generates a UX brief, flows, and handoff docs.
3. A frontend engineer implements a screen using the screen specs, component map, design tokens, and interaction model.
4. A backend engineer checks API and validation impact from the backend handoff document.
5. QA validates the delivered UI against acceptance criteria and design implementation audit.
6. A later design change updates the change log, decision record, version history, and release design notes.

## UX Risks

| Risk | Impact | Mitigation |
|---|---|---|
| Requirements are vague | Screens solve the wrong problem | Require open questions before design starts |
| AI generates generic UI | Product-specific workflows are lost | Anchor outputs to repo context and user tasks |
| Flow gaps appear late | Implementation rework | Require user-flow review before layout |
| Design changes are undocumented | Future agents use stale assumptions | Require version-control updates |

## Accessibility Risks

| Risk | Impact | Mitigation |
|---|---|---|
| Accessibility reviewed too late | Expensive UI rework | Include checklist before handoff |
| States are undocumented | Screen reader and keyboard gaps | Use state model and interaction spec |
| Design tokens lack contrast rules | Inconsistent readability | Define semantic color tokens and contrast notes |

## Success Metrics

- Every feature has a design brief before implementation.
- Every screen maps to a user role and task.
- Every major flow has a Mermaid or Markdown flow artifact.
- Every handoff includes frontend, backend, component, and acceptance criteria.
- Every design change updates version-control files.
- QA can validate design implementation without asking for missing context.

## Quality Gate

The design brief is ready when:

- Problem, users, goals, requirements, risks, and success metrics are documented.
- Each requirement maps to a user task, business rule, system behavior, or validation rule.
- Open questions are captured with owners.
- Related source files are referenced when applicable.
