# React useEffect Hook Bug

This repository demonstrates a common bug in React applications involving the `useEffect` hook and its dependency array. The `MyComponent` component uses `setInterval` to update a counter every second, but the dependency array is missing the `count` variable, causing the effect to run repeatedly, resulting in an extremely fast-updating counter.

The solution shows how to fix the issue by correctly including `count` in the dependency array.  This ensures the effect only runs when the `count` value changes.