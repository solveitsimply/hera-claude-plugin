# Hera Plugin Setup

Help the user connect and authenticate the Hera Claude plugin.

Explain the following to the user:

## Claude Desktop / Claude Cowork

1. **Install the plugin**: Open **Settings → Customize → Personal plugins** and add the Hera plugin from the marketplace.

2. **Authenticate with Hera**: Go to **Customize → Hera → Connectors** and click the Hera connector. A browser window will open asking you to allow Claude access to your Hera workspace. Log in if needed, then click **Allow Access**.

3. **Verify it's working**: Once connected, try asking Claude things like:
   - "Show me all active associates"
   - "List any open incidents this week"
   - "What's the company scorecard?"
   - "Find associate John Smith"

4. **Revoke access**: If you need to disconnect Claude from Hera, go to **Settings → Service Users** in your Hera workspace and revoke the "Claude Cowork" service user.

## Claude Code (CLI)

1. **Authenticate with Hera**: Run `/mcp` or open Settings → MCP Servers and click **Authenticate** next to the Hera server. A browser window will open asking you to allow Claude Code access to your Hera workspace. Log in if needed, then click **Allow Access**.

2. **Verify it's working**: Once connected, try asking Claude things like:
   - "Show me all active associates"
   - "List any open incidents this week"
   - "What's the company scorecard?"
   - "Find associate John Smith"

3. **Revoke access**: If you need to disconnect Claude from Hera, go to **Settings → Service Users** in your Hera workspace and revoke the "Claude Cowork" service user.

## Troubleshooting

If you see an "Authentication failed" error, try the Authenticate flow again. If the issue persists, check that the "Claude Cowork" service user is active under **Settings → Service Users** in your Hera workspace.
