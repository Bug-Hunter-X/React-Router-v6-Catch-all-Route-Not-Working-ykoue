# React Router v6 Catch-all Route Issue

This repository demonstrates a problem with the catch-all route ('/*') in React Router v6.  The issue is that the catch-all route is not being triggered when a user navigates to a non-existent path.  All other routes are functioning correctly.

## Steps to reproduce

1. Clone the repository.
2. Run `npm install` to install the dependencies.
3. Run `npm start` to start the development server.
4. Navigate to any non-existent route (e.g., '/invalid-path').  The '404 Not Found' component should be displayed, but it's not.

## Solution

The solution is provided in the AppSolution.js file.  The problem was the order of the Routes in App.js. The catch-all route must always be placed last.