# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React's `useEffect` hook: creating an infinite loop by incorrectly updating state within the dependency array.  The `bug.js` file contains the buggy code. The `bugSolution.js` file provides the corrected version.

## Bug Description
The bug occurs due to the incorrect dependency array in the `useEffect` hook. When `count` is updated, it triggers the `useEffect` function again, causing an infinite loop of state updates.  This leads to performance issues and potential crashes.

## Solution
The solution modifies the dependency array to prevent the infinite loop.  Details are in `bugSolution.js`.