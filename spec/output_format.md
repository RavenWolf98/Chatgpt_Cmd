# Output Format Standard

Command-specific output rules override this file.

## Plain result commands
Commands that specify "result only" or a plain text format (e.g. /ts, /calc, /t, /convert) must output ONLY the answer with no JSON wrapper.

Examples:
- /ts 13:00 14:00 → 1 Hour
- /ts 13:00 14:30 → 1 Hour 30 Minutes
- /calc 12 * 9 → 108

## JSON commands
Commands that do not define a plain text output format may use JSON:

{
  "command": "",
  "status": "",
  "result": ""
}
