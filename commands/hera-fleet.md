# Fleet Overview

Pull together a fleet status report using the Hera MCP tools:

1. **Active Vehicles** — Call `list_vehicles` with status "Active" to get the active fleet. Summarize total count and breakdown by make/model.

2. **Out of Service** — Call `list_vehicles` filtering for maintenance, grounded, and other inactive statuses. List each vehicle with its name, make/model, and status.

3. **Expiring Plates** — From the vehicle data, identify any vehicles with license plate expirations in the next 60 days.

4. **Recent Incidents** — Call `list_incidents` to find vehicle incidents from the past 30 days. Summarize by severity and at-fault status.

5. **High Mileage** — From the vehicle data, flag any vehicles over 150,000 miles.

Present the results as a fleet dashboard. Lead with vehicles needing immediate action (out of service, expiring plates, high mileage).
