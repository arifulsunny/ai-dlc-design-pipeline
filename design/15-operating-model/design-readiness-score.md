# Design Readiness Score

## Purpose

This file defines a measurable score for deciding whether a design is ready for handoff, implementation, or release.

## Score Scale

| Score | Meaning |
|---:|---|
| 1 | Missing or unusable |
| 2 | Incomplete and risky |
| 3 | Usable with major gaps |
| 4 | Ready with minor gaps |
| 5 | Strong, clear, implementation-ready |

## Score Categories

| Category | What To Check | Score |
|---|---|---:|
| Requirement clarity | Problem, goals, users, constraints, assumptions | TBD |
| User flow quality | Primary, secondary, error, empty, and permission flows | TBD |
| Interaction and state quality | Loading, empty, error, success, disabled, validation, permission states | TBD |
| Layout and component clarity | Screen specs, responsive behavior, component map | TBD |
| Accessibility readiness | Checklist, risk report, keyboard, screen reader, contrast, focus | TBD |
| Backend and API alignment | Permissions, validation, data needs, error contracts | TBD |
| Handoff quality | Frontend, backend, component contract, acceptance criteria | TBD |
| Version and traceability | Change log, DDR, version history, source references | TBD |
| Pattern governance | Reusable, deprecated, or candidate patterns reviewed | TBD |

## Final Score Formula

```text
Final score = average of all applicable category scores
```

For high-risk work, requirement clarity, accessibility readiness, backend/API alignment, and handoff quality must each be at least `4`, even if the average is higher.

## Blocking Thresholds

| Pipeline Level | Blocking Threshold |
|---|---:|
| Lite | Below 3.5 |
| Standard | Below 4.0 |
| Full | Below 4.25 |

## Score Record Template

| Date | Change | Pipeline Level | Final Score | Decision | Reviewer |
|---|---|---|---:|---|---|
| TBD | TBD | Lite/Standard/Full | TBD | Pass/Blocked | TBD |

## Failure Handling

| Failed Category | Re-enter Stage |
|---|---|
| Requirement clarity | `01-requirements/design-brief.md` |
| User flow quality | `03-flow/user-flow.md` |
| Interaction and state quality | `04-ux/interaction-model.md`, `04-ux/state-model.md` |
| Layout and component clarity | `05-layout/screen-specs.md`, `05-layout/component-map.md` |
| Accessibility readiness | `07-accessibility/accessibility-checklist.md`, `07-accessibility/a11y-risk-report.md` |
| Backend and API alignment | `11-handoff/backend-impact.md` |
| Handoff quality | `11-handoff/` |
| Version and traceability | `13-version-control/` |
| Pattern governance | `17-pattern-governance/`, `14-design-system-update/` |

## Quality Gate

- The design cannot move to handoff when the final score is below the selected pipeline level threshold.
- Any category below `3` must be fixed before release.
