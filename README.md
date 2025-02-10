# React Native Null Access Error

This repository demonstrates a common error in React Native applications: attempting to access a property of an object before it's fully initialized.  The error typically manifests as a null pointer exception, and this example shows how to handle and prevent it. 

## Bug
The `bug.js` file contains code that attempts to render data from a state variable before the data has been fetched asynchronously. This leads to a null value being accessed, causing the app to crash.

## Solution
The `bugSolution.js` file shows the corrected code. It uses optional chaining and nullish coalescing to safely access the data, preventing the error.  Additionally, it uses a loading state to handle the asynchronous operation gracefully.

## Setup
1. Clone this repository.
2. Navigate to the project directory.
3. Run `npm install` to install the necessary packages.
4. Run `npx react-native run-android` or `npx react-native run-ios` to start the app.