# Report an Injury

Walk the user through reporting a workplace injury step by step. This is an OSHA-style injury report — be thorough but conversational.

## Steps

1. **Who was injured?** Ask for the associate's name. Use `list_associates` to find them and get their ID, hire date, DOB, and gender.

2. **When did it happen?** Collect:
   - `injuryDate` — date of injury
   - `injuryTime` — time of injury (or mark `injuryTimeIsUnknown`)
   - `timeStaffStartedWork` — what time did they start their shift?

3. **What happened?** Ask the user to describe the incident. Use their response to fill:
   - `descriptionBeforeAccident` — what was the associate doing before the injury?
   - `descriptionIncident` — how did the injury occur?
   - `descriptionInjury` — what is the injury? (e.g., sprain, cut, fracture)
   - `descriptionDirectHarmCause` — what directly caused the harm? (e.g., wet floor, heavy box)
   - `injuryType` — categorize the injury type

4. **Medical treatment** — Ask if they received medical treatment:
   - `physicianName`, `physicianFacility`
   - `physicianAddress`, `physicianCity`, `physicianState`, `physicianZip`
   - `wasTreatedInER` — was the associate treated in the emergency room?
   - `wasHospitalizedOvernight` — were they hospitalized overnight?

5. **Case details** — Ask for:
   - `caseNumber` — OSHA case number if applicable
   - `completedBy` — who is completing this report?
   - `completedByTitle`, `completedByPhone`

6. **Notes** — Any additional notes.

7. **Review and confirm** — Show a complete summary before creating. Ask the user to confirm.

8. **Create** — Call `create_injurie` with the collected data. Show the result.

This is a compliance-sensitive form. Be thorough and make sure nothing is missed.
