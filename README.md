# Cadenzova plugin for Claude Code

Connects Claude Code to [Cadenzova](https://cadenzova.com) and adds two skills:

- `/plan-my-week`: plans, writes and checks next week's posts, then leaves them for your approval.
- `/monthly-review`: explains the last 30 days and records what to change.

Posts wait for your approval unless you choose Autopilot on your connection.

## Install

In Claude Code:

```
/plugin marketplace add cadenzova/cadenzova-claude-plugin
/plugin install cadenzova@cadenzova
```

Then run `/mcp`, choose `cadenzova`, and sign in with your Cadenzova account. On the consent screen choose
**Draft and approve**.

Without the plugin, the server alone:

```bash
claude mcp add --scope user --transport http cadenzova https://mcp.cadenzova.com/mcp
```

## What it contains

- `.claude-plugin/` the plugin and marketplace listing
- `.mcp.json` the Cadenzova server address (no secrets)
- `skills/` the two skill instructions

No passwords or keys are stored here. Your sign-in stays in Claude Code and your Cadenzova account.

## More

- Feature page: https://cadenzova.com/features/ai-agents
- API reference: https://mcp.cadenzova.com/v1/docs

This repository is a published copy of the plugin folder. Changes are made in the Cadenzova product repository and copied here.

## Licence

MIT. See [LICENSE](LICENSE).
