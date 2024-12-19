# MongoDB Aggregation Pipeline Bug: Unexpected $inc Behavior

This repository demonstrates an uncommon error related to the `$inc` operator within MongoDB's aggregation pipeline.  The issue stems from attempting to increment a field that does not yet exist within an embedded document. The code appears to run without error, but produces unexpected aggregation results.

The `bug.js` file contains the erroneous code, highlighting the problematic usage of `$inc`. The `bugSolution.js` file provides the corrected code demonstrating how to properly handle creating and incrementing fields using the aggregation framework.

This issue is particularly subtle because it doesn't throw an error, making it difficult to detect.  The solution clarifies the correct way to achieve the desired outcome.
