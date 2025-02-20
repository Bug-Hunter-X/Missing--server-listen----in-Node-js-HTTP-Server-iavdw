# Missing 'server.listen()' in Node.js HTTP Server

This repository demonstrates a common error in Node.js where the `server.listen()` method is missing, preventing the HTTP server from starting.  The `bug.js` file contains the erroneous code.  The solution is provided in `bugSolution.js`.

## Bug

The `bug.js` file creates an HTTP server but fails to start it because it omits the crucial `server.listen()` call. This leads to a server that doesn't respond to any requests.

## Solution

The `bugSolution.js` file corrects the issue by adding the `server.listen()` method, specifying the port to listen on, and adding an error handling callback to gracefully handle any startup errors.