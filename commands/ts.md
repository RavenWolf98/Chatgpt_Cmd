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
 → 1 hour

Output:
<number> hours or minutes
