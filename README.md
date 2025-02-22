# Express.js Route Handler Missing Error Handling for Invalid User ID

This repository demonstrates a common error in Express.js route handlers: missing error handling for invalid input. Specifically, the provided code attempts to parse a user ID from the request parameters as an integer without any validation. If the ID is not a number, the `parseInt()` function will return `NaN`, leading to potential errors or unexpected behavior.

The `bug.js` file contains the erroneous code. The `bugSolution.js` file provides a corrected version with added error handling to prevent unexpected crashes or failures and ensure a more robust and reliable application.

## How to Reproduce

1. Clone the repository.
2. Run `npm install` to install the necessary dependencies.
3. Run `node bug.js`. Attempt to access a route with a non-numeric ID (e.g., `/users/abc`).
4. Observe the error or unexpected behavior.
5. Run `node bugSolution.js` to see the corrected code in action.