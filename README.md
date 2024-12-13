# Incorrect Use of $inc Operator in MongoDB

This example demonstrates an uncommon error in MongoDB update operations that involves the `$inc` operator. The `$inc` operator is used to increment a numeric field by a specified value.  However, if a string is provided as the increment value, instead of an integer or a floating point number, the update operation might not produce the expected results.

## Bug
The `bug.js` file shows the incorrect usage of the `$inc` operator.  This code attempts to increment the `count` field by '1' (string), which is an invalid input, and will not increment the value properly.

## Solution
The `bugSolution.js` file demonstrates the correct usage of the `$inc` operator.  The increment value should be a number.