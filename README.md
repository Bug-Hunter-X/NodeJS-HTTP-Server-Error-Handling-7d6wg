# Unhandled Exception in Node.js HTTP Server

This repository demonstrates an example of an unhandled exception in a Node.js HTTP server and provides a solution to handle it gracefully.  Improper error handling can lead to unexpected server crashes and a poor user experience.

## Bug

The `bug.js` file contains a Node.js HTTP server that lacks proper error handling.  If a client requests the `/error` endpoint, an uncaught exception is thrown causing the server to crash.

## Solution

The `bugSolution.js` file provides a solution that uses a `try...catch` block to handle the exception gracefully.  This prevents the server from crashing and allows for more robust error handling.

## How to Reproduce

1. Clone this repository.
2. Navigate to the directory.
3. Run `node bug.js`.
4. Access `http://localhost:3000/error` in your browser. Observe the server crashing.
5. Run `node bugSolution.js`.
6. Access `http://localhost:3000/error` again. Observe the graceful error handling.