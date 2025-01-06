# Express.js JSON Body Parsing Error
This repository demonstrates a common issue in Express.js applications where the `express.json()` middleware fails to correctly handle empty or invalid JSON request bodies.

## Bug Description
The provided Express.js application attempts to parse the JSON request body using `express.json()`. However, if the request body is empty or contains invalid JSON data, the application will either throw an error or fail to correctly process the request.

## Bug Solution
The solution addresses this issue by adding error handling to gracefully handle cases where the request body is empty or not valid JSON.  This is done by checking the request body before attempting to access its properties.