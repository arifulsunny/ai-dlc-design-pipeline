# Interaction Model

## Purpose

This file defines how users, reviewers, and AI agents interact with the design pipeline.

## Interaction Patterns

| Pattern | Where Used | Expected Behavior |
|---|---|---|
| Intake | Context and requirements | Gather sources, list assumptions, identify gaps |
| Mapping | Users, tasks, components, risks | Convert inputs into structured tables |
| Sequencing | Flow and navigation | Define order, entry points, decisions, exits |
| Specification | Layout, UX, style, handoff | Turn decisions into implementation-ready requirements |
| Review | Accessibility, design review, validation | Evaluate artifacts against explicit criteria |
| Versioning | Change log, DDRs, version history | Capture what changed, why, impact, and rollback notes |
| System feedback | Design system updates | Convert project-specific learning into reusable guidance |

## AI Agent Interaction Rules

- Read upstream artifacts before generating downstream files.
- State assumptions in the artifact when source data is incomplete.
- Do not overwrite a prior decision without creating or updating a design decision record.
- When generating from multiple sources, update the source reference section required by `design/source-reference-instructions.md`.
- Preserve file paths and source names so reviewers can trace outputs.

## Human Review Interaction Rules

| Review Moment | Required Action |
|---|---|
| After context intake | Confirm product goal, users, and missing inputs |
| After design brief | Approve scope, risks, and success metrics |
| After flows | Validate task sequence and exception cases |
| After layout and style | Confirm screens, components, responsive behavior, and visual rules |
| Before handoff | Confirm accessibility, scalability, and risk gates |
| After implementation | Audit UI and update version-control docs |

## Feedback Model

| Feedback Type | Use When | Document In |
|---|---|---|
| Inline correction | Small wording or requirement fix | Affected file |
| Design change | Flow, screen, interaction, or component changes | Change log and DDR |
| Release note | User-visible design change | Release design notes |
| System update | Reusable or deprecated pattern | Design system update files |

## Quality Gate

- Every interaction has a clear owner and output.
- AI-generated updates are traceable to source artifacts.
- Review feedback is captured in the correct downstream file.
