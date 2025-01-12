# Handling Network Errors in React Native

This example demonstrates how to robustly handle network requests in a React Native application.  Unhandled network errors can lead to a poor user experience.  This example shows how to gracefully handle these errors and display appropriate messages to the user.

## Problem

Network requests can fail due to various reasons (server down, network issues, etc.).  Without proper error handling, your app might crash or silently fail, leaving the user confused.

## Solution

This example uses `async/await` and a `try...catch` block to handle potential errors during the fetch request.  A loading state is displayed while fetching, and informative error messages are shown if something goes wrong.  The `finally` block ensures the loading state is set to `false` regardless of success or failure.

## How to use

1.  Replace `'YOUR_API_ENDPOINT'` in `DataList.js` with your actual API endpoint.
2.  Run the app and observe the error handling.