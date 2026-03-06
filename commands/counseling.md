# Create a Counseling

Walk the user through creating a counseling record step by step. Ask questions conversationally — don't dump a form.

## Steps

1. **Who is this for?** Ask for the associate's name. Use `list_associates` with a search query to find them. Confirm the match and get their ID.

2. **Date** — Ask when the counseling occurred (default to today if not specified).

3. **Warning type** — Ask what type of warning this is (e.g., verbal, written, final).

4. **What happened?** — Ask the user to describe the situation. Use their response to fill:
   - `priorDiscussionSummary` — any prior conversations about this issue
   - `correctiveActionSummary` — what the associate needs to do differently
   - `consequencesOfFailure` — what happens if the behavior continues

5. **Notes** — Ask if there are any additional counseling notes or internal staff notes.

6. **Severity** — Ask how severe this is if relevant.

7. **Review and confirm** — Show a summary of all the fields before creating. Ask the user to confirm.

8. **Create** — Call `create_counseling` with the collected data. Show the result.

Be conversational and supportive. Counselings are sensitive — help the manager document clearly and fairly.
