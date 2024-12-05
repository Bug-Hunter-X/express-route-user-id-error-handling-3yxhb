# Unhandled Error: Invalid User ID in Express Route

This repository demonstrates a common error in Express.js route handlers:  the lack of proper error handling when dealing with user input.  The example shows a route that fetches a user by ID, but fails to handle cases where the ID is not a valid number.

## Bug

The `bug.js` file contains the erroneous code.  It attempts to parse the user ID as an integer without any error handling. If a non-numeric ID is provided, `parseInt` will return `NaN`, leading to a failed search and no appropriate error response.

## Solution

The `bugSolution.js` file provides the corrected code. It includes explicit checks to ensure the user ID is a valid number before attempting to parse it and handles the case where the user is not found.