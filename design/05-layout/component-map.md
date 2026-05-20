# Component Map

## Purpose

This file maps required UI and documentation components to their purpose, usage rules, and design system status.

## Core Product Components

| Component | Purpose | Common States | Design System Status |
|---|---|---|---|
| App shell | Main navigation and content frame | Default, collapsed, mobile drawer | Required |
| Header | Screen title, context, primary action | Default, sticky, compact | Required |
| Button | Trigger actions | Default, hover, focus, disabled, loading | Required |
| Form input | Capture user data | Default, focus, error, disabled, required | Required |
| Select/menu | Choose from options | Default, open, selected, disabled | Required |
| Table | Display structured records | Loading, empty, sorted, filtered, error | Required |
| Card | Group related content | Default, interactive, selected | Optional |
| Modal/dialog | Focused task or confirmation | Open, loading, destructive, dismissible | Required |
| Toast/alert | Feedback and notices | Success, warning, error, info | Required |
| Badge/status | Show state or category | Neutral, success, warning, error | Required |
| Tabs | Switch related views | Active, inactive, disabled | Optional |
| Stepper/progress | Multi-step flow | Current, complete, error | Optional |
| Empty state | Explain missing data | Default, permission, filtered | Required |
| Error state | Recovery from failure | Retryable, fatal, validation | Required |

## Pipeline Documentation Components

| Component | Used In | Purpose |
|---|---|---|
| Source reference block | All generated files when multi-source | Trace source inputs |
| Quality gate checklist | All stage files | Define pass/fail readiness |
| Risk table | Brief, accessibility, scalability, review | Capture impact and mitigation |
| Decision record | Version control | Preserve why decisions changed |
| Acceptance criteria list | Handoff, validation | Make QA and implementation testable |
| Mermaid diagram | Flow | Keep diagrams repo-native |

## Component Contract Template

| Component | Props or Inputs | Output Behavior | Accessibility Requirements | Owner |
|---|---|---|---|---|
| TBD | TBD | TBD | TBD | TBD |

## Quality Gate

- Every P0 screen maps to components.
- New components are either added to the design system update log or marked as one-off.
- Component states match the state model.
