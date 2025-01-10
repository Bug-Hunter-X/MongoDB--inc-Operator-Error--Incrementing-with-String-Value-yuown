# MongoDB $inc Operator Error

This repository demonstrates an uncommon error that can occur when using the `$inc` operator in MongoDB update operations.

The error arises from attempting to increment a numeric field with a string value.

## Bug Description

The provided `bug.js` file contains incorrect code that attempts to increment the `age` field of a document with a string value ('1') rather than a numeric value (1).

## Solution

The `bugSolution.js` file shows the corrected implementation of the `$inc` operator.

The key to resolving this bug is to ensure you use numeric values for incrementing fields using `$inc`. String values will not increment the field, but instead result in an error or incorrect behaviour.