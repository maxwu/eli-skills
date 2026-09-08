# ELI Skills

**Simplify the explanation, not the underlying system.**

ELI Skills is a small family of explanation skills. Each skill keeps causality,
important caveats, and uncertainty intact while changing the explanation lens.

## Skills

| Skill | Best for | Default lens |
|---|---|---|
| [`eli5`](skills/eli5/SKILL.md) | Anyone encountering an unfamiliar idea | Plain language, concrete examples, honest simplification |
| [`eli-grad`](skills/eli-grad/SKILL.md) | CS graduates and junior engineers | Mental model, execution flow, CS concepts, production consequences |
| [`eli-biz`](skills/eli-biz/SKILL.md) | Product, operations, and technical stakeholders | Business purpose, rules, decisions, states, and outcomes |
| [`eli-bank`](skills/eli-bank/SKILL.md) | Banking and financial-system explanations | Money, obligations, ledgers, lifecycle, controls, and failure paths |

## Visual explanations

Every skill can use the shared [bento viewgraph guidance](shared/bento-viewgraph.md)
when a compact visual would clarify a flow, comparison, state machine, timeline,
or evidence map. Visuals are optional; the skills remain useful in plain text.

## Use

Copy a skill directory into your Codex or Claude Code skills directory, or link
it from a local clone. Invoke the skill with a topic, source file, repository
path, ticket, document, or URL that the active environment can access.

Examples:

```text
/eli5 What is eventual consistency?
/eli-grad Explain this worker pool and then go deeper.
/eli-biz Explain the eligibility rules in this service as a decision table.
/eli-bank Show the payment lifecycle as a bento viewgraph.
```

## Design principle

The skills simplify progressively. They never invent missing facts, silently
merge conflicting evidence, or hide an important limitation behind an analogy.

