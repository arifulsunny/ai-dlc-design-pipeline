# Command: /accessibility-review

## Purpose

Review design artifacts for accessibility readiness before handoff and after implementation.

## Inputs

- `design/04-ux/state-model.md`
- `design/05-layout/screen-specs.md`
- `design/05-layout/component-map.md`
- `design/06-style-guide/design-tokens.json`
- `design/09-prototype/interaction-spec.md`
- Implemented UI or screenshots, when available

## Output Files

- `design/07-accessibility/accessibility-checklist.md`
- `design/07-accessibility/a11y-risk-report.md`

## Required Sections

- Keyboard review
- Screen reader review
- Contrast review
- Form and validation review
- Focus management review
- Motion and responsive review
- Risk matrix
- Mitigation plan
- Source references, when multi-source
- Quality gate

## Quality Score Criteria

| Category | 5 Means |
|---|---|
| Keyboard support | Primary tasks can be completed without mouse |
| Screen reader support | Labels, errors, status changes, and headings are clear |
| Visual accessibility | Contrast, focus, responsive behavior are acceptable |
| Risk mitigation | High risks have owners and fixes |

## Pass Threshold

- Lite: 3.5 when no accessibility-sensitive behavior changed
- Standard: 4.0
- Full: 4.25

## Failure Re-Entry

If score is below threshold, return to screen specs, interaction spec, component contract, or implementation audit.
