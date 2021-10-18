## Intro to JavaScript

### Part 2. A Little More of a Challenge...

1. `3` is printed. Because `prices = [100, 200, 300]` and `prices.length = 3`, when loop exits, `i=3`. So, `console.log(i)` prints `3`.
2. `150` is printed. Because `prices = [100, 200, 300]`, when loop exits, `discountedPrice = prices[2] * (1 - discount) = 300 * (1 - 0.5) = 150`. So, `console.log(discountedPrice)` prints `150`.
3. `150` is printed. Because `prices = [100, 200, 300]`, when loop exits, `finalPrice = Math.round(discountedPrice * 100) / 100 = 150`. So, `console.log(finalPrice)` prints `150`.
4. This function returns `[50, 100, 150]`. It returns a list of all calculated `finalPrice` which are `100*0.5=50, 200*0.5=100, 300*0.5=150`.
5. Line 12 causes an error `Uncaught ReferenceError: i is not defined`. This is because `i` is declared by `let` and it's only visible inside for loop, so `i` can't be accessed in line 12 (line 12 and `let i = 0` are not in the same code block).
6. Line 13 causes an error `Uncaught ReferenceError: discountedPrice is not defined`. This is because `discountedPrice` is declared by `let` and it's only visible inside for loop, so `discountedPrice` can't be accessed in line 13 (line 13 and `let discountedPrice = ...` are not in the same code block).
7. `150` is printed. This is because `finalPrice` is declared by `let` and it's visible inside function `discountPrices`, so `finalPrice` can be accessed in line 14 (line 14 and `let finalPrice = 0` are in the same code block).
8. This function returns `[50, 100, 150]`. It returns a list of all calculated `finalPrice` which are `100*0.5=50, 200*0.5=100, 300*0.5=150`.
9. Line 11 causes an error `Uncaught ReferenceError: i is not defined`. This is because `i` is declared by `let` and it's only visible inside for loop, so `i` can't be accessed in line 11 (line 11 and `let i = 0` are not in the same code block).
10. `3` is printed. Because `prices = [100, 200, 300]` and `prices.length = 3`, and `length` is declared by `const length = prices.length` and it's visible inside function `discountPrices`, so `length` can be accessed in line 12 (line 12 and `const length = prices.length` are in the same code block).
11. This function returns `[50, 100, 150]`. It returns a list of all calculated `finalPrice` which are `100*0.5=50, 200*0.5=100, 300*0.5=150`.
12. Given the above Object, the notation for:
    -  A. Accessing the value of the name property in the student object: `student.name`
    -  B. Accessing the value of the Grad Year property in the student object: `student["Grad year"]`
    -  C. Calling the function for the greeting property in the student object: `student.greeting()`
    -  D. Accessing the name property of the object in the Favorite Teacher property in student: `student["Favorite Teacher"].name`
    -  E. Access the first index in the array of the courseLoad property of the student object: `student.courseLoad[0]`
13. Arithmetic
    -  A. `'3' + 2` outputs `'32'`, `+` here is interpreted as string concatenation, so `2` is converted to `'2'`, `'3' + '2' = '32'`
    -  B. `'3' - 2` outputs `1`, `-` here is interpreted as arithmetic operation, so `'3'` is converted to `3`, `3 - 2 = 1`
    -  C. `3 + null` outputs `3`, `+` here is interpreted as arithmetic operation, so `null` is converted to `0`, `3 + 0 = 3`
    -  D. `'3' + null` outputs `'3null'`, `+` here is interpreted as string concatenation, so `null` is converted to `'null'`, `'3' + 'null' = '3null'`
    -  E. `true + 3` outputs `4`, `+` here is interpreted as arithmetic operation, so `true` is converted to `1`, `1 + 3 = 4`
    -  F. `false + null` outputs `0`, `+` here is interpreted as arithmetic operation, so `false` is converted to `0` and `null` is converted to `0`, `0 + 0 = 0`
    -  G. `'3' + undefined` outputs `'3undefined'`, `+` here is interpreted as string concatenation, so `undefined` is converted to `'undefined'`, `'3' + 'undefined' = '3undefined'`
    -  H. `'3' - undefined` outputs `NaN`, `-` here is interpreted as arithmetic operation, `'3'` is converted to `3` and doing arithmetic operations with undefined will have an output of `NaN`, `3 - undefined = NaN`
14. Comparison
    -  A. `'2' > 1` outputs `true`, `>` here is interpreted as arithmetic comparison, `'2'` is converted to `2`, `2 > 1` is `true`
    -  B. `'2' < '12'` outputs `false`, `<` here is interpreted string comparison, `'2' < '1' = false` so `'2' < '12'` is `false`
    -  C. `2 == '2'` outputs `true`, `==` here is interpreted as arithmetic comparison, `'2'` is converted to `2`, `2 == 2` is `true`
    -  D. `2 === '2'` outputs `false`, `===` is strict equality check, it does not perform type conversion, so `2` has type `number` and `'2'` has type `string` and they are different, `2 === '2'` is `false`
    -  E. `true == 2` outputs `false`, `==` here is interpreted as arithmetic comparison, `true` is converted to `1`, `1 == 2` is `false`
    -  F. `true === Boolean(2)` outputs `true`, `Boolean(2)` is `true`, so `true === true` is `true`
15. Explain the difference between the == and === operators: A regular equality check `==` performs type conversion and then check the equality, A strict equality operator `===` checks the equality without type conversion.
16. Code is in a JS file part2-question16.js.
17. `modifyArray([1,2,3], doSomething)` returns `[2, 4, 6]`. Calling `modifyArray` with parameters `array = [1,2,3]` and `callback = doSomething`, it first creates a list `newArr`, and then for each element in `array = [1,2,3]`, it calls `callback(element)` and push that returned value into `newArr`. `callback` takes a `num` and returns `num * 2`, so `newArr = [2, 4, 6]` after the for loop. `modifyArray` returns `newArr = [2, 4, 6]` at the end.
18. Code is in a JS file part2-question18.js.
19. The output of the above code is:
```
1
4
3
2
```