1. Line 12 will print 2, which is the most recent value of i. This is because variables declared with the var keyword are not block scoped, so the variable i used in the for loop is also accessible outside it.

2. Line 12 will print 150, which is the most recent value of discountedPrice.  This is because variables declared with the var keyword are not block scoped, so the variable discountedPrice used in the for loop is also accessible outside it.

3. Line 14 will print 150, which is the most recent value oof finalPrice.

4. The function will return [50, 100, 150]. On the first iteration of the for loop, the value 100 is read from the input array prices and multiplied by 0.5 (since discount = 0.5 and 1 - 0.5 = 0.5) to get 50 for the first value of discountPrice. Then finalPrice multiplies discountPrice by 100 and divides by 100 to get the same value of 50, which is then loaded into the discounted array as the first element. By the same logic, 100 and 150 are loaded as the next 2 elements, therefore, the function returns the array [50,100,150].

5. The code causes an error because the variable i is declared used the let keyword, which is block scoped, which means that i is not recognized as a valid variable outside the for loop.

6. The code causes an error because the variable discountedPrice is declared used the let keyword, which is block scoped, which means that discountedPrice is not recognized as a valid variable outside the for loop.

7. Line 14 will print 150, which is the most recent value oof finalPrice. This is because finalPrice is declared outside the for loop, so it is also accessible outside the for loop.

8. The function will return [50, 100, 150]. The behavior of the code inside the for loop is unaffected by the variables being declared using let, as they are still wihtin scope, so finalPrice is calculated the same as it is in quesion 4 for each iteration, resulting in the same array.

9. The code causes an error because the variable i is declared used the let keyword, which is block scoped, which means that i is not recognized as a valid variable outside the for loop.

10. Line 12 will print 3. Since the variable length is declared outside the for loop, its scope is outside the for loop as well. Since there are 3 elements in the prices array, length is assigned the value 3 on line 4, which means that when the value of length is printed by the console.log command, 3 gets printed.

11. The function will return [50, 100, 150]. Since all of the numbers in the prices array result in nice integer values, the line that was there in previous code to calculate the finalPrice was not really needed, as it just resulted in the previously calculated discountedPrice values. For this reason, removing that line in this instance does not change the results of the function, and the values passed in are still halved.

12. 
    A. student.name
    B. student["Grad Year"]
    C. student.greeting()
    D. student["Favorite Teacher"].name
    E. student.courseLoad[0]

13. 
    A. '32' was the result. This is because the '+' operator is also used for string concatenation, and because '3' is a string type, the string mapping of the second operand was used, and '2' was concatenated to the end of '3' to form the string '32'.
    B. 1 was the result. This is because the '-' operator is only used for numbers, so JavaScript converts all the operands to numbers. So '3' gets converted to 3 and 3 - 2 = 1.
    C. The result is 3. Null maps to an numeric value of 0, so when null is added to 3, the resulting operation is 3 + 0, which equals 3.
    D. '3null' was the result. This is because the '+' operator is also used for string concatenation, and because '3' is a string type, the string mapping of the second operand was used, and 'null' was concatenated to the end of '3' to form the string '3null'.
    E. 4 was the result. This is because true maps to a numeric value of 1, so when 3 is added to true, the resulting operation is 1 + 3, which equals 4.
    F. 0 was the result. This because both false and null map to a numeric value of 0. So when the '+' operator is used, the numeric mapping of each is used, and the resulting operation is 0 + 0 = 0.
    G. '3undefined' was the result. This is because the '+' operator is also used for string concatenation, and because '3' is a string type, the string mapping of the second operand was used, and 'undefined' was concatenated to the end of '3' to form the string '3undefined'.
    H. NaN was the result. This is because the '-' operator is used for calculating numeric differences, so the numeric values of both operands were taken. The numeric mapping of '3' is 3 and the numeric mapping of undefined is NaN, so the resulting operation is 3 - NaN, which results in NaN.

14. 
    A. The result is true. SInce the second operand 1, is a numeric type, the first operand '2' gets converted to a numeric type. Since 2 > 1 evaluates to true, the result is true.
    B. The result is false. Since both operands are strings, a numerical comparison is not done, but instead, a lexicographical string comparison. Since '12' starts with '1', it comes lexicographically first, so '2' will actually be greater, causing the expression to evaluate to false.
    C. The result is true. Since the '==' operator is used, JavaScript tries to convert both operands to the same type before comparing them. This means that the string '2' is converted to the numeric value 2, and since 2 = 2, the expression evaluates to true.
    D. The result is false. Since the '===' operator is used, both value and type are checked for the comparision and type conversion is not done, and since 2 is not the same as '2', the expression evaluates to false.
    E. The result is false. Since the '==' operator is used, JavaScript tries to convert both operands to the same type before comparing them. This means that true is converted to the numeric value 1, but since 1 is not equal to 2, the expression evaluates to false.
    F. The result is true. This is because the Boolean() function converts the numeric value 2 to a boolean value, and 2 converts to true in boolean. Since true is the same as true, the expression evaluates to true.

15. The '==' operator allows for type coersion, which means that it tries to convert variables to the same type before comparing them. The '===' operator on the other hand, checks if both value and type are the same and does not convert variable types.

17. The result will be [2,4,6]. Inside the function modifyArray, each element in the passed in array is iterated through and fed into the callback function doSomething, which returns the doubled value of the element. The computed value from the callback is then stored into the new array that modifyArray returns, which means that all the elements in the new array are equivalent to each element in the original array * 2, hence resulting in the array [2,4,6].

19. The code prints 1, then 4 on the next line, then 3 on the next line, then 2 on the next line.
