# Hera Plugin Setup

Help the user connect and authenticate the Hera Claude plugin.

Explain the following to the user:

1. **Authenticate with Hera**: Open the MCP panel (run `/mcp` or open Settings → MCP Servers) and click **Authenticate** next to the Hera server. A browser window will open asking you to allow Claude Cowork access to your Hera workspace. Log in if needed, then click **Allow Access**.

2. **Verify it's working**: Once connected, try asking Claude things like:
   - "Show me all active associates"
   - "List any open incidents this week"
   - "What's the company scorecard?"
   - "Find associate John Smith"

3. **Revoke access**: If you need to disconnect Claude from Hera, go to **Settings → Service Users** in your Hera workspace and revoke the "Claude Cowork" service user.

If the user sees an "Authentication failed" error, ask them to try the Authenticate flow again from the MCP panel.
