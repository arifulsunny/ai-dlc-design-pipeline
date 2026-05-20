# UX Principles

## Purpose

This file defines the behavior and experience principles that every design pipeline artifact should follow.

## Principles

| Principle | Meaning | Practical Rule |
|---|---|---|
| Start with context | Design must come from repo, requirements, users, and constraints | Do not create screens before context and brief are documented |
| Every screen serves a task | UI exists to help a role complete a task | Link each screen to the role matrix and task map |
| Document decisions close to implementation | Design knowledge must live in the repo | Update Markdown, JSON, Mermaid, and version files |
| Make state behavior explicit | Users and engineers need predictable feedback | Document loading, empty, error, success, disabled, and permission states |
| Favor reusable patterns | AI-DLC benefits from consistent repeatable artifacts | Capture reusable components and patterns |
| Design for reviewability | Humans and agents must be able to audit the work | Use tables, checklists, source references, and quality gates |
| Accessibility is not optional | Accessibility defects are product defects | Run accessibility checklist before handoff |
| Scalability affects UX | Edge cases, data volume, and permissions shape design | Include scalability and edge-case review before handoff |
| Version every meaningful change | Future teams need to know why design changed | Update change log, DDR, version history, and release notes |

## Experience Tone

The pipeline should feel clear, disciplined, practical, and engineering-friendly. It should avoid vague design language and prefer specific, testable decisions.

## Artifact Writing Rules

- Write for both humans and AI agents.
- Prefer explicit tables over long narrative when mapping responsibility, states, or risks.
- Record assumptions instead of hiding uncertainty.
- Link to source files when decisions depend on another repo or artifact.
- Keep quality gates actionable and pass/fail friendly.

## Quality Gate

- UX decisions are tied to user roles, tasks, and source context.
- Each major artifact includes purpose, inputs, outputs, and quality gate.
- Design language is precise enough for implementation and QA.
