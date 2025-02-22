# React Native AsyncStorage: Handling Asynchronous Data Retrieval

This repository demonstrates a common error when using AsyncStorage in React Native: accessing data before it has been fully retrieved from storage.  This often leads to errors like "undefined is not an object (evaluating 'data.someProperty')".

The `bug.js` file shows the problematic code, and `bugSolution.js` presents the corrected version.

## Problem

Incorrectly handling the asynchronous nature of `AsyncStorage.getItem` can cause the application to attempt to render a component with undefined data.

## Solution

The solution involves correctly using the `useEffect` hook and conditional rendering to handle the asynchronous operation and avoid accessing data before it is available.

## How to Run

1. Clone this repository.
2. Navigate to the directory in your terminal.
3. Run `npm install` to install dependencies.
4. Run `npx react-native run-android` (or `npx react-native run-ios`) to start the app.