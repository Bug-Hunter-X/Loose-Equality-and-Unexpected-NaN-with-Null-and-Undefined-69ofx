# JavaScript Loose Equality Bug

This repository demonstrates a common JavaScript error involving loose equality (`==`) when dealing with `null` and `undefined` values.

The `bug.js` file contains a function that intends to handle `null` values gracefully.  However, due to the use of loose equality, it fails to correctly handle `undefined`, leading to `NaN` in the output.

The `bugSolution.js` file presents a solution using strict equality (`===`) to address this issue and achieve the desired behavior.

## How to Reproduce

1. Clone this repository.
2. Open `bug.js` and observe the unexpected `NaN` output for `undefined`.
3. Open `bugSolution.js` to see how using strict equality fixes the problem.

## Key Learning Points

* Loose equality (`==`) in JavaScript performs type coercion, which can sometimes lead to unexpected results, particularly with `null` and `undefined`.
* Strict equality (`===`) directly compares values without type coercion, improving reliability.
* Always use strict equality (`===`) when comparing values in JavaScript to avoid subtle bugs.