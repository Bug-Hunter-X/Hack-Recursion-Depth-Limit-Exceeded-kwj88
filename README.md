# Hack Recursion Depth Limit

This repository demonstrates a common error in Hack: exceeding the recursion depth limit.  The `foo` function calculates the factorial of a number using recursion.  While this is a conceptually simple approach, it's not suitable for large inputs because Hack has a limited recursion depth.

The `bug.hack` file contains the code that produces the stack overflow.  The `bugSolution.hack` file offers a solution using iteration to avoid recursion and resolve the stack overflow issue.

## How to Reproduce

1.  Clone this repository.
2.  Compile and run `bug.hack` with a relatively large input for `x` (e.g., `x = 2000`).
3.  Observe the stack overflow error.
4.  Compile and run `bugSolution.hack` with the same input. Note that it executes without error.

## Solution

The solution involves rewriting the factorial calculation using iteration instead of recursion. This avoids exceeding the recursion depth limit and works reliably for larger input values.  See `bugSolution.hack` for the iterative implementation.