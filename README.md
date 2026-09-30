# Auto Plugins

The official [Claude Code plugin](https://docs.anthropic.com/en/docs/claude-code) marketplace package for [Auto](https://on.auto).

```
/plugin marketplace add BeOnAuto/auto-plugins
```

This repository bundles:

| Plugin | What it does |
|--------|-------------|
| **[ketchup](https://ketchup.on.auto/)** | LLM-powered guardrails for Claude Code. Turn every AI mistake into a rule AI can't repeat. 17 validators ship by default; bad commits don't land. |

## Install

Inside a Claude Code session:

```
/plugin marketplace add BeOnAuto/auto-plugins
/plugin install ketchup
/reload-plugins
```

## What it does

### ketchup

Runs LLM-powered guardrails on every AI commit so bad commits don't land. The pattern: observe an AI mistake, encode it as a rule, AI can't repeat it.

- 17 LLM validators ship by default; add your own in `.ketchup/validators/`
- Reminders re-inject your operating context every session and every prompt
- Deny-list gives structural protection for files AI must never touch
- Auto-continue reads `ketchup-plan.md` and keeps the agent working when commits stay clean
- TCR gate: red commits don't land

```
/ketchup:config show
```

> Auto gives you the spec. Ketchup gives you the discipline to execute against it.

## Part of the ecosystem

- **[on.auto](https://on.auto)**: model your software as narratives
- **[narrativedriven.org](https://narrativedriven.org)**: the spec dialect behind Auto
- **[specdriven.com](https://specdriven.com)**: why specifications matter for AI-native development

## Community

- [Discord](https://discord.com/invite/B8BKcKMRm8)
- [Auto App](https://app.on.auto)

## License

MIT · [Auto](https://on.auto)
