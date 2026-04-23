# Auto Plugins

The official [Claude Code plugin](https://docs.anthropic.com/en/docs/claude-code) marketplace package for [Auto](https://on.auto).

```
/plugin marketplace add BeOnAuto/auto-plugins
```

This repository bundles two plugins:

| Plugin | What it does |
|--------|-------------|
| **[auto-agent](https://github.com/beOnAuto/auto-agent)** | Connects your coding agent to an Auto workspace. Syncs the narrative model, scaffolds dev servers, and builds application code from structured specs. |
| **[ketchup](https://ketchup.on.auto/)** | LLM-powered guardrails for Claude Code. Turn every AI mistake into a rule AI can't repeat. 17 validators ship by default; bad commits don't land. |

## Install

Inside a Claude Code session:

```
/plugin marketplace add BeOnAuto/auto-plugins
/plugin install auto-agent
/plugin install ketchup
/reload-plugins
```

Install either or both. They work independently.

## What each plugin does

### auto-agent

Bridges your coding agent to the [Auto](https://on.auto) platform. Model your software as [narratives](https://narrativedriven.org/what-is-ndd), then let your agent build from the structured model.

- Scaffolds React + Apollo GraphQL dev servers with live preview
- Syncs the narrative model from your Auto workspace in real time
- Builds application code scene-by-scene with browser verification
- Validates model changes against 50+ structural rules

```
/auto-agent:connect <your-api-key>
/auto-agent:scaffold
/auto-agent:build
```

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
