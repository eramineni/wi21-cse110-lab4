1. The bug was that the values were being concatenated as strings instead of integers. For example, if the first number was "1" and the second one was "2", the value "12" was returned as opposed to 3.
2. To fix this bug, simply use the Number() function to convert num1 and num2 to integers so that they will add numerically. 
