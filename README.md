# Auto Plugins

The official [Claude Code plugin](https://docs.anthropic.com/en/docs/claude-code) marketplace package for [Auto](https://on.auto).

```
/plugin marketplace add BeOnAuto/auto-plugins
```

This repository bundles two plugins:

| Plugin | What it does |
|--------|-------------|
| **[auto-agent](../auto-agent/)** | Connects your coding agent to an Auto workspace — syncs the narrative model, scaffolds dev servers, and builds application code from structured specs |
| **[claude-auto](../claude-auto/)** | Husky-style hooks for Claude Code — commit validators, context-injection reminders, deny-lists, auto-continue, and TCR discipline |

## Install

Inside a Claude Code session:

```
/plugin marketplace add BeOnAuto/auto-plugins
/plugin install auto-agent
/plugin install claude-auto
/reload-plugins
```

Install either or both — they work independently.

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

### claude-auto

Installs a quality loop into Claude Code so you can trust your agent and run multiple sessions in parallel.

- Validates every commit against configurable rules (17 built-in validators)
- Injects context reminders at the right hook points
- Protects files via deny-list glob patterns
- Auto-continues the agent until the plan is done
- Enforces TCR (Test && Commit || Revert) discipline

```
/claude-auto:config show
```

## Part of the ecosystem

- **[on.auto](https://on.auto)** — model your software as narratives
- **[narrativedriven.org](https://narrativedriven.org)** — the spec dialect behind Auto
- **[specdriven.com](https://specdriven.com)** — why specifications matter for AI-native development

## Community

- [Discord](https://discord.com/invite/B8BKcKMRm8)
- [Auto App](https://app.on.auto)

## License

MIT · [Auto](https://on.auto)
