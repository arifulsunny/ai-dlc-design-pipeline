# Pipeline Usage Levels

## Purpose

This file defines how much of the design pipeline must be used for a given change. The goal is to keep the pipeline useful without making small changes bureaucratic.

## Usage Levels

| Level | Use For | Required Files | Minimum Score |
|---|---|---|---:|
| Lite | Copy changes, small visual fixes, simple component tweaks | `13-version-control/design-change-log.md`, `11-handoff/acceptance-criteria.md` | 3.5 |
| Standard | New screen, normal feature, workflow update | Context, brief, users, flow, screen specs, accessibility, handoff, validation, change log | 4.0 |
| Full | New product area, major redesign, high-risk workflow, permission-heavy feature | All pipeline stages, RACI, re-entry triggers, command specs, review, versioning, pattern governance | 4.25 |

## Level Selection Checklist

| Question | If Yes |
|---|---|
| Does the change affect user flow? | Use Standard or Full |
| Does the change affect permissions, APIs, or state transitions? | Use Standard or Full |
| Does the change introduce a new reusable pattern? | Use Standard or Full |
| Does the change affect accessibility risk? | Use Standard or Full |
| Does the change affect multiple teams or agents? | Use Full |
| Is the change only copy, spacing, or a local visual adjustment? | Use Lite |

## Required Sections Per Level

| Section | Lite | Standard | Full |
|---|---:|---:|---:|
| Source references | Required when multi-source | Required | Required |
| Acceptance criteria | Required | Required | Required |
| Design readiness score | Required | Required | Required |
| Re-entry triggers | Optional | Required when impacted | Required |
| RACI ownership | Optional | Recommended | Required |
| Claude command specs | Optional | Required for AI-generated artifacts | Required |
| Pattern promotion review | Optional | Required when reusable | Required |

## Quality Score

Use `design/15-operating-model/design-readiness-score.md`.

If the score is below the minimum for the selected level:

1. Mark the design as `Blocked`.
2. Identify the lowest-scoring category.
3. Return to the earliest affected artifact.
4. Update change log if the design meaning changes.

## Quality Gate

- Every change selects a usage level before artifact generation starts.
- The selected level determines required files and minimum score.
- A reviewer can challenge the selected level if risk is underestimated.
