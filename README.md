# React Navigation useNavigation Hook Returning Null

This repository demonstrates a common issue in React Native applications using React Navigation: the `useNavigation` hook returning `null`.  This typically happens when the hook is used outside the context of a screen managed by a React Navigation navigator.

The `bug.js` file showcases the problematic code, while `bugSolution.js` presents a corrected implementation.

## How to Reproduce

1. Clone this repository.
2. Run `npm install` or `yarn install`.
3. Run the app using your preferred React Native method (e.g., `npx react-native run-android` or `npx react-native run-ios`).
4. Observe the error or unexpected behavior.

## Solution

The solution involves ensuring that the `useNavigation` hook is used within a component that is directly or indirectly a child of a React Navigation screen component. Refactoring your component tree or using techniques like context providers may be necessary depending on your application's architecture.