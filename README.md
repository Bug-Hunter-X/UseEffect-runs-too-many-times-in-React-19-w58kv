# React 19 useEffect Bug
This repository demonstrates a common bug in React 19 related to the `useEffect` hook running more frequently than expected.  The example shows a simple counter component where the `useEffect` hook is intended to log a message only when the count changes. However, due to a misunderstanding of the `useEffect`'s behavior in React 19, it runs on every render causing unnecessary console logs and potential performance issues.

## Bug Description
The `useEffect` hook, even with a dependency array specified, runs multiple times unexpectedly in React 19.

## Solution
The solution involves reviewing the component's logic and dependencies to ensure the useEffect hook only runs when necessary. For this particular example, double-checking the specified dependencies within the dependency array and making sure it is correctly specified guarantees the desired behavior.