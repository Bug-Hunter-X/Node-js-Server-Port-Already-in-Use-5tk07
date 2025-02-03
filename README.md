# Node.js Server Port Already in Use

This repository demonstrates a common error encountered when starting a Node.js HTTP server: the specified port is already in use.

The `server.js` file contains the problematic code.  The `serverSolution.js` file shows how to gracefully handle this scenario.

## Bug Description

The server fails to start, producing an unhelpful error message which doesn't clearly indicate the port in use. This makes debugging difficult.

## Bug Solution

The solution involves using the `'listening'` event and error handling to gracefully manage port conflicts.  This solution checks if the port is in use before starting the server and provides informative feedback to the user.