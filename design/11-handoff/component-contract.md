# Component Contract

## Purpose

This file defines the contract between design, frontend implementation, and design system reuse.

## Contract Requirements

Every shared or P0 component must define:

- Name
- Purpose
- Inputs or props
- Content rules
- Data dependencies
- States
- Events or callbacks
- Accessibility behavior
- Responsive behavior
- Design tokens
- Ownership and reuse status

## Component Contract Table

| Component | Purpose | Inputs | Events | States | Accessibility | Tokens | Reuse Status |
|---|---|---|---|---|---|---|---|
| Button | Trigger action | Variant, label, icon, disabled, loading | Click/submit | Default, hover, focus, disabled, loading | Accessible name, focus ring | Action, radius, space | Shared |
| Form input | Capture data | Label, value, required, error, helper | Change, blur | Default, focus, error, disabled | Label association, error association | Border, text, status | Shared |
| Table | Display records | Columns, rows, sort, filter, pagination | Sort, select, paginate | Loading, empty, error, default | Header semantics, keyboard support | Surface, border, text | Shared |
| Modal | Focused task | Title, content, actions, open state | Open, close, confirm | Open, loading, error | Focus trap, escape, restore focus | Surface, shadow, radius | Shared |

## Quality Gate

- Component contracts match screen specs and interaction specs.
- Shared components are reflected in reusable patterns or existing design system notes.
- Component changes that break behavior are recorded in design decision records.
