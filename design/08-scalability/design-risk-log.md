# Design Risk Log

## Purpose

This file tracks design risks across the pipeline so they can be owned, mitigated, accepted, or closed.

## Risk Log

| Risk ID | Risk | Impact | Likelihood | Severity | Owner | Mitigation | Status |
|---|---|---|---|---|---|---|---|
| DR-001 | Design starts without complete context | Wrong flows or screens | Medium | High | Product/Design | Complete context intake and open questions | Open |
| DR-002 | AI-generated docs become generic | Low implementation value | Medium | High | Design owner | Anchor artifacts to repo sources and user tasks | Open |
| DR-003 | Design changes are not versioned | Future agents use stale decisions | High | High | Design lead | Update change log, DDR, and version history | Open |
| DR-004 | Accessibility review is skipped | Users may be blocked | Medium | High | QA/Design | Require accessibility checklist before handoff | Open |
| DR-005 | Backend impact is missed | Flow cannot be implemented | Medium | High | Backend lead | Review state model and backend impact | Open |
| DR-006 | Design system drift | Inconsistent UI across features | Medium | Medium | Design system owner | Maintain update log and deprecated patterns | Open |

## Risk Status Values

- Open
- In review
- Mitigated
- Accepted
- Closed

## Quality Gate

- High severity open risks must be reviewed before implementation handoff.
- Accepted risks must include owner and rationale.
