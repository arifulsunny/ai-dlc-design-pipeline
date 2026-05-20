# State Model

## Purpose

This file defines the states that must be considered for screens, flows, components, and design artifacts.

## Standard UI States

| State | Description | Required Design Detail |
|---|---|---|
| Default | Normal usable state | Primary layout, content, actions |
| Loading | Data or action in progress | Spinner, skeleton, progress, disabled controls |
| Empty | No data exists yet | Message, next action, permission-aware guidance |
| Error | Something failed | Error message, recovery action, retry behavior |
| Success | User action completed | Confirmation, next step, status update |
| Disabled | Action unavailable | Reason, requirement, tooltip or helper text |
| Permission restricted | User lacks access | Safe message, escalation path if applicable |
| Validation | User input is invalid or incomplete | Inline error, focus behavior, required field logic |
| Offline or degraded | Network or service problem | Fallback message and retry behavior |
| Conflict | Data changed elsewhere | Conflict notice, refresh or merge guidance |

## Pipeline Artifact States

| Artifact State | Meaning | Action |
|---|---|---|
| Draft | Generated or incomplete | Review before downstream use |
| Review needed | Ready for owner feedback | Assign reviewer and due point |
| Approved | Can be used for handoff | Mark status and version |
| Blocked | Missing source or decision | Add open question and owner |
| Superseded | Replaced by later design | Update version history and DDR |
| Released | Implemented and validated | Add release design notes |

## State Documentation Template

| Screen or Component | State | Trigger | UI Behavior | Backend/API Impact | Accessibility Note |
|---|---|---|---|---|---|
| TBD | Loading | Data fetch begins | Show skeleton | GET endpoint pending | Announce loading only when delay is meaningful |

## Quality Gate

- P0 screens and components include all relevant standard UI states.
- Permission and validation states are reviewed with backend and QA.
- State changes that alter user flow are reflected in the flow and handoff files.
