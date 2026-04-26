1. values added:  20
   
2. final result:  20
   
3. We should not use var because it is function-scoped and can cause unexpected behavior. In this example, result is declared inside the if block, but line 13 can still access it
   because var ignores block scope. Using let and const is better since they are block-scoped, safer, and less likely to cause bugs.

4. values added:  20
   
5. This code will cause an error.
   Because `result` is declared with `let`, it is block-scoped and only exists inside the if block. Line 13 is outside of that block, so JS cannot access result there, which causes a `ReferenceError`.

6. This code will cause an error at line 7. 
    Because `result` is declared with `const`, so its value cannot be reassigned. After `const result = 0;` JS does not allow changging result to another value. This causes: `TypeError: Assignment to constant variable.` So line 9 does not print anything, because the program already stops at line 7
    
7. This code will cause an error at line 7.
   Nothing is printed by line 13 because the program already throws an error at line 7. Since execution stops there, line 9 and line 13 are never reached.