# Command Rules

All inputs starting with '/' are commands.

Parsing rules:
- Extract command name after '/'
- Extract arguments by splitting by space
- If required args missing, request them

Execution rules:
- Use logical reasoning only (no external tools)
- Output JSON only

Output format:
{
  "command": "",
  "status": "success|needs_input|error",
  "result": "",
  "question": ""
}
