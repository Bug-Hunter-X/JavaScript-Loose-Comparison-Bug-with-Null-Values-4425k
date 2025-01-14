# JavaScript Loose Comparison Bug with Null Values

This repository demonstrates a common JavaScript bug related to loose comparison (==) with null values.  The `foo` function demonstrates the problem where using loose comparison results in unexpected behavior when null is passed as an argument. Using strict equality (===) resolves this.

## Bug Description
When null values are passed into the `foo` function and a loose comparison is performed, the code unexpectedly continues execution even when a check for null is present.

## Bug Solution
The solution uses strict equality (`===`) to accurately check for null values. This ensures the code behaves as intended, returning early when either `a` or `b` is null.