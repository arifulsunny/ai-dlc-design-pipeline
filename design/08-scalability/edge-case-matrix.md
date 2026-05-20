# Edge Case Matrix

## Purpose

This file captures edge cases that can affect UX, layout, backend behavior, QA, and implementation quality.

## Matrix

| Edge Case | User Impact | Design Response | Engineering Impact | Priority |
|---|---|---|---|---:|
| Missing source files | AI may generate incomplete artifacts | Add open questions and block dependent outputs | Need source discovery or clarification | P0 |
| Conflicting requirements | User flow may be inconsistent | Document conflict and request decision | May require product decision before build | P0 |
| Unknown user roles | Screens may not map to valid users | Add role assumptions and review | Permission model may be unclear | P0 |
| Large data sets | Tables and dashboards may become unusable | Define filtering, pagination, empty and loading states | API pagination or search needed | P1 |
| Permission mismatch | User sees actions they cannot perform | Define restricted and disabled states | Backend authorization alignment needed | P0 |
| Multi-repo source inputs | Output may lose traceability | Use source-reference instructions | Need stable file paths and commit refs | P0 |
| Design system missing component | UI inconsistency | Add temporary rule and reusable pattern note | Component build or variant needed | P1 |
| Rapid design changes | Stale implementation handoff | Update change log, DDR, and affected artifacts | Rework may be required | P0 |
| Mobile constraints | Layout breaks on small screens | Apply responsive rules | Frontend responsive implementation needed | P1 |
| Accessibility exception | Users may be blocked | Document risk and mitigation | QA and frontend fix required | P0 |

## Quality Gate

- P0 edge cases are resolved or explicitly accepted before handoff.
- Engineering impact is documented for each high-risk edge case.
- Edge cases that change the product flow are reflected in user-flow and acceptance criteria.
