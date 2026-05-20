# Accessibility Checklist

## Purpose

This checklist must be used before frontend handoff and again during implementation validation.

## Checklist

| Area | Check | Status | Notes |
|---|---|---|---|
| Keyboard | All interactive controls can be reached by keyboard | Not started |  |
| Keyboard | Focus order follows visual and task order | Not started |  |
| Keyboard | Focus is trapped in modals and restored on close | Not started |  |
| Screen reader | Controls have accessible names | Not started |  |
| Screen reader | Status changes are announced when needed | Not started |  |
| Screen reader | Error messages are associated with fields | Not started |  |
| Contrast | Text meets required contrast ratio | Not started |  |
| Contrast | Focus indicators are visible | Not started |  |
| Forms | Required fields are programmatically identified | Not started |  |
| Forms | Validation is clear and recoverable | Not started |  |
| Navigation | Current page or active section is indicated | Not started |  |
| Navigation | Skip or landmark navigation is available where needed | Not started |  |
| Content | Headings follow logical order | Not started |  |
| Content | Link text is descriptive | Not started |  |
| Motion | Motion respects reduced-motion preference | Not started |  |
| Responsive | Content reflows without overlap | Not started |  |
| Error handling | Errors explain recovery steps | Not started |  |
| Permission states | Restricted content is communicated safely | Not started |  |

## Required Evidence

- Link to screen specs reviewed.
- Link to component contract reviewed.
- Link to implementation audit after build.
- Notes for any exception or deferred item.

## Quality Gate

- No P0 screen is approved for handoff with unresolved critical accessibility risks.
- Any deferred accessibility item has an owner, reason, and follow-up date.
