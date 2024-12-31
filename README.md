# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React's `useEffect` hook that leads to an infinite loop.  The problem stems from incorrectly updating the state within the `useEffect`'s callback without proper dependency management.

## Bug Description
The `MyComponent` attempts to increment the `count` state within the `useEffect` hook's callback without any dependencies. This causes the `useEffect` to re-run endlessly because each update to `count` triggers another update, creating an infinite loop.

## Solution
The provided solution demonstrates the correct way to use `useEffect` to prevent this error.
