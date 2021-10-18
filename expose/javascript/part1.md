## Intro to JavaScript

### Part 1. A Quick Introduction...

1. values added:  `20`
2. final result:  `20`
3. values added:  `20`
4. Line 13 causes `Uncaught ReferenceError: result is not defined`. This is because a `let` variable can only be access in its own code block `{...}`, and line 13 is not in the code block of variable `result`.
5. Line 7 causes `Uncaught TypeError: Assignment to constant variable`. This is because `result` is declared as a `const`, so it can't be reassigned.
6. Line 7 causes `Uncaught TypeError: Assignment to constant variable`. This is because `result` is declared as a `const`, so it can't be reassigned.
