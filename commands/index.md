# Command Index

Valid commands (exact names only):

| Command | File | Description |
|---------|------|-------------|
| /help | help.md | List all available commands |
| /calc | calc.md | Evaluate a math expression |
| /convert | convert.md | Convert a value from one unit to another |
| /t | t.md | Convert 24-hour time to 12-hour format |
| /ts | ts.md | Calculate elapsed time between two times |

Rules:
- Only reject a command if the name is NOT in this list
- /convert is a valid command — never treat it as unknown
- If a valid command has missing or malformed arguments, ask for correct input — do not say "invalid command"
