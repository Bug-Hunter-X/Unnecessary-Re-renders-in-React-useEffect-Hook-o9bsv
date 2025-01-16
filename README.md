# Unnecessary Re-renders in React useEffect Hook

This example demonstrates a common issue in React applications where the `useEffect` hook runs after every render, leading to unnecessary re-renders and potential performance problems. 
The `useEffect` hook in the provided code lacks a dependency array. As a result, it runs after every render of the component, even when the `count` state hasn't changed. This leads to the message 'Component rendered with count:' being logged to the console every time the component re-renders, which is unnecessary and indicates potential performance issues. 
The solution is to add a dependency array to specify that the effect should only run when the `count` state value changes.
