# MongoDB $inc Operator Error

This repository demonstrates an incorrect usage of the MongoDB `$inc` operator within an `updateOne` operation.  The error arises from attempting to increment a field using a string value instead of a number. This leads to unexpected behavior and potential data corruption.  The solution shows how to correct the operation for accurate field incrementation.

## Bug
The bug lies in the use of the `$inc` operator. The provided code attempts to increment the 'field' by '1', which is a string.  The `$inc` operator requires a numeric value.

## Solution
The correct way to increment the 'field' is to pass a numeric value, in this case, 1.