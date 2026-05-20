# Command: /design-context

## Purpose

Generate the design-ready context artifact from repository and external source inputs.

## Inputs

- `README.md`
- Main context file, if present
- Product requirements
- Business requirements
- User stories
- GitHub issues or PRs
- Existing frontend and backend files
- Existing design system files
- Previous `design/` artifacts

## Output File

`design/00-context/design-context.md`

## Required Sections

- Purpose
- Primary inputs
- Product summary
- Pipeline users
- Known product goals
- Core pipeline stages
- Design constraints
- Assumptions
- Open questions
- Source references, when multi-source
- Quality gate

## Quality Score Criteria

| Category | 5 Means |
|---|---|
| Requirement clarity | Product goal, users, constraints, and assumptions are explicit |
| Source traceability | Inputs are referenced with confidence levels when needed |
| Open questions | Missing information has owner and needed-before stage |
| Downstream usefulness | Design brief and user mapping can start from this file |

## Pass Threshold

- Lite: 3.5
- Standard: 4.0
- Full: 4.25

## Failure Re-Entry

If score is below threshold, return to source discovery and update open questions before generating downstream files.
