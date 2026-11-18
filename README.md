# Utmost for Claude

[Utmost](https://utmostcoach.com) is a training platform. People log their training in the Utmost iPhone app, and trainers and studios plan programs and follow their clients there. This plugin connects Claude to your Utmost account, so you can ask how your training is going, or let Claude help you coach.

## Install

In Claude, add Utmost from the plugin directory. In Claude Code you can also install it from this repository:

```
/plugin install utmost --marketplace webreact/utmost-claude-plugin
```

Before Claude Code 2.1.275, add the marketplace first:

```
/plugin marketplace add webreact/utmost-claude-plugin
/plugin install utmost@utmost
```

## What it contains

- **The Utmost connector** (`.mcp.json`): Utmost's remote MCP server at `https://app.utmostcoach.com/mcp`. You sign in to Utmost and approve Claude the first time you use it (OAuth). The plugin runs nothing on your computer.
- **The skill `utmost-coaching`**: how to review a week of training, check in on clients and propose exercises or program drafts with the connector's tools.

## What you can do

- **Your own training:** sessions, progress, personal records and the history of an exercise.
- **If you coach:** your clients' weeks and progress, and your organization's exercises and programs. A client is only there when they share their training log with your organization and allow the AI assistant.
- **Propose changes:** Claude can propose an exercise or a program draft. Nothing changes until you open the link it gives you, sign in to Utmost and approve it.

What the connector can do follows your Utmost account every time Claude asks. You need an Utmost account with a confirmed email address.

## What it sends and where

Claude calls the Utmost server with your questions' parameters (for example a date range or a client id), and the server answers with the training data your account may see. Utmost logs which tool was used and when, never what you asked or what the tool answered. The answers go to Claude and are handled under Anthropic's terms. Disconnect at any time in Utmost under Settings → Connected apps or in the iPhone app under Profile → Connected apps.

- Setup and help: <https://app.utmostcoach.com/ai-apps>
- Privacy policy: <https://app.utmostcoach.com/privacy>
- Terms of service: <https://app.utmostcoach.com/terms>
- Support: <support@utmostcoach.com>
