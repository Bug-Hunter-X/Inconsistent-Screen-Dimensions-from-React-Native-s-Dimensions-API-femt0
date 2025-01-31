# Inconsistent Screen Dimensions in React Native

This repository demonstrates a common issue encountered when using the `Dimensions` API in React Native to obtain screen dimensions. The problem arises when the returned dimensions are incorrect or inconsistent, often resulting in layout problems.  This usually happens because of asynchronous loading of the dimensions. 

The `DimensionsBug.js` file showcases the problem, while `DimensionsBugSolution.js` provides a solution using `Dimensions.addEventListener` to handle dimension changes reliably.

## Steps to Reproduce

1. Clone this repository.
2. Run `npm install`.
3. Run the app on an emulator or device.
4. Observe the inconsistencies in the displayed dimensions.

## Solution

The provided solution uses `Dimensions.addEventListener` to listen for changes in screen dimensions and update the component's state accordingly. This ensures the app always uses the correct and up-to-date dimensions.