# JavaScript Null Handling Bug

This repository demonstrates a common, yet subtle, bug in JavaScript related to handling null values within functions.  The `foo` function intends to add two numbers, returning null if either input is null. However, the current implementation may not behave as expected in all cases, especially with multiple null checks.

## Bug Description
The provided JavaScript code shows a simple addition function with null checks. While it functions correctly for valid numerical input, it returns `null` if *either* input is `null`. The issue arises from the strict equality check (`===`).

## Solution
The solution improves the null handling, enhancing clarity and potentially improving performance.  Instead of checking for null on both inputs simultaneously, the solution uses a guard clause. This reduces nesting and makes the code flow more straightforward.