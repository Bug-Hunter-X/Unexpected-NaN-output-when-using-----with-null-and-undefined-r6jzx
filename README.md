# Unexpected NaN output when using === with null and undefined
This code demonstrates an unexpected behavior in JavaScript when using the strict equality operator (===) with null and undefined values.
The function `foo` is designed to check if the input `x` is null. If so, it returns 0. Otherwise, it adds 1 to `x` and returns the result.
However, when the input is `undefined`, the function returns `NaN` instead of handling it gracefully (e.g., returning a default value or throwing an error). This is because `undefined + 1` results in `NaN`.
The solution provides an improved version of the function that explicitly checks for both `null` and `undefined`, handling them appropriately.