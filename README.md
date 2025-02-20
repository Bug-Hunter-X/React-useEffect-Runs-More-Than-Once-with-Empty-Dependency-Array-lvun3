# React useEffect Runs More Than Once with Empty Dependency Array

This repository demonstrates a subtle bug related to the `useEffect` hook in React.  The `useEffect` hook, with an empty dependency array (`[]`), is expected to run only once after the initial render. However, due to a common misunderstanding, it may appear to run multiple times.

## Problem

The provided `MyComponent` uses `useEffect` with an empty dependency array. Despite this, the effect's code will log multiple times to the console.

## Solution

The solution involves a deeper understanding of React's rendering cycle and the role of the dependency array in the `useEffect` hook.  The corrected code ensures the effect runs only once, as intended.