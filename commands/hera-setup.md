# Hera Plugin Setup

Help the user connect and authenticate the Hera Claude plugin.

Explain the following to the user:

## Claude Desktop / Claude Cowork

1. **Install the plugin**: Open **Settings → Customize → Personal plugins** and add the Hera plugin.

2. **Authenticate with Hera**: Go to **Customize → Hera → Connectors** and click the Hera connector. Your browser will open to a Hera authorization page. Log in if needed, then click **Allow Access**. A "Claude Cowork" service user will be created automatically in your workspace.

3. **Verify it's working**: Once connected, try asking Claude things like:
   - "Show me all active associates"
   - "List any open incidents this week"
   - "What's the company scorecard?"
   - "Find associate John Smith"

4. **Revoke access**: To disconnect Claude from Hera, go to **Settings → Service Users** in your Hera workspace and revoke the "Claude Cowork" service user.

## Claude Code (CLI)

1. **Authenticate with Hera**: Run `/mcp` or open Settings → MCP Servers and click **Authenticate** next to the Hera server. Your browser will open to a Hera authorization page. Log in if needed, then click **Allow Access**.

2. **Verify it's working**: Once connected, try asking Claude things like:
   - "Show me all active associates"
   - "List any open incidents this week"
   - "What's the company scorecard?"
   - "Find associate John Smith"

3. **Revoke access**: To disconnect Claude from Hera, go to **Settings → Service Users** in your Hera workspace and revoke the "Claude Cowork" service user.

## Troubleshooting

- **Authentication failed**: Try the Authenticate flow again. If the issue persists, check that the "Claude Cowork" service user is active under **Settings → Service Users** in your Hera workspace.
- **No browser window opens**: The OAuth endpoints may not be deployed yet. Check with your Hera admin that the latest API version is live.
