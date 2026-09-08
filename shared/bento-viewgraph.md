# Bento Viewgraphs

Use a bento viewgraph only when spatial grouping makes the explanation easier
to understand than short prose. Good candidates include flows, state changes,
comparisons, evidence maps, timelines, and one concept with several consequences.

## Default composition

Choose only the cells that help:

```text
┌──────────────────────────┬──────────────────────────┐
│ THE SHORT ANSWER         │ WHY IT EXISTS            │
│ One plain sentence       │ Problem and consequence  │
├──────────────────────────┴──────────────────────────┤
│ HOW IT WORKS                                        │
│ Input → decision → state change → outcome           │
├──────────────────────────┬──────────────────────────┤
│ CONCRETE EXAMPLE         │ WATCH OUT                │
│ One representative case │ Boundary or failure path │
├──────────────────────────┴──────────────────────────┤
│ WHAT THIS VIEW SIMPLIFIES                           │
└─────────────────────────────────────────────────────┘
```

## Rules

- Lead with one message, not a dashboard of unrelated facts.
- Give each cell one job and a short, descriptive heading.
- Preserve reading order from top-left to bottom-right.
- Prefer five useful cells to nine crowded cells.
- Use arrows only for real sequence or causality.
- Label illustrative values and inferred relationships.
- Include failure, exception, or uncertainty cells when material.
- Never let decoration compete with meaning.
- For text-only environments, use Markdown tables, Mermaid, or compact ASCII.
- For rendered artifacts, use high contrast, generous whitespace, restrained
  colour, and readable type at presentation distance.

## Lens-specific cells

- `eli5`: short answer, why, example, steps, analogy boundary.
- `eli-grad`: mental model, execution flow, CS connection, production impact.
- `eli-biz`: purpose, actors, rules, decisions, states, business outcome.
- `eli-fintech`: parties, money/obligation, ledger effect, lifecycle, controls.
