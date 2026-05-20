# Responsive Layout Rules

## Purpose

This file defines responsive design expectations for pipeline-generated product screens and documentation artifacts.

## Breakpoints

| Token | Width | Intent |
|---|---:|---|
| `sm` | 480px | Small phones |
| `md` | 768px | Tablets and large phones |
| `lg` | 1024px | Small laptops |
| `xl` | 1280px | Desktop |
| `2xl` | 1536px | Wide desktop |

## Layout Principles

- Content should reflow, not overlap.
- Navigation should remain reachable on all viewports.
- Primary tasks should stay visible without unnecessary scrolling.
- Tables must have responsive alternatives or horizontal scrolling when data is wide.
- Forms should use single-column layout on small screens.
- Touch targets should be at least 44px by 44px.
- Long labels, role names, and state messages must wrap cleanly.

## Documentation Layout Rules

| Content Type | Desktop | Mobile |
|---|---|---|
| Markdown table | Use full table | Allow horizontal scroll or convert to stacked sections |
| Mermaid diagram | Keep left-to-right when readable | Use simpler diagram or provide text fallback |
| Checklist | Multi-section list | Single-column list |
| Screen spec | Sectioned document | Same order, shorter tables where possible |
| Audit matrix | Table with status | Stack by issue or screen if needed |

## Product UI Rules

| Pattern | Desktop | Tablet | Mobile |
|---|---|---|---|
| App shell | Sidebar plus content | Collapsible sidebar | Bottom nav or drawer |
| Data table | Full table with filters | Priority columns plus details | Cards or compact rows |
| Form | Two-column where useful | One or two columns | Single column |
| Wizard | Horizontal stepper | Compact stepper | Vertical or progress text |
| Dashboard | Multi-column grid | Two-column grid | Single-column cards |

## Quality Gate

- Every P0 screen specifies desktop and mobile behavior.
- Wide tables or dense data have a responsive plan.
- No layout relies on fixed widths that can break in normal product viewports.
