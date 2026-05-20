# Backend Impact

## Purpose

This file documents backend, API, permission, validation, and data implications of design decisions.

## Backend Impact Areas

| Area | Design Question | Backend Review Needed |
|---|---|---|
| Authentication | Does the flow require login or role detection? | Auth state and redirects |
| Authorization | Which roles can view or act? | Permission rules and response codes |
| Data loading | What data does each screen need? | API endpoints, pagination, caching |
| Validation | What input rules exist? | Server-side validation and error shape |
| State transitions | What user actions change status? | State machine or workflow rules |
| Error handling | What failures can occur? | Error contracts and retry behavior |
| Auditability | Are changes logged? | Audit events and metadata |
| Notifications | Are users informed after changes? | Email, in-app, webhook, or event triggers |

## Impact Matrix

| Flow or Screen | Backend Need | API or Service | Validation | Permission | Status |
|---|---|---|---|---|---|
| TBD | TBD | TBD | TBD | TBD | Not started |

## Error Contract Template

| Error Type | User Message Need | API Shape | UI Behavior |
|---|---|---|---|
| Validation | Field-level message | Field error map | Focus invalid field or summary |
| Permission | Safe restriction message | 403 or equivalent | Show restricted state |
| Not found | Explain missing or removed item | 404 or equivalent | Show not-found state |
| Server error | Recovery and retry | 5xx or equivalent | Show retryable error |

## Quality Gate

- Backend impact is reviewed before frontend implementation begins.
- Permission, validation, and error shapes are aligned with interaction and state models.
