# IntelMCP for Claude Code and Cowork

IntelMCP gives security analysts searchable, monitored threat intelligence from
public Telegram channels, inside Claude. This plugin adds the IntelMCP connector
and two commands:

- `/intelmcp:setup` — Claude interviews you about what you need to watch, tests
  alert rules against recent history, and saves your setup once you approve it.
- `/intelmcp:dashboard` — a visual overview of your matches, severities,
  trending indicators, rules and sources.

## Install

You need an IntelMCP subscription: https://intelmcp.io

    /plugin marketplace add intelmcpops-creator/intelmcp-plugin
    /plugin install intelmcp@intelmcp

The first time Claude uses IntelMCP, it asks you to sign in (Google or an
emailed code). Use the email address you subscribed with.

In claude.ai, add `https://mcp.intelmcp.io/mcp` as a custom connector instead;
the setup interview and dashboard are available there as connector prompts.

Docs: https://intelmcp.io/docs/ · Privacy: https://intelmcp.io/privacy/ ·
Terms: https://intelmcp.io/terms/ · Contact: intelmcp.ops@gmail.com

IntelMCP is not affiliated with or endorsed by Telegram.
