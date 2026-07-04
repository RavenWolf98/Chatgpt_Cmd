# /convert - Unit Conversion

Input:
 /convert value from_unit to to_unit

Description:
Convert a numeric value from one unit to another.

Parsing rules:
- Command name is: convert
- Format: /convert <number> <from_unit> to <to_unit>
- The word "to" separates source and target units
- Units may be one or more words (e.g. km, miles, feet, celsius, fahrenheit)

Examples:
 /convert 10 km to miles
 /convert 100 celsius to fahrenheit
 /convert 5 feet to inches

Rules:
- Use logical reasoning and standard conversion factors
- No external tools
- If arguments are missing or malformed, ask for correct format — do not treat as invalid command

Output:
result only (plain text, no JSON)

Format:
- Return converted value with target unit only
- Example: 6.21 miles
- Do not wrap in JSON
- Do not include any other text
