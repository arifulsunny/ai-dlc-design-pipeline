# Pattern Deprecation Rules

## Purpose

This file defines when a pattern should be deprecated and how teams should migrate away from it.

## Deprecation Triggers

| Trigger | Example | Required Action |
|---|---|---|
| Accessibility risk | Pattern blocks keyboard or screen reader users | Deprecate and define replacement |
| Implementation inconsistency | Same pattern behaves differently across screens | Replace with component contract |
| Low usability | User testing or QA finds recurring confusion | Redesign and document migration |
| Design system replacement | New token/component supersedes old pattern | Mark old pattern deprecated |
| AI generation risk | Pattern causes repeated wrong outputs | Add to deprecated patterns and command guidance |

## Deprecation Workflow

```text
Identify risky pattern
-> Add to deprecated patterns
-> Define replacement
-> Update command specs if AI agents may reuse it
-> Add migration notes
-> Track in release design notes when user-facing
```

## Quality Gate

- No deprecated pattern can be used in a new P0 screen without Accountable owner approval.
- Every deprecated pattern must have a replacement or explicit removal plan.
