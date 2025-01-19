# RecursionError in Factorial Function

This repository demonstrates a common error in recursive functions: the lack of a proper base case leading to a `RecursionError: maximum recursion depth exceeded`. The `factorial` function is implemented recursively, but it doesn't handle negative input values which cause infinite recursion.

The `bug.py` file shows the faulty implementation, while `bugSolution.py` provides a corrected version.

## Bug Description

When the function receives a negative input, it recursively calls itself indefinitely, leading to the error. Python has a recursion depth limit to prevent stack overflow. 

## Solution

The solution involves adding a check for negative input, returning an appropriate value (e.g., `ValueError`), or handling it differently.  The corrected version is in `bugSolution.py`.