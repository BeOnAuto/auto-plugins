# Auto Plugins

The official [Claude Code plugin](https://docs.anthropic.com/en/docs/claude-code) marketplace package for [Auto](https://on.auto).

```
/plugin marketplace add BeOnAuto/auto-plugins
```

This repository bundles two plugins:

| Plugin | What it does |
|--------|-------------|
| **[auto-agent](https://github.com/beOnAuto/auto-agent)** | Connects your coding agent to an Auto workspace. Syncs the narrative model, scaffolds dev servers, and builds application code from structured specs. |
| **[auto-ketchup](https://ketchup.on.auto/)** | A quality loop for Claude Code. Validators gate every commit, reminders inject your guidelines, deny-lists protect files, auto-continue keeps the agent working. Stop babysitting, start parallelizing. |

## Install

Inside a Claude Code session:

```
/plugin marketplace add BeOnAuto/auto-plugins
/plugin install auto-agent
/plugin install auto-ketchup
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

### auto-ketchup

Installs a quality loop into Claude Code so you can trust your agent and run multiple sessions in parallel.

- Validates every commit against configurable rules (17 built-in validators)
- Injects context reminders at the right hook points
- Protects files via deny-list glob patterns
- Auto-continues the agent until the plan is done
- Enforces TCR (Test && Commit || Revert) discipline

```
/auto-ketchup-config show
```

> Auto gives you the spec. Ketchup gives you the discipline to execute against it without babysitting.

## Part of the ecosystem

- **[on.auto](https://on.auto)** — model your software as narratives
- **[narrativedriven.org](https://narrativedriven.org)** — the spec dialect behind Auto
- **[specdriven.com](https://specdriven.com)** — why specifications matter for AI-native development

## Community

- [Discord](https://discord.com/invite/B8BKcKMRm8)
- [Auto App](https://app.on.auto)

## License

MIT · [Auto](https://on.auto)
