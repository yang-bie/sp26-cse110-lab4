1. At line 12, the code will print `3`.
   This happens because `i` is declared with `var` inside the `for` loop. In JS, `var` is a function-scoped, not block-scoped, so `i` can still be accessed outside the `for` loop.
   After the `for` loop finishes, `i` has been incremented from `0` to `3` and then the loop condition `i < prices.length` becomes false. Since `prices.length` is `3`, `console.log(i)` prints `3`.

2. At line 13, the code will print `150`.
   This happens because `discountedPrice` is declared with `var` inside the `for` loop. In JavaScript, `var` is function-scoped, not block-scoped, so `discountedPrice` can still be accessed outside the loop.
   After the loop finishes, `discountedPrice` keeps its last assigned value. In the last iteration, `prices[2]` is `300`, so `300 * (1 - 0.5)` equals `150`.

3. At line 14, the code will print `150`.
   This happens because `finalPrice` is declared with `var` at the top of the function, so it can be accessed anywhere inside the function.
   During the loop, `finalPrice` is updated each time. In the last iteration, `discountedPrice` is `150`, so `Math.round(discountedPrice * 100) / 100` is also `150`.
   Therefore, after the loop finishes, `finalPrice` keeps its last assigned value, which is `150`.

4. This function will return `[50, 100, 150]`.
   This happens because the function loops through the `prices` array and applies the discount to each price. Since `discount` is `0.5`, each price is multiplied by `1 - 0.5`,
   which is `0.5`. So the calculations are: `100 * 0.5 = 50`, `200 * 0.5 = 100`, `300 * 0.5 = 150`. Each calculated value is pushed into the `discounted` array. Therefore, the function returns `[50, 100, 150]`.

5. This function will cause an error at line 12.
   This happens because `i` is declared with `let` inside the `for` loop. In JavaScript, `let` is block-scoped, so `i` can only be accessed inside the `for` loop block. Line 12 tries to access `i` outside of the `for` loop, so the code causes a `ReferenceError`.

6. This function will cause an error at line 13.
    This happens because `discountedPrice` is declared with `let` inside the `for` loop. In JavaScript, `let` is block-scoped, so `discountedPrice` can only be accessed inside the `for` loop block. Line 13 tries to access `discountedPrice` outside of the `for` loop, so the code causes a `ReferenceError`.

7. At line 14, the code will print `150`.
   This happens because `finalPrice` is declared with `let` at the top of the function, not inside the `for` loop. Therefore, `finalPrice` can be accessed anywhere inside the function after it is declared. During the loop, `finalPrice` is updated each time. In the last iteration, `discountedPrice` is `150`, so `finalPrice` also becomes `150`.

8. This function will return `[50, 100, 150]`. 
   This happens because the function loops through the `prices` array and applies the discount to each price. Since `discount` is `0.5`, each price is multiplied by `1 - 0.5`, which is `0.5`. So the calculations are: `100 * 0.5 = 50`, `200 * 0.5 = 100`, `300 * 0.5 = 150`. Each result is stored in `finalPrice` and then pushed into the `discounted` array. Therefore, the function returns `[50, 100, 150]`.
   
9. This function will cause an error at line 11.
   This happens because `i` is declared with `let` inside the `for` loop. In JavaScript, `let` is block-scoped, so `i` can only be accessed inside the `for` loop block.
   Line 11 tries to access `i` outside of the `for` loop, so the code causes a `ReferenceError`.

10. At line 12, the code will print `3`.
    This happens because `length` is declared with `const` near the top of the function, and it is inside the function block, not inside the `for` loop. Therefore, it can still be accessed at line 12. `length` is assigned the value of `prices.length`. Since the array is `[100, 200, 300]`, `prices.length` is `3`.

11. This function will return `[50, 100, 150]`.
    This happens because `discounted` is declared with `const`, but the array itself can still be changed. `const` only prevents reassigning the variable to a different value; it does not prevent modifying the contents of the array. The function loops through the `prices` array and calculates each discounted price: `100 * (1 - 0.5) = 50`, `200 * (1 - 0.5) = 100`, `300 * (1 - 0.5) = 150`. Each result is pushed into the `discounted` array, so the function returns `[50, 100, 150]`.

12. 
    A. `student.name`

    B. `student['Grad Year']`

    C. `student.greeting()`

    D. `student['Favorite Teacher'].name`

    E. `student.courseLoad[0]`

13. Arithmetic

    A. `'3' + 2` outputs `"32"`  
    Because `+` with a string performs string concatenation, so `2` becomes `"2"`.

    B. `'3' - 2` outputs `1`  
    Because `-` only works as numeric subtraction, so `'3'` is converted to the number `3`.

    C. `3 + null` outputs `3`  
    Because `null` is converted to `0` in numeric addition.

    D. `'3' + null` outputs `"3null"`  
    Because `+` with a string performs string concatenation, so `null` becomes `"null"`.

    E. `true + 3` outputs `4`  
    Because `true` is converted to `1`.

    F. `false + null` outputs `0`  
    Because `false` is converted to `0`, and `null` is also converted to `0`.

    G. `'3' + undefined` outputs `"3undefined"`  
    Because `+` with a string performs string concatenation, so `undefined` becomes `"undefined"`.

    H. `'3' - undefined` outputs `NaN`  
    Because `undefined` becomes `NaN` when converted to a number, so the result is `NaN`.


14. Comparison

    A. `'2' > 1` outputs `true`  
    Because `'2'` is converted to the number `2`, and `2 > 1` is true.

    B. `'2' < '12'` outputs `false`  
    Because both values are strings, so JavaScript compares them alphabetically. Since `'2'` comes after `'1'`, the result is false.

    C. `2 == '2'` outputs `true`  
    Because `==` allows type conversion, so `'2'` is converted to the number `2`.

    D. `2 === '2'` outputs `false`  
    Because `===` checks both value and type. One is a number, and the other is a string.

    E. `true == 2` outputs `false`  
    Because `true` is converted to `1`, and `1 == 2` is false.

    F. `true === Boolean(2)` outputs `true`  
    Because `Boolean(2)` returns `true`, so this becomes `true === true`.


15. Difference between `==` and `===`
    `==` checks if two values are equal after allowing type conversion.
    `===` checks if two values are equal without type conversion. The values must have the same value and the same type.
    In general, `===` is safer and better to use because it avoids unexpected type conversion.

17. The result will be `[2, 4, 6]`.

    This happens because `modifyArray` takes two parameters: an array and a callback function. In this case, the array is `[1, 2, 3]`, and the callback function is `doSomething`.

    Inside the `for` loop, each element of the array is passed into `doSomething`.

    `doSomething(1)` returns `1 * 2`, which is `2`.

    `doSomething(2)` returns `2 * 2`, which is `4`.

    `doSomething(3)` returns `3 * 2`, which is `6`.

    Each returned value is pushed into `newArr`. Therefore, `modifyArray([1, 2, 3], doSomething)` returns `[2, 4, 6]`.

19. The output will be:

    1
    4
    3
    2

    This happens because `console.log(1)` runs first.

    Then the two `setTimeout` functions are scheduled, but they do not run immediately.

    After that, `console.log(4)` runs.

    Even though `console.log(3)` has a delay of `0`, it still waits until the current function finishes running. So `3` prints after `4`.

    Finally, `console.log(2)` prints after about 1000 milliseconds.