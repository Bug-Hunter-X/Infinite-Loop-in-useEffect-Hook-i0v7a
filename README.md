# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React's `useEffect` hook: an infinite loop caused by improperly managing dependencies.

The `bug.js` file contains the buggy code, where the effect runs on every render, leading to an infinite loop.  The `bugSolution.js` file provides the corrected code, showcasing the proper use of dependency arrays in `useEffect`.

## How to Reproduce

1. Clone this repository.
2. Navigate to the project directory.
3. Run `npm install` (or `yarn install`).
4. Run `npm start` (or `yarn start`).
5. Observe the console log and the behavior of the counter.

## Solution

The issue is fixed by correctly specifying the dependencies array in `useEffect`. Only when 'count' changes, the effect will run.