# Daily Briefing

Pull together a morning overview for the user's Hera workspace. Use the Hera MCP tools to gather the following, then present a concise summary:

1. **Today's Roster** — Call `list_rosters` to see who is scheduled today. Summarize headcount and any gaps.

2. **Open Incidents** — Call `list_incidents` to find recent/open incidents. Highlight anything from the last 7 days.

3. **Fleet Status** — Call `list_vehicles` filtered by non-active statuses (Inactive - Maintenance, Inactive - Grounded, etc.) to show vehicles currently out of service.

4. **Performance Snapshot** — Call `get_performance_company_scorecard` to get the latest company scorecard. Highlight key metrics and any trends.

5. **Recent Counselings** — Call `list_counselings` to surface any counselings from the past 7 days.

Format the output as a clean briefing with sections and bullet points. Keep it scannable — highlight anything that needs immediate attention at the top.
