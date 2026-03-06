# Hera Plugin Setup

Help the user set up and authenticate the Hera Claude plugin.

Explain the following to the user:

1. **Get your Hera API key**: Log in to your Hera workspace, go to Settings → API Keys, and generate a new key.

2. **Configure the API key**: The Hera plugin reads your API key from the `HERA_API_KEY` environment variable. Set it in your shell profile:
   ```
   export HERA_API_KEY=your_key_here
   ```
   Then restart Claude Code for the change to take effect.

3. **Verify it's working**: Once configured, you can ask Claude things like:
   - "Show me all active associates"
   - "List any open incidents this week"
   - "What's the company scorecard?"
   - "Find associate John Smith"

If the user is on Claude.ai (not Claude Code), tell them the plugin uses MCP and requires the `HERA_API_KEY` environment variable to be set in their environment before Claude Code starts.
