# Design Decision Records

## Purpose

This file records important design decisions so future humans and AI agents know why the design changed.

## Decision Records

### DDR-001: Use repo-native design artifacts

Date: 2026-05-21
Status: Accepted

Context:

AI-DLC and agentic development workflows need design context that is available to coding agents and engineering teams directly inside the repository.

Decision:

Use Markdown, JSON, and Mermaid files under `design/` as the primary design artifact structure.

Reason:

Repo-native artifacts are easy to review in GitHub, version in Git, reference from AI agents, and connect to implementation pull requests.

Alternatives considered:

1. Keep design only in Figma.
2. Keep design only in product documents.
3. Generate one large design document.

Impact:

The pipeline is split into stage-specific files so each artifact can be reviewed, updated, and referenced independently.

Related files:

- `README.md`
- `design/00-context/design-context.md`
- `design/13-version-control/design-change-log.md`

## New Decision Template

```text
Decision ID:
Title:
Date:
Status: Proposed | Accepted | Rejected | Superseded

Context:

Decision:

Reason:

Alternatives considered:

Impact:

Accessibility impact:

Engineering impact:

Related files:

Related issue or PR:
```

## Quality Gate

- Major UX, flow, layout, accessibility, or design system decisions are recorded here.
- Superseded decisions link to the replacement decision.
