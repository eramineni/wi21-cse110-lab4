Part 1 of Part 3
1. The bug was that the values were being concatenated as strings instead of integers. For example, if the first number was "1" and the second one was "2", the value "12" was returned as opposed to 3.
2. To fix this bug, simply use the Number() function to convert num1 and num2 to integers so that they will add numerically. 

Part 2 of Part 3
1. citylots.json
2. part2.js
3. 11.7 mb
4. 4.25 seconds
5. Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/87.0.4280.141 Safari/537.36
6. Apache
7. Tue, 26 Jan 2021 22:14:13 GMT
8. application/json
9. fetchData()
