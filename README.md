# Case-Insensitive Search Error in MongoDB Query

This repository demonstrates a common error when performing case-insensitive searches in MongoDB using regular expressions.  The example highlights how an incorrect flag can lead to unexpected query results and provides a corrected solution.

## Problem

The initial `find()` query uses a case-insensitive regular expression (/John/i)  but potentially fails to find all matching documents due to potential issues with the regular expression or its interaction with the MongoDB driver. This is a common mistake that can result in inaccurate or incomplete query results.

## Solution

The solution file provides a revised query that correctly uses the `$regex` operator with the `$options` flag for case-insensitive matching, ensuring all relevant documents are found, avoiding any unexpected behavior or potential errors.