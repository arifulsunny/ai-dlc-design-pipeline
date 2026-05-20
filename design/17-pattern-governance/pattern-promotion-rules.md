# Pattern Promotion Rules

## Purpose

This file defines when a feature-level design pattern should become a design-system-level pattern.

## Promotion Threshold

A pattern becomes a design system candidate when one or more are true:

- It appears independently in 3 or more features.
- It is required by 2 or more product teams.
- It solves a recurring accessibility, state, or layout problem.
- It replaces a deprecated pattern.
- It is required for implementation consistency across frontend surfaces.

## Promotion Workflow

```text
Feature-specific pattern
-> Candidate pattern log
-> Design lead review
-> Component contract or token update
-> Reusable pattern documentation
-> Design system update log
```

## Promotion Review Criteria

| Criteria | Required |
|---|---|
| Reuse evidence | Yes |
| Component or token contract | Yes |
| Accessibility behavior | Yes |
| Responsive behavior | Yes |
| Ownership | Yes |
| Migration notes | Required when replacing an existing pattern |

## Quality Gate

- A promoted pattern must be documented in `14-design-system-update/reusable-patterns.md`.
- A promoted component must update `11-handoff/component-contract.md` or the owning design system contract.
