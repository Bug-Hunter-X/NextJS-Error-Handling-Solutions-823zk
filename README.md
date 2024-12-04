# Unhandled Runtime Error in Next.js About Page

This repository demonstrates a common yet easily missed error in Next.js applications: unhandled runtime errors that crash the client-side rendering.  The `about.js` page attempts to access a variable that hasn't been defined, resulting in a JavaScript error.

## Problem

The `about.js` file contains a runtime error.  This error isn't gracefully handled, causing the entire page to crash and display a blank screen or an error message in the browser's console.

## Solution

The solution involves adding error boundaries to catch and gracefully handle these exceptions.  The `aboutSolution.js` file demonstrates the use of React's error boundaries to render a fallback UI instead of crashing the page.

## How to Reproduce

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npm run dev` to start the Next.js development server.
4. Navigate to `/about` in your browser. You'll see the error.
5. Observe the fix in the solution file.