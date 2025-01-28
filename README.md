# React useEffect Cleanup Function Missing Return Statement

This example demonstrates a common error in React's `useEffect` hook: omitting the return statement for the cleanup function. This can lead to memory leaks and unexpected behavior.

## Bug

The `bug.js` file contains a `MyComponent` that uses `useEffect` to add an event listener.  However, it's missing the return statement that's necessary to remove the event listener when the component unmounts.

## Solution

The `bugSolution.js` file fixes this by adding the `return` statement, ensuring proper cleanup when the component is no longer needed.

## How to reproduce

1. Clone this repository.
2. Navigate to the directory containing the files.
3. Run `npm install` (or `yarn install`).
4. Run `npm start` (or `yarn start`).
5. Observe the behavior with and without the fix.