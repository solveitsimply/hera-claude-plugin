# Record a Drug Test

Help the user record a drug test for an associate.

## Steps

1. **Who was tested?** Ask for the associate's name. Use `list_associates` to find them and confirm.

2. **Test details** — Ask for:
   - `date` — when was the test? (default to today)
   - `location` — where was the test conducted?
   - `results` — what were the results?

3. **Review and confirm** — Show a summary before creating.

4. **Create** — Call `create_drug_test` with the collected data. Show the result.
