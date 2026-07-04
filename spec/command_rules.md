# Command Rules

All inputs starting with '/' are commands.

Parsing rules:
- Extract command name after '/'
- Extract arguments by splitting by space
- If required args missing, request them

Execution rules:
- Use logical reasoning only (no external tools)
- Follow the output format defined in each command's spec file

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
