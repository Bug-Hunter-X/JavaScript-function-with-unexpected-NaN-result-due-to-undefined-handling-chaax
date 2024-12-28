# JavaScript Function with Unexpected NaN Result

This repository demonstrates a common JavaScript bug related to how the code handles `undefined` values. The function `foo` intends to add two numbers, but it produces an unexpected `NaN` result when one of the inputs is `undefined`. 

## Bug Description
The bug lies in the way the function handles undefined values. While it correctly handles null values by returning 0, it doesn't explicitly check for `undefined`, leading to an unexpected `NaN` result. 

## How to Reproduce
1. Clone this repository.
2. Run the `bug.js` file using Node.js (or a similar JavaScript environment).
3. Observe the unexpected `NaN` result when calling `foo` with an `undefined` argument.

## Solution
The solution involves explicitly checking for `undefined` values along with null values, similar to how null values are already being handled.