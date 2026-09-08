---
name: eli5
description: Explain an unfamiliar idea in plain language without losing essential causality, caveats, or uncertainty. Use when the user asks for ELI5, a simple explanation, an intuitive walkthrough, or an accessible visual.
---

# ELI5

Explain plainly without falsifying, omitting essential causality, or treating
the subject as magic.

## Calibrate first

Infer the reader's background from the request and conversation. If it is not
clear, begin accessibly and let the reader ask for greater depth. Do not make
the tone childish unless the user actually asks for a child-oriented answer.

When a source, file, repository path, ticket, document, or URL is named, inspect
it before making claims about its contents. Say what could not be accessed.

## Default explanation

Use only the sections that improve understanding:

1. **The short answer** — one or two plain sentences.
2. **Why it exists** — the problem it solves and what happens without it.
3. **A concrete example** — one representative scenario.
4. **How it works** — the smallest honest causal sequence.
5. **A simple visual** — only for relationships, decisions, states, or time.
6. **Where the analogy breaks** — name misleading edges of any analogy used.
7. **What was simplified** — reveal important omitted complexity.
8. **Go deeper** — offer two or three specific directions, not a generic prompt.

Do not force every heading into a short answer.

## Explanation discipline

- Prefer familiar words, but introduce the correct term so the reader can reuse it.
- Explain cause and effect; do not replace mechanisms with metaphors.
- Separate established facts, observations, inference, examples, and unknowns.
- Label invented names, numbers, and scenarios as illustrative.
- Keep prerequisites local: explain only the background needed for this topic.
- When sources conflict, show the disagreement rather than silently resolving it.
- If the simple model would produce a wrong decision, add the missing nuance.
- If the user says `deeper`, add mechanism, trade-offs, and failure modes instead
  of repeating the same explanation with more words.

## Visual mode

When the user asks for a visual or viewgraph, or when a compact visual materially
improves comprehension, follow [`../../shared/bento-viewgraph.md`](../../shared/bento-viewgraph.md).
Keep the explanation usable without the rendered artifact.

