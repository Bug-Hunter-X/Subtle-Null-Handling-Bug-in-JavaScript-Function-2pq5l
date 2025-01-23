# Subtle Null Handling Bug in JavaScript

This repository demonstrates a common, yet subtle, bug in JavaScript related to null value handling. The `foo` function aims to add two numbers, but its null handling is incomplete.

## Bug Description
The `foo` function correctly returns `null` if either input is `null`. However, it lacks a mechanism to handle cases where one input is a number and the other is `null`.  This can lead to unexpected behavior or errors if not properly addressed.

## How to Reproduce
1. Clone this repository.
2. Run the `bug.js` file using a JavaScript runtime (e.g., Node.js).
3. Observe the output, noting that the function returns `null` even when one argument is a valid number and the other is `null`. 

## Solution
The solution (`bugSolution.js`) demonstrates a more robust approach by using loose comparison (`==`) which will properly handle null and undefined values and add them as 0.  Alternatively, you can use a ternary operator for a more concise solution.