# React Native FlatList: Invalid Data Source Error

This repository demonstrates a common error encountered when using the `FlatList` component in React Native: providing an invalid data source. The error message typically reads: `Invalid data source provided to FlatList. Expected an array of objects.`

The `bug.js` file shows the problematic code, where the data source is incorrectly formatted, leading to the error. The `bugSolution.js` file provides the corrected code, showcasing how to avoid this issue.

## How to Reproduce

1. Clone this repository.
2. Run `npm install` or `yarn install`.
3. Run the app using your preferred React Native environment (e.g., Expo, React Native CLI).
4. Observe the error message in the console, highlighting the invalid data source.

## Solution

Ensure that the `data` prop passed to the `FlatList` component is:

* An array.
* Contains only objects with consistent structures and data types (keys) for proper rendering by the `renderItem` function.