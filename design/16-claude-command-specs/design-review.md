# Command: /design-review

## Purpose

Run structured design review and produce a readiness score before implementation or release.

## Inputs

- All applicable pipeline files for the selected usage level
- `design/15-operating-model/pipeline-usage-levels.md`
- `design/15-operating-model/design-readiness-score.md`
- `design/15-operating-model/raci-matrix.md`
- Related GitHub issues, PRs, or source references

## Output File

`design/10-review/design-review-report.md`

## Required Sections

- Review scope
- Findings
- Severity
- Owner
- Recommendation
- Design readiness score
- Re-entry recommendation
- Approval table
- Source references, when multi-source
- Quality gate

## Quality Score Criteria

| Category | 5 Means |
|---|---|
| Review coverage | All required files for selected level are reviewed |
| Finding quality | Findings are specific, actionable, and severity-ranked |
| Decision clarity | Pass, blocked, or accepted-risk decision is explicit |
| Re-entry clarity | Failed categories map to exact files to revisit |

## Pass Threshold

- Lite: 3.5
- Standard: 4.0
- Full: 4.25

## Failure Re-Entry

If score is below threshold, mark the review as `Blocked` and re-enter the exact failed stage.
