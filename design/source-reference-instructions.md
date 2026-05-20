# Source Reference Instructions

## Purpose

Use this instruction file when any design artifact is generated or updated by referencing multiple files, repositories, branches, pull requests, issues, design files, documents, or other external sources.

The goal is to make every generated design file traceable, reviewable, and safe for future humans and AI agents to reuse.

## When This Applies

Apply these instructions when an artifact uses any of the following:

- More than one file in the same repository
- Files from another repository
- Files from another branch
- GitHub issues or pull requests
- Figma, FigJam, screenshots, PDFs, spreadsheets, docs, or slide decks
- API documentation or backend contracts
- Prior design artifacts
- A shared conversation or external product note

## Required Source Reference Block

Add this block near the top or bottom of the generated file when multiple sources inform the output:

```md
## Source References

| Source | Location | Version or Date | Used For | Confidence |
|---|---|---|---|---|
| Example source name | repo/path/file.md or URL | commit, branch, PR, date, or version | Requirement, flow, API, UI pattern, decision | High/Medium/Low |

## Source Assumptions

- Assumption 1
- Assumption 2

## Source Gaps

| Gap | Owner | Needed Before | Status |
|---|---|---|---|
| Missing detail | Product/Design/Engineering | Handoff/review/release | Open |
```

## Required Metadata

Whenever possible, record:

- Repository name
- File path
- Branch name
- Commit SHA
- Pull request or issue number
- Document version
- Figma file and frame link
- Date accessed
- Which part of the generated artifact used the source
- Confidence level

## Confidence Levels

| Level | Meaning |
|---|---|
| High | Source is current, specific, and directly supports the generated content |
| Medium | Source is relevant but incomplete, older, or partially inferred |
| Low | Source is indirect, ambiguous, or needs owner confirmation |

## Conflict Handling

When sources disagree:

1. Do not silently choose one source.
2. Document the conflict in `Source Gaps`.
3. Prefer the newest approved source only when ownership and status are clear.
4. Add an open question with an owner.
5. If the conflict affects flow, layout, accessibility, backend behavior, or release scope, add a design risk log entry.

## Cross-Repo Safety Rules

- Do not copy private or unrelated implementation details into public design docs.
- Reference exact paths instead of vague source names.
- Avoid using stale generated artifacts as source truth unless version history confirms they are current.
- If a source file is unavailable, state that clearly and mark confidence as low.
- If generated content changes a previous decision, update `design/13-version-control/design-decision-records.md`.

## Quality Gate

A multi-source generated artifact is ready only when:

- Source references are documented.
- Assumptions and gaps are visible.
- Conflicts are resolved or assigned.
- Confidence levels are stated.
- Affected change log or decision record files are updated when the design meaning changes.
