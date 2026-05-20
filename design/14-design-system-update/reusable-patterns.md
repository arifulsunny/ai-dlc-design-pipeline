# Reusable Patterns

## Purpose

This file captures patterns that should be reused across future AI-DLC design work.

## Patterns

| Pattern | Use When | Includes | Notes |
|---|---|---|---|
| Stage-based design artifacts | A repo needs design before implementation | Context, brief, users, flow, UX, layout, handoff, validation | Core pattern of this repository |
| Quality gate per artifact | A file feeds implementation or review | Pass/fail readiness criteria | Helps humans and AI agents avoid incomplete handoff |
| Source reference block | Artifact uses multiple repos or files | Source list, scope, confidence, assumptions | Defined in `design/source-reference-instructions.md` |
| State model table | Screens have dynamic behavior | Trigger, UI response, API impact, accessibility | Reuse for every P0 feature |
| Change log plus DDR | Design changes affect implementation | What changed and why | Required for traceability |

## Pattern Template

| Pattern | Problem Solved | When to Use | When Not to Use | Related Files |
|---|---|---|---|---|
| TBD | TBD | TBD | TBD | TBD |

## Quality Gate

- Reusable patterns must be specific enough to apply in another project.
- Patterns that require implementation support must link to component contracts or handoff files.
