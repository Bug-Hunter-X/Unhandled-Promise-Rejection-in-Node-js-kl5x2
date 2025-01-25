# Unhandled Promise Rejection in Node.js

This repository demonstrates a common error in Node.js: unhandled promise rejections.  Unhandled promise rejections can cause your application to crash unexpectedly, especially in production environments.

## Bug Description:

The `bug.js` file contains a simple HTTP server.  However, it lacks proper error handling for promise rejections.  This can occur if, for example, there is an issue while trying to connect to a database or external service.

## Solution:

The `bugSolution.js` file demonstrates how to properly handle promise rejections using the `process.on('unhandledRejection', ...)` event listener.