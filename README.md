# Unhandled Error in Express.js Route Parameter

This repository demonstrates a common error in Express.js route handlers: the lack of proper error handling when dealing with user-provided parameters. The `bug.js` file contains the erroneous code, while `bugSolution.js` provides a corrected version.

The bug arises from directly parsing a route parameter (`req.params.id`) as an integer without validating its format.  If the ID isn't a valid number, `parseInt()` will return `NaN`, leading to unexpected behavior or potential application crashes. The solution implements robust error handling to gracefully manage these situations.