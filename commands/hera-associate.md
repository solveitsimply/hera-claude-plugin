# Associate Deep-Dive

Look up a specific associate and build a comprehensive profile. Ask the user which associate they want to review if not specified.

Use the Hera MCP tools to gather the following for the associate:

1. **Profile** — Call `get_associate` or `list_associates` with a search query to find the associate. Show their name, status, hire date, contact info, key focus area, and coaching opportunity.

2. **Performance** — Call `list_performance_associate_scorecards` for their scorecard history. Summarize recent trends.

3. **Counselings** — Call `list_associates_counselings` for this associate. List any active or recent counselings with dates and types.

4. **Kudos** — Call `list_associates_associate_kudos` for this associate. Highlight recent recognition.

5. **Documents** — Call `list_associates_documents` to show what documents are on file (license, certifications, etc.) and flag anything expired or missing.

6. **Issues** — Call `list_associates_associate_issues` for any open issues.

7. **Drug Tests & Medical Cards** — Call `list_associates_drug_tests` and `list_associates_medical_cards` to check compliance status.

Present the results as a structured profile. Flag anything that needs attention (expired documents, open issues, declining performance).
