# /ts - Time Since

Input:
 /ts HH:MM [HH:MM]

Description:
Calculate elapsed time between a start time and an end time.

Rules:
- First argument is the start time (HH:MM or HHMM)
- If a second argument is provided, use it as the end time
- If no second argument is provided, use the current time as the end time
- Convert both times to minutes
- Compute difference (end time minus start time)
- Return human readable duration

Examples:
 /ts 13:00
 → uses current time as end time

 /ts 13:00 14:00
 → 1 Hour

 /ts 13:00 14:30
 → 1 Hour 30 Minutes

Output:
result only (plain text, no JSON)

Format:
- Use singular/plural correctly: "1 Hour", "2 Hours", "1 Minute", "45 Minutes"
- When both hours and minutes apply, include both: "1 Hour 30 Minutes"
- Do not wrap in JSON
- Do not include any other text
