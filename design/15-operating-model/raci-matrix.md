# RACI Matrix

## Purpose

This file defines responsibility for each stage so human team members and AI agents do not duplicate work or leave ownership gaps.

## RACI Legend

| Letter | Meaning |
|---|---|
| R | Responsible: does the work |
| A | Accountable: approves the outcome |
| C | Consulted: provides input |
| I | Informed: kept aware |

## Stage RACI

| Stage | Product | BA | UX/Product Design | Frontend | Backend | QA | AI Agent | Design Lead |
|---|---|---|---|---|---|---|---|---|
| Context intake | A | C | C | C | C | I | R | C |
| Design brief | A | R | C | I | I | C | R | C |
| Role and task mapping | C | R | A | C | C | C | R | C |
| User flow and IA | C | C | R | C | C | C | R | A |
| UX and state model | C | C | R | C | C | C | R | A |
| Layout and components | C | I | R | C | I | C | R | A |
| Style guide and tokens | I | I | R | C | I | C | R | A |
| Accessibility review | I | C | R | C | I | A | R | C |
| Scalability and edge cases | C | R | C | C | C | A | R | I |
| Prototype | C | I | R | C | I | C | R | A |
| Design review | C | C | C | C | C | C | R | A |
| Frontend handoff | I | I | C | A/R | C | C | R | C |
| Backend impact | I | C | C | C | A/R | C | R | I |
| Validation | C | I | C | C | C | A/R | R | C |
| Version control | C | I | R | I | I | I | R | A |
| Design system update | I | I | R | C | I | C | R | A |

## AI Agent Ownership Rule

AI agents may be Responsible for drafting, checking, and updating artifacts, but a human or designated approval agent must be Accountable for high-risk decisions.

## Quality Gate

- Every stage has exactly one Accountable owner.
- High-risk changes identify Responsible and Accountable owners before handoff.
- If two agents edit related files in parallel, the Accountable owner resolves conflicts.
