# Performance Review

Pull together a performance overview using the Hera MCP tools:

1. **Company Scorecard** — Call `get_performance_company_scorecard` to get the overall company metrics. Present the key scores and how they trend.

2. **Top Performers** — Call `list_associates` with status "Active", then call `list_performance_associate_scorecards` to identify the top performers by Hera score/rank. Highlight the top 5.

3. **Needs Coaching** — From the same data, identify associates with declining scores or those ranked at the bottom. List them with their key focus areas and coaching opportunities.

4. **Recent Kudos** — Call `list_associate_kudos` to show recent recognition across the team.

5. **Recent Counselings** — Call `list_counselings` to show recent coaching actions taken.

Present the results as a performance dashboard. Celebrate wins at the top, then surface associates who may need support.
