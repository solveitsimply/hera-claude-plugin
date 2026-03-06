# Start Onboarding

Help the user create an onboarding record for a new associate.

## Steps

1. **Who is being onboarded?** Ask for the associate's name. Use `list_associates` to find them and confirm. Get their ID.

2. **Onboarding program** — Ask what onboarding program or checklist to use:
   - `name` — the name/title of the onboarding record

3. **Dates** — Ask for:
   - `dateStart` — when does onboarding start? (default to today)
   - Any other key dates if relevant

4. **Trainer** — Ask who will be the trainer for this onboarding.

5. **Review and confirm** — Show a summary before creating. Ask the user to confirm.

6. **Create** — Call `create_onboarding` with the collected data. Show the result.

After creating, suggest the user check back on progress using the associate deep-dive command.
