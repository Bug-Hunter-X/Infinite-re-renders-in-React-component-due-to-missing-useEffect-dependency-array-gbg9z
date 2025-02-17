# React useEffect Infinite Loop Bug

This repository demonstrates a common bug in React applications involving the `useEffect` hook.  The bug arises from a missing dependency array, leading to an infinite loop of renders.

## Bug Description
The provided `MyComponent` uses `useEffect` without specifying a dependency array. This causes the effect to run after every render, creating a continuous loop and potentially crashing the browser.

## Solution
The solution involves adding a dependency array to `useEffect`. In this case, `[count]` ensures the effect only runs when the `count` state variable changes.