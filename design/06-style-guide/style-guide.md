# Style Guide

## Purpose

This file defines visual and writing rules for pipeline-generated design documentation and product UI specifications.

## Visual Direction

The design pipeline should support clear, professional, engineering-friendly product interfaces. It should favor usability, clarity, accessibility, and consistency over decorative styling.

## Design Qualities

| Quality | Rule |
|---|---|
| Clear | Users should understand what to do next |
| Consistent | Patterns and tokens should repeat across screens |
| Accessible | Contrast, keyboard use, focus, and labels are required |
| Scalable | Layout and components should handle growth |
| Traceable | Design decisions should link back to source and version files |

## Typography

| Use | Guidance |
|---|---|
| Page title | Clear feature or screen name |
| Section title | Short and task-oriented |
| Body text | Direct, plain language |
| Helper text | Explain requirement, validation, or next step |
| Error text | State what happened and how to recover |

## Color Usage

Use semantic color roles instead of hard-coded intent:

- Primary: main actions and active states
- Secondary: supporting actions
- Surface: page and panel backgrounds
- Border: separation and structure
- Text: primary and secondary content
- Success: completed actions
- Warning: risky or attention-needed states
- Error: failed or destructive states
- Info: neutral guidance

## Spacing and Density

- Use consistent spacing steps from `design-tokens.json`.
- Dense operational screens may use compact spacing, but readability must remain intact.
- Do not use nested cards for page sections.
- Group related content through headings, spacing, and clear hierarchy.

## Content Style

- Prefer active voice.
- Use specific role and task names.
- Avoid vague phrases such as "improve UX" without explaining how.
- Write acceptance criteria as testable statements.
- When uncertain, write assumptions and open questions.

## Quality Gate

- Visual decisions map to tokens or reusable rules.
- Text is specific enough for implementation and QA.
- Accessibility and state language are included for risky interactions.
