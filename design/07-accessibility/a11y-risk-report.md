# Accessibility Risk Report

## Purpose

This file records accessibility risks discovered during design and implementation review.

## Risk Matrix

| Risk ID | Area | Risk | Severity | Impact | Mitigation | Status |
|---|---|---|---|---|---|---|
| A11Y-001 | Keyboard | Missing focus order in complex flows | High | Keyboard users may be blocked | Define focus order in interaction spec | Open |
| A11Y-002 | Forms | Validation errors not tied to inputs | High | Screen reader users may miss errors | Require inline errors and `aria-describedby` equivalent | Open |
| A11Y-003 | Color | Token contrast not verified in all states | Medium | Low-vision users may struggle | Test semantic token pairs before release | Open |
| A11Y-004 | State changes | Loading/success/error not announced | Medium | Assistive tech users may lose context | Document announcement rules in state model | Open |
| A11Y-005 | Responsive | Tables may overflow on mobile | Medium | Mobile users may not read data | Provide responsive table behavior | Open |

## Risk Review Questions

- Can every primary task be completed without a mouse?
- Are destructive and irreversible actions clearly labeled and confirmed?
- Are empty, error, disabled, and permission states accessible?
- Do tokens support contrast in normal and disabled states?
- Does the implementation preserve headings, landmarks, labels, and focus order?

## Quality Gate

- High severity accessibility risks must be resolved or explicitly accepted before release.
- Mitigation must reference the affected artifact or implementation issue.
