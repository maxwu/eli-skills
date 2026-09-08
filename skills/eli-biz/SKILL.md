---
name: eli-biz
description: Explain complicated business logic implemented in software, prioritizing business meaning, rules, decisions, state changes, exceptions, and outcomes while retaining only the technical context that affects behaviour.
---

# ELI Business

Apply the honesty and progressive-simplification principles of `eli5`. Explain
what the software means to the business before explaining how it implements it.

## Discover evidence

Inspect relevant available sources: requirements, acceptance criteria, product
documentation, tickets, code, tests, configuration, schemas, decision records,
and user-provided paths or URLs. Do not speculate about a source that was not opened.

When sources disagree, report the conflict. Treat authoritative current requirements
as intended behaviour, executable accepted tests as behavioural evidence, and
implementation as actual behaviour; do not assume these are identical.

## Default explanation

1. **Business purpose** — capability, initiating actor, business object, outcome.
2. **Domain entities** — meaning, relationships, important attributes, lifecycle.
3. **Business rules** — express important rules as conditions and outcomes.
4. **Decision flow** — show decisions in business language, preferably as a table.
5. **State transitions** — trigger, conditions, new state, business consequence.
6. **Exceptions and overrides** — manual paths, legacy cases, temporal rules,
   configuration, feature flags, partial completion, and conflicting rules.
7. **Business invariants** — conditions that must remain true.
8. **Technical context** — only mechanisms that alter timing, consistency,
   reliability, visibility, or another business-relevant behaviour.
9. **Risk and unknowns** — material failure consequences and unresolved intent.

Classify code conditions as business rule, data validation, technical safeguard,
operational workaround, legacy compatibility, or unknown. Never invent a business rationale.

For a visual explanation, follow
[`../../shared/bento-viewgraph.md`](../../shared/bento-viewgraph.md) and prefer
purpose, actors, rules, decision, state, exception, and outcome cells.

