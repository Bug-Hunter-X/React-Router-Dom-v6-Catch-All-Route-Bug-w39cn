# React Router Dom v6 Catch All Route Bug

This repository demonstrates a common issue with the catch-all route (`/*`) in React Router Dom v6. The catch-all route, intended to handle unmatched routes, is incorrectly matching all routes, even specific routes defined before it.

## Problem
The `/*` route in `Routes` matches all other routes, preventing any routes defined after it from working.

## Solution
The issue is resolved by placing the `/*` catch-all route as the last route within the `Routes` component.  This ensures that more specific routes are matched before the catch-all.