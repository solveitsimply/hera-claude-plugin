# Report an Incident

Walk the user through reporting a vehicle incident (accident) step by step. Ask questions conversationally.

## Steps

1. **When did it happen?** Ask for the date and time of the incident.

2. **Which vehicle?** Ask for the vehicle name/number. Use `list_vehicles` with a search query to find it. Confirm and get the ID.

3. **Who was driving?** Ask for the associate's name. Use `list_associates` with a search query to find them. Confirm and get their ID.

4. **What happened?** Ask the user to describe the incident. Use their response to determine:
   - `vehicleHistoryType` — type of incident
   - `atFault` — was the associate at fault?
   - `damage` — description of damage
   - `damageSeverity` — severity level

5. **Location** — Ask where it happened:
   - `address`, `addressCity`, `addressState`, `addressZip`

6. **Police involvement** — Ask if police were called. If yes, collect:
   - `policeReportNumber`
   - `policeOfficerName`
   - `policeDepartment`

7. **Witnesses** — Ask if there were any witnesses:
   - `witnessName`
   - `witnessStatement`

8. **Insurance** — Ask if an insurance claim was filed:
   - `insuranceClaimNumber`

9. **Drug test** — Ask if a post-incident drug test was conducted:
   - `drugTestDate`
   - `drugTestResult`

10. **Notes** — Ask if there's anything else to add.

11. **Review and confirm** — Show a summary of all fields before creating. Ask the user to confirm.

12. **Create** — Call `create_incident` with the collected data. Show the result.

Skip questions that aren't relevant based on earlier answers (e.g., skip police details if no police were called).
