# Week 6 Assignment - Safe Functions

- `safe_tools.py` - Contains three functions (`safe_divide`, `safe_number`, `get_field`) that use try/except so the program never crashes.
- `README.md` - This file, describing the assignment and files.

## Why can the `if` check not catch `abc` on its own?
An `if` check can only test for conditions you thought of in advance, such as `b == 0`. Text like `"abc"` can fail `int()` in many ways, and you only find out when the conversion is attempted, so `try/except ValueError` is needed to catch the error as it happens.