# React useEffect Hook Runs on Every Render

This repository demonstrates a common issue with React's `useEffect` hook and its solution.  The problem arises when the dependency array is missing or incorrect, causing the effect to run unexpectedly on every render. This is usually due to an incorrect or missing dependency array.   This extra rendering can lead to performance issues and unexpected behavior.

## Bug

The `bug.js` file contains a React component that uses `useEffect` to log the current count. Without the dependency array, the effect runs on every render, even when the count doesn't change. This can lead to unnecessary re-renders and potential performance problems.

## Solution

The `bugSolution.js` file shows the corrected implementation.  By adding `[count]` as the dependency array, the `useEffect` hook runs only when the value of `count` changes, resolving the issue. 

## How to run
1. Clone the repository
2. Run  `npm install`
3. Run `npm start`