# Unhandled Exception in Asynchronous Node.js Server

This repository demonstrates a common issue in Node.js applications: unhandled exceptions within asynchronous operations.  The server simulates an asynchronous task that randomly fails, causing a 500 Internal Server Error if no error handling is in place. The solution implements proper error handling to gracefully manage these exceptions.

## Bug

The `bug.js` file contains a Node.js HTTP server with a simulated asynchronous operation. This operation randomly fails, potentially leading to unhandled exceptions and inconsistent 500 errors.

## Solution

The `bugSolution.js` file shows how to correctly handle exceptions within the asynchronous operation, preventing unhandled rejections and ensuring robust error handling.  The solution uses a try...catch block to catch potential errors and gracefully respond to the client.