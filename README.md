# Javascript Bug: Handling Null and Undefined Values

This repository demonstrates a common issue in JavaScript related to handling null and undefined values. The `foo` function adds two numbers, but it doesn't handle the cases where one or both arguments are undefined. This can lead to unexpected behavior or errors.

## Bug Description

The original `bug.js` file contains a function that handles null values correctly but doesn't consider undefined values. This results in unexpected behavior when undefined values are passed as arguments.

## Solution

The solution in `bugSolution.js` addresses the issue by explicitly checking for both null and undefined values using the loose equality operator (`==`).  This ensures that the function behaves consistently in all cases.

## How to reproduce the bug
1. Clone the repository
2. Run `node bug.js` and observe the output for various inputs, including undefined values.

## How to fix the bug
1. Replace `bug.js` with `bugSolution.js`
2. Run `node bugSolution.js` and observe the improved output.

This example highlights the importance of considering both null and undefined values when working with potentially missing data in JavaScript. Using strict equality (`===`) could also be considered for stricter type checking depending on specific needs.