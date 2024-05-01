1. The bug was that the type of result is a string instead of a numeric type, which means that the '+' operator is treated as string concatenation and concatenates the string forms of the inputs num1 and num2 to each other, then stores the new string in result.

2. I would fix the bug by casting the inputs to numeric types first before adding them.