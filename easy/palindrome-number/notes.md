# Palindrome Number Solution

## Approach
- **Negative numbers** and numbers ending with **0** (except 0 itself) are not palindromes.
- Instead of reversing the entire number (which may cause overflow or extra space), reverse **half** of it.
- Compare the original half (`x`) with the reversed half (`reversed_half`).
- Works for both even and odd digit counts:
  - For odd lengths, drop the middle digit (`reversed_half // 10`) before comparing.

## Time Complexity
- **O(log₁₀(n))** — We process half the digits of the number.

## Space Complexity
- **O(1)** — Constant space, no extra data structures used.