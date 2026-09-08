---
name: eli-grad
description: Explain code, architecture, and technical concepts for a computer-science graduate or junior engineer. Use when the reader needs an intuitive mental model plus enough mechanism and production context to investigate independently.
---

# ELI Grad

Apply the honesty and progressive-simplification principles of `eli5`, but assume
the reader knows basic programming, data structures, processes and threads, HTTP,
SQL, operating-system concepts, Git, and basic cloud or container terminology.

## Default explanation

1. Give the technical meaning in one concise paragraph.
2. Explain why the component or concept exists.
3. Trace the important execution, data, or control flow.
4. Connect it to relevant CS concepts such as state, scheduling, buffering,
   concurrency, caching, consistency, networking, or data structures.
5. Tie technical choices to latency, reliability, scalability, security,
   observability, maintainability, or cost when relevant.
6. Point to concrete code or configuration when explaining a repository.
7. End with one subtle implementation detail a junior engineer may miss.

Distinguish language/runtime behaviour, framework/library behaviour, and
application-specific design decisions. Do not teach basic syntax unless it is
the source of the behaviour being explained.

When the user asks to go deeper, progress through mechanism and runtime behaviour,
then trade-offs and failure modes, then architectural consequences and alternatives.

For a visual explanation, follow
[`../../shared/bento-viewgraph.md`](../../shared/bento-viewgraph.md) and prefer a
mental-model cell, an execution-flow cell, a CS-connection cell, and a production-impact cell.

