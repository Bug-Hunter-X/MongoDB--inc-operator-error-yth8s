# MongoDB $inc Operator Error

This repository demonstrates a common error when using the `$inc` operator in MongoDB update queries.  The `$inc` operator is designed to increment a numeric field by a specified value.  However, if a string is provided instead of a number, the update operation will fail silently or produce unexpected results.

## Bug Description
The code attempts to increment the `field` in a document where the `_id` is 1. However, instead of providing a numerical increment value, it provides the string '1'. This will lead to an error or unexpected behavior.

## Solution
The solution involves providing the correct numeric value for the increment.