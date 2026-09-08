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
| [`eli-fintech`](skills/eli-fintech/SKILL.md) | Fintech and financial-system explanations | Money, obligations, ledgers, lifecycle, controls, and failure paths |

## Visual explanations

Every skill can use the shared [bento viewgraph guidance](shared/bento-viewgraph.md)
when a compact visual would clarify a flow, comparison, state machine, timeline,
or evidence map. Visuals are optional; the skills remain useful in plain text.

## Installation

Clone the repository once:

```sh
git clone https://github.com/maxwu/eli-skills.git "$HOME/.local/share/eli-skills"
cd "$HOME/.local/share/eli-skills"
```

### Codex

Install all four skills for your user account:

```sh
mkdir -p "$HOME/.agents/skills" "$HOME/.agents/shared"
cp -R skills/. "$HOME/.agents/skills/"
cp shared/bento-viewgraph.md "$HOME/.agents/shared/bento-viewgraph.md"
```

Codex detects skill changes automatically. If the new skills do not appear,
restart Codex. In Codex CLI or the IDE extension, use `/skills` or type `$` to
select a skill.

### Claude Code

Install all four skills for your user account:

```sh
mkdir -p "$HOME/.claude/skills" "$HOME/.claude/shared"
cp -R skills/. "$HOME/.claude/skills/"
cp shared/bento-viewgraph.md "$HOME/.claude/shared/bento-viewgraph.md"
```

Claude Code normally detects changes to an existing skills directory during the
current session. Restart it if you created the top-level directory for the first
time. Invoke a skill with `/eli5`, `/eli-grad`, `/eli-biz`, or `/eli-fintech`.

### Install selected skills only

Replace `eli5` below with any skill name:

```sh
mkdir -p "$HOME/.agents/skills" "$HOME/.agents/shared"
cp -R skills/eli5 "$HOME/.agents/skills/eli5"
cp shared/bento-viewgraph.md "$HOME/.agents/shared/bento-viewgraph.md"
```

For Claude Code, use `$HOME/.claude/skills` and `$HOME/.claude/shared` instead.

### Update

Pull the latest version, then repeat the relevant copy commands above:

```sh
cd "$HOME/.local/share/eli-skills"
git pull --ff-only
```

### Uninstall

Remove only the ELI Skills directories you installed:

```sh
rm -rf "$HOME/.agents/skills/eli5" \
       "$HOME/.agents/skills/eli-grad" \
       "$HOME/.agents/skills/eli-biz" \
       "$HOME/.agents/skills/eli-fintech"
rm -f "$HOME/.agents/shared/bento-viewgraph.md"
```

For Claude Code, replace `$HOME/.agents` with `$HOME/.claude`.

## Use

Copy a skill directory into your Codex or Claude Code skills directory, or link
it from a local clone. Invoke the skill with a topic, source file, repository
path, ticket, document, or URL that the active environment can access.

Examples:

```text
/eli5 What is eventual consistency?
/eli-grad Explain this worker pool and then go deeper.
/eli-biz Explain the eligibility rules in this service as a decision table.
/eli-fintech Show the payment lifecycle as a bento viewgraph.
```

## Design principle

The skills simplify progressively. They never invent missing facts, silently
merge conflicting evidence, or hide an important limitation behind an analogy.
