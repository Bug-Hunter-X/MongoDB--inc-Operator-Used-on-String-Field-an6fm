# MongoDB $inc Operator with String Field
This example demonstrates an incorrect usage of the MongoDB `$inc` operator, attempting to increment a string field.  The `$inc` operator is designed to increment numeric values and will throw an error when used incorrectly.

## Bug
The `bug.js` file shows the erroneous usage of `$inc` with a string field. This results in an error because the operator is applied to a non-numeric type.

## Solution
The `bugSolution.js` file presents the corrected approach, which involves ensuring that the target field is a number before attempting to increment it using the `$inc` operator. If necessary it also shows how to properly convert the field to a number.