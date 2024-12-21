# Unhandled Asynchronous Error in Node.js
This repository demonstrates a common error in Node.js applications involving unhandled asynchronous errors and provides a solution.

## The Problem
The `bug.js` file contains an Express.js app with a route that simulates an asynchronous operation.  Sometimes, this operation throws an error, but the error isn't caught, causing the server to crash silently. This is a classic example of an unhandled promise rejection or uncaught exception in asynchronous code.

## The Solution
The `bugSolution.js` file shows how to properly handle the error using a `try...catch` block within the asynchronous function or by handling promise rejections using `.catch()`, making the application more robust and preventing unexpected crashes.