# React useEffect Cleanup Function Issue

This repository demonstrates a common issue encountered when using the `useEffect` hook in React: the cleanup function not executing as expected.  The example showcases an effect with a cleanup function that should be triggered upon unmounting the component, but fails to do so under certain conditions.

## Problem

The provided `MyComponent` utilizes `useEffect` with an empty dependency array, indicating it should only run once after the initial render. While the initial log statement executes correctly, the cleanup function fails to run when the component is unmounted.  This can lead to unexpected behavior, such as memory leaks or lingering side effects. 