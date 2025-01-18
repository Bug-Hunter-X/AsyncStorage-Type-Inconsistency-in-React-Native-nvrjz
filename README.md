# AsyncStorage Type Inconsistency Bug in React Native

This repository demonstrates a common, yet easily overlooked, bug in React Native's AsyncStorage.  The problem lies in the inconsistent type handling of AsyncStorage's `getItem` method.  Regardless of the type of data originally stored (number, object, or string), `getItem` always returns a string. This can lead to unexpected type errors and incorrect program behavior.

The `bug.js` file showcases the buggy code, and `bugSolution.js` demonstrates how to resolve the issue using JSON.parse() for object retrieval and parseInt() for numerical data.

## How to Reproduce

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run the app on an emulator or physical device.
4. Observe the console for errors and incorrect output in `bug.js`.
5. Compare with the correct output and type handling in `bugSolution.js`.