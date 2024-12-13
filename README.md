# React useEffect Hook Bug
This repository demonstrates a common bug in React's `useEffect` hook involving an incorrect conditional statement.

## Description
The `MyComponent` component uses the `useEffect` hook to log a message when the `count` state variable is greater than 0. However, the condition `count > 0` is incorrect because it does not handle the case where `count` is decremented to 0.  This leads to the effect not being triggered when the count goes from 1 to 0. 

## Solution
The solution involves modifying the conditional statement to include the case where `count` is equal to 0.