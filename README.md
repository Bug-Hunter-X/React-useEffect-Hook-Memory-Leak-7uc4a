# React useEffect Hook Memory Leak

This example demonstrates a common error in React's `useEffect` hook: forgetting to include a cleanup function to handle asynchronous operations.

The `bug.js` file shows the incorrect implementation, leading to potential memory leaks if the component unmounts before the fetch completes.  The solution, shown in `bugSolution.js`, demonstrates the correct use of cleanup functions in `useEffect` to avoid these issues.