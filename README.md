# React useEffect Infinite Loop Bug

This repository demonstrates a common bug in React applications involving the `useEffect` hook.  The bug is caused by an infinite loop triggered by incorrectly updating state within the `useEffect` hook's dependency array.

## Bug Description

The `MyComponent` function uses the `useEffect` hook to update the `count` state. However, the update happens within the useEffect itself and without a condition to stop, resulting in an infinite render loop.