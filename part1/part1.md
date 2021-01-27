1. At line 11, the current value of i will be printed. This current value is whatever i was set equal to following the complete execution of the for loop. The reason the value of i still persists beyond the for loop is because i is of type var. This type has no sense of block scope, and is either function-scoped or global-scoped. 

2. At line 12, the value of discountedPrice will be printed. This is because discounted price is of type var, and var's have no sense of block scope, and is rather function-scoped or global-scoped. The value of discountedPrice will be recalculated as the for loop goes through each index of prices and will essentially be dependent on whatever the last value of the last index of prices is. 

3. At line 13, the value of finalPrice will be printed. This is because finalPrice is of type var, and var's have no sense of block scope, and is rather function-scoped or global-scoped. The value of finalPrice will be recalculated as the for loop goes through each index of prices and will essentially be dependent on whatever the last value of the last index of prices is.

4. The function will return [50, 100, 150]. The reason for this is because the function will return an array/list called discounted. This variable initially starts out empty. As the for loop traverses through prices, a discountedPrice is calculated. In the first iteration, this is 100(0.5) = 50. Next, finalPrice is set to Math.round(discountedPrice * 100) / 100. Math.round rounds to the nearest integer, so this calculation will give us 5000/100 = 50. Next, 50 is added to the end of the list called discounted. There are 2 more iterations of the for loop to go through. In the second iteration, discountedPrice is set to 200(0.5) = 100. Next, finalPrice is set to Math.round(100 * 100) / 100 = 100. Then, this value of finalPrice is pushed into the end of the list named discounted. In the final iteration of the for loop, discountedPrice is recalculated again to give us 300(0.5) = 150. Next, the finalPrice is calculated, and this is Math.round(discountedPrice * 150) / 100 = 150. This value is pushed to the end of discounted. Finally, discounted is returned, and it is equal to [50, 100, 150].

5. An error will be thrown because i is a let, and it is declared inside a code block which is the for loop. Thus, it is not defined outside the code block in places like line 11 where it is trying to print it out.

6. An error will be thrown because discountedPrice is a let, and it is declared inside a code block which is the for loop. Thus, it is not defined outside the code block in places like line 12 where it is trying to print it out.

7. This would print whatever the value of finalPrice is set to following the termination of the for loop. This is because this console.log statement is in the same block as the declaration of discounted which is at the beginning of the function, and outside the for loop. 

8. The function would still return the same value as it did for number 4. This is because discounted is a let, and it is declared in the same code block level as the return. This value that would be returned is [50, 100, 150]. As the for loop traverses through prices, a discountedPrice is calculated. In the first iteration, this is 100(0.5) = 50. Next, finalPrice is set to Math.round(discountedPrice * 100) / 100. Math.round rounds to the nearest integer, so this calculation will give us 5000/100 = 50. Next, 50 is added to the end of the list called discounted. There are 2 more iterations of the for loop to go through. In the second iteration, discountedPrice is set to 200(0.5) = 100. Next, finalPrice is set to Math.round(100 * 100) / 100 = 100. Then, this value of finalPrice is pushed into the end of the list named discounted. In the final iteration of the for loop, discountedPrice is recalculated again to give us 300(0.5) = 150. Next, the finalPrice is calculated, and this is Math.round(discountedPrice * 150) / 100 = 150. This value is pushed to the end of discounted. Finally, discounted is returned, and it is equal to [50, 100, 150].

9. At line 11, an error will be thrown because i is a let, and it is declared inside a code block which is the for loop. Thus, it is not defined outside the code block in places like line 11 where it is trying to print it out.

10. At line 12, nothing will be printed, and an error will have been thrown prior in the for loop. This is because discountedPrice is a variable of type const that is being reassigned values after each iteration of the for loop. However, this is not allowed because the value of a const is not allowed to be changed. 

11. At line 13, nothing will be printed, and an error will have been thrown prior in the for loop. This is because finalPrice is a variable of type const that is being reassigned values after each iteration of the for loop. However, this is not allowed because the value of a const is not allowed to be changed. 

12. Nothing will be returned because an error will have been thrown an uncaught typeerror prior which is the assignment to a constant variable. This is not allowed as the values of consts are not allowed to be changed. 

13.  
    1. student.name 
    2. student["Grad Year"] 
    3. student.greeting()
    4. student["Favorite Teacher"].name
    5. student.courseLoad[0]

14. 
    1. '32'; String conversion will occur.The + sign will indicate to concatenate when used with a string. Therefore, 2 will be concatenated to the string '3' and output 32.
    2. 1; Numeric conversion will occur. The - indicates subtraction. Therefore 2 will be subtracted from the integer conversion of '3' and tield 1.
    3. 3; Numeric conversion will occur. Adding an integer and null causes the null value to be converted to 0, and the output will be the int 3.
    4. '3null'; String conversion will occur. The + sign will indicate to concatenate when used with a string. Therefore, null will be converted to the string word "null" and be added to 3.
    5. 4; The true will be converted to a 1 because we are adding to the int 3, and thus 3+1 = 4.
    6. 0; Numeric conversion will occur, and the false will be converted to a 0, and the null will be converted to a 0. 0+0 = 0.
    7. "3undefined"; String conversion will occur, and thus, the word undefined will be concatenated.
    8. NaN; Numeric conversion will attempt to occur; however, this conversion will fail because string is not a valid number, and neither is undefined. 
    
15. 
    1. True; When comparing values of different types, JavaScript converts the values to numbers. 2 is greater than 1, so true is returned.
    2. False; The values are both strings, so string comparison or lexicographical order comparisons will occur. The first character of '12' comes before '2' lexicographically, so it is not greater.
    3. True; When comparing values of different types, JavaScript converts the values to numbers. 2 is equal to 2, so true is returned.
    4. False; === checks equality without performing type conversion. A string and an int are different types, so false is automatically returned.
    5. False; When comparing values of different types, JavaScript converts the values to numbers. True is converted to 1 which is not equal to 2.
    6. True; Boolean(2) becomes true because 2 is not an inherently empty value. True is the same type and equal to true, so true is returned.

16. == Performs type conversions and then checks equality. It is a non-strict check. Meanwhile, === is a strict equality check, and does not perform type conversions. 

17. 'How are you' is printed because the first statement is false and the next statement is true. In the first statement, true gets converted to an int, and it is equal to 1 which is not equal to 2. The second branch of the conditionals is true because 2 is converted to a boolean. It is converted to true because it represents or signifies a non-empty value.

18. In JS file titled part1-question18.js

19. 
