# React Router Dom v6 Catch-all Route Issue

This repository demonstrates a common issue encountered when using catch-all routes (`/*`) in React Router Dom v6.  The catch-all route, intended to handle non-matching routes, unexpectedly overrides other defined routes.

## Problem
The provided example shows that the `NotFound` component (defined with `/*` path) is always rendered, even when valid routes like `/` or `/about` are accessed.

## Solution
The solution involves reordering the routes. The catch-all route (`/*`) must be placed last in the `Routes` component to ensure it only matches routes not covered by other routes.