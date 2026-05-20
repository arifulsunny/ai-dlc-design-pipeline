# Component Usage Guidelines

## Purpose

This file defines how components should be selected, reused, documented, and updated in the AI-DLC design pipeline.

## Component Selection Rules

| Situation | Rule |
|---|---|
| Existing component fits | Reuse it and document any state or content differences |
| Existing component almost fits | Extend only if the variant will be reused |
| New feature needs new UI | Add proposed component to component map and design system update log |
| One-off interaction | Document as a one-off and explain why reuse is not appropriate |
| Component is harmful or outdated | Add it to deprecated patterns |

## Required Component Documentation

For every component used in a P0 screen, document:

- Purpose
- Inputs or props
- Data source
- User actions
- States
- Accessibility behavior
- Responsive behavior
- Ownership

## Do and Do Not

| Do | Do Not |
|---|---|
| Use semantic component names | Name components by visual appearance only |
| Specify all relevant states | Assume frontend will infer error or empty states |
| Reuse design tokens | Introduce untracked colors or spacing |
| Document accessibility behavior | Treat accessibility as QA-only work |
| Update design system notes | Let reusable patterns stay hidden in one feature |

## Quality Gate

- Component usage matches the component map.
- New reusable components are captured in `14-design-system-update/reusable-patterns.md`.
- Deprecated or replaced patterns are captured in `14-design-system-update/deprecated-patterns.md`.
