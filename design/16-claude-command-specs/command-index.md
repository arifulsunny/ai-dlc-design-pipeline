# Claude Command Specs

## Purpose

This folder defines practical Claude command contracts. Each command specifies inputs, output file, required sections, and quality score criteria.

## Command List

| Command | Purpose | Output File |
|---|---|---|
| `/design-context` | Extract design-ready context from repo and sources | `design/00-context/design-context.md` |
| `/design-brief` | Convert requirements into UX-ready brief | `design/01-requirements/design-brief.md` |
| `/user-flow` | Generate user flow, navigation map, inventory, Mermaid diagram | `design/03-flow/` |
| `/screen-spec` | Generate implementation-ready screen specs | `design/05-layout/screen-specs.md` |
| `/accessibility-review` | Review accessibility checklist and risks | `design/07-accessibility/` |
| `/handoff` | Generate frontend/backend/component/acceptance handoff | `design/11-handoff/` |
| `/design-review` | Run design review and readiness scoring | `design/10-review/design-review-report.md` |

## Global Command Rules

- Read upstream files before generating downstream files.
- Add source references when using multiple files or external sources.
- Include assumptions and open questions.
- Output must update the target file, not only print a response.
- Apply `design/15-operating-model/design-readiness-score.md`.

## Quality Gate

- Each command output includes enough structure for review.
- Scores below threshold must return a re-entry recommendation.
