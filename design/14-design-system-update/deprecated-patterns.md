# Deprecated Patterns

## Purpose

This file records patterns that should no longer be used in the design pipeline or product UI.

## Deprecated Patterns

| Pattern | Reason | Replacement | Status |
|---|---|---|---|
| Designing screens before context intake | Leads to generic or incorrect UI | Complete `00-context` and `01-requirements` first | Deprecated |
| Handoff without state documentation | Causes missing loading, error, empty, and permission behavior | Use `04-ux/state-model.md` and `09-prototype/interaction-spec.md` | Deprecated |
| Accessibility only after implementation | Creates late rework and user risk | Use checklist before handoff and during audit | Deprecated |
| Unversioned design changes | Future agents and teams lose rationale | Update change log, DDR, version history, and release notes | Deprecated |
| Unreferenced multi-source generation | Cannot trace source truth | Use source-reference instructions | Deprecated |

## Deprecation Template

| Pattern | Deprecated Date | Reason | Replacement | Migration Notes |
|---|---|---|---|---|
| TBD | TBD | TBD | TBD | TBD |

## Quality Gate

- Deprecated patterns must include a replacement.
- Active files must not recommend deprecated patterns.
