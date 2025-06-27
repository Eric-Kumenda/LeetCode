# Roman to Integer Solution

## Approach
- Use a **map** of Roman symbols to values.
- Traverse the string left to right:
  - If the current value is **less than the next**, **subtract** it.
  - Else, **add** it.
- Handles subtractive pairs like `IV`, `IX`, `XL`, etc.

## Time Complexity
- **O(n)** — One pass through the string of length *n*.

## Space Complexity
- **O(1)** — Fixed map size; no extra space used per input.