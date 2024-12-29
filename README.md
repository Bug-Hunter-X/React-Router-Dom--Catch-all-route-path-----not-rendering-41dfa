# React Router Dom Catch-All Route Issue

This repository demonstrates a problem with the catch-all route (`path="*"`) in `react-router-dom` when nested within other routes.  The `NotFound` component, intended to handle all non-existent URLs, fails to render correctly.

## Problem
The `path="*"` route is designed to act as a fallback, displaying a 404 Not Found page when the URL doesn't match any other defined routes.  However, in this example, it does not function as intended.  Even when navigating to a URL that doesn't match any other path, the default component is shown instead of the NotFound component. 

## Solution
The issue arises from improper nesting of routes. The solution uses a different approach for handling not found routes, which ensures it acts as a proper fallback.