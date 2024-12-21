# Express.js Route Parameter Type Error

This repository demonstrates a common error in Express.js applications related to route parameter parsing and error handling.  Specifically, it focuses on the scenario where a route parameter is expected to be a number, but the incoming request provides a non-numeric value.

## Bug Description
The provided code snippet defines an Express.js route that expects a numeric user ID as a parameter.  However, it lacks proper error handling for cases where the parameter is not a valid number. This could lead to unexpected behavior or crashes due to type coercion failures or attempts to access non-existent properties.

## Solution
The solution adds input validation and robust error handling to prevent the application from crashing. It explicitly checks for the correct data type before attempting any operations and returns appropriate error responses.