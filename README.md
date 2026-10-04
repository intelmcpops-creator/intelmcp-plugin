# IntelMCP for Claude Code and Cowork

IntelMCP gives security analysts searchable, monitored threat intelligence from
public Telegram channels, inside Claude. This plugin adds the IntelMCP connector
and five commands:

- **Set up monitoring**, `/intelmcp:setup`: Claude asks what you need to watch,
  tests alert rules against recent history, saves your setup once you approve it
  and shows the first matches. Run it again later to tune your rules.
- **Dashboard**, `/intelmcp:dashboard`: a visual overview of your matches,
  severities, trending indicators, rules and sources.
- **Triage matches**, `/intelmcp:triage`: Claude judges your unreviewed matches
  against your watch profile and tells you what's new and what matters, with links.
- **Investigate**, `/intelmcp:investigate <question>`: research a threat actor,
  campaign, leak or indicator across the collection, with every point cited.
- **Command centre**, `/intelmcp:command-centre`: creates your own live IntelMCP
  dashboard as a private page in your Claude account (Artifacts), where you triage
  alerts and manage rules, exclusions and deliveries. It needs IntelMCP connected
  in claude.ai too. More: https://intelmcp.io/command-centre/

## Install

You need an IntelMCP subscription: https://intelmcp.io

    /plugin marketplace add intelmcpops-creator/intelmcp-plugin
    /plugin install intelmcp@intelmcp

Then sign in once: run `/mcp`, choose **intelmcp**, then **Authenticate**, and
sign in with Google or an emailed code. Use the email address you subscribed
with. Install either this plugin or the `claude mcp add` command from the docs,
not both.

In claude.ai, add `https://mcp.intelmcp.io/mcp` as a custom connector instead.
The same four are prompts there: pick them by title (Set up monitoring,
Dashboard, Triage matches, Investigate) from the IntelMCP prompt menu.

Docs: https://intelmcp.io/docs/ · Privacy: https://intelmcp.io/privacy/ ·
Terms: https://intelmcp.io/terms/ · Contact: support@intelmcp.io

IntelMCP is not affiliated with or endorsed by Telegram.
