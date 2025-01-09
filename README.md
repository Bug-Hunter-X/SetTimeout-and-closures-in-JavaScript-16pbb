# setTimeout and Closures in JavaScript

This repository demonstrates a common issue encountered when using `setTimeout` within a loop in JavaScript involving closures.  The code intends to log numbers 0-9 with a one-second delay, but due to how closures work with `setTimeout`, it unexpectedly logs 10 ten times.

The `bug.js` file contains the erroneous code. The `bugSolution.js` file demonstrates the corrected version using an immediately invoked function expression (IIFE) to create a new scope for each iteration of the loop, preserving the correct value of `i`.