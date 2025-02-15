# React Native: Unexpected Null Value When Accessing Object Property

This repository demonstrates a common React Native error: attempting to access a property of an object before it's been populated by asynchronous data, resulting in a null value error.  The solution shows proper null checks and conditional rendering to handle this situation gracefully.

## Bug
The `bug.js` file contains a component that fetches data asynchronously.  It attempts to render the fetched data's `name` property immediately, causing an error if the data hasn't finished loading and is still null.

## Solution
The `bugSolution.js` file demonstrates the corrected component. It uses optional chaining (?.) to safely access the `name` property and conditional rendering to prevent rendering before the data is available.