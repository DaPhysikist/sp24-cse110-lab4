1. Line 9 prints "values added: 20".
2. Line 13 runs without an error as var is not block scoped, so the declaration of result is hoisted to the top of the function. It prints "final result: 20". 
3. Line 9 prints "values added: 20".
4. Line 13 returns an error, as result is declared using the let keyword, which is block scoped, so it only has local scope to the inside of the if statement, and is not recognized as a valid variable outside it.
5. Line 9 returns an error, as result is declared using the const keyword, which does not allow reassignment, but line 4 tried to reassign the value of result to num1 + num2.
6. Line 13 returns an error, as result is declared using the const keyword, which is block scoped, so it only has local scope to the inside of the if statement, and is not recognized as a valid variable outside it.