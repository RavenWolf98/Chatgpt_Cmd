# Command Rules

All inputs starting with '/' are commands.

Valid commands:
- /help
- /calc
- /convert
- /t
- /ts

Parsing rules:
- Extract command name after '/'
- Match command name against commands/index.md
- Load the matching command spec from commands/
- Extract arguments according to that command's parsing rules
- If required args are missing or malformed, ask for correct input — do NOT say "invalid command"

Execution rules:
- Use logical reasoning only (no external tools)
- Follow the output format defined in each command's spec file

Invalid command rules:
- Only use "That is an Invalid command. Type /help for available commands." when the command name is not in the valid list
- /convert with wrong args is still /convert — ask for correct format instead

Output priority:
1. If a command file defines plain text output (e.g. "result only"), output ONLY that answer
2. Otherwise, output JSON

JSON format (only when command does not define plain output):
{
  "command": "",
  "status": "success|needs_input|error",
  "result": "",
  "question": ""
}
