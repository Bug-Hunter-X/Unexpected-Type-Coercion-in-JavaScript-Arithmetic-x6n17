# Unexpected Type Coercion in JavaScript Arithmetic
This repository demonstrates a common, yet subtle, bug in JavaScript stemming from its dynamic typing system and how it handles type coercion during arithmetic operations. 

## The Bug
JavaScript's loose typing allows for implicit type conversions, which can lead to unexpected results, especially in arithmetic operations involving numbers and strings.  When adding a number and a string, the number is implicitly converted to a string, resulting in string concatenation. Subtraction, on the other hand, may lead to different type conversions, potentially yielding unexpected outcomes.  The example code showcases this unexpected behavior.

## The Solution
To avoid such issues, it's crucial to enforce type checking or use explicit type conversion before performing arithmetic operations.  The provided solution demonstrates how to use the `parseInt()` function to convert strings to numbers before calculating the sum and difference, ensuring accurate results.

## How to Reproduce
1. Clone this repository.
2. Open `bug.js` in your browser's console or a JavaScript interpreter.
3. Execute the code to observe the unexpected outputs.
4. Open `bugSolution.js` and execute the code to see the corrected behavior.