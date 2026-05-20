# Command: /design-brief

## Purpose

Convert requirements and context into a UX-ready design brief.

## Inputs

- `design/00-context/design-context.md`
- Product requirements
- Business requirements
- User stories
- GitHub issues or PRs
- API constraints
- Existing design documentation

## Output File

`design/01-requirements/design-brief.md`

## Required Sections

- Purpose
- Source inputs
- Problem statement
- Target users
- User goals
- Business goals
- Functional requirements
- Non-functional requirements
- Key user scenarios
- UX risks
- Accessibility risks
- Success metrics
- Source references, when multi-source
- Quality gate

## Quality Score Criteria

| Category | 5 Means |
|---|---|
| Requirement clarity | Every requirement maps to a task, behavior, rule, or validation need |
| User value | User goals and scenarios are specific |
| Business value | Business goals and success metrics are measurable |
| Risk visibility | UX and accessibility risks are concrete |

## Pass Threshold

- Standard: 4.0
- Full: 4.25

## Failure Re-Entry

If score is below threshold, return to requirements, source references, or open questions before creating flows.
