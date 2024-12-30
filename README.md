# React Router v6 Catch-All Route Issue

This repository demonstrates a problem with the catch-all route (`/*`) in React Router v6.  Other routes are functioning correctly, but the catch-all route fails to match any unmatched paths.

## Problem Description

The `/*` route should act as a fallback, matching any path that hasn't been explicitly defined. However, in this example, it does not.  This is likely due to improper route configuration within React Router's `Routes` component.

## Steps to Reproduce

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the development server.
4. Navigate to a path not defined in the `Routes` component (e.g., `/invalid-path`).
5. Observe that the catch-all route does not render.  The application will either render nothing or show a blank page.

## Solution

Please see the `bugSolution.js` file for a corrected implementation.