# Incorrect Usage of $inc Operator in MongoDB
This repository demonstrates a common error when using the `$inc` operator in MongoDB update operations. The error occurs when a string is used instead of a number for the increment value, leading to an unexpected outcome.

## Bug Description
The `$inc` operator is used to increment a numeric field in a MongoDB document.  The provided code attempts to increment the `field` by `'1'`, which is a string, not a number. MongoDB will not increment the field properly and the update might fail or produce unexpected results.

## Solution
The solution involves using a numeric value instead of a string when using `$inc`. The updated code shows the correct usage of the `$inc` operator using a numeric value for incrementing the field.

## How to Reproduce the Bug
1. Run the script `bug.js`.
2. Observe that the field is not incremented as expected.