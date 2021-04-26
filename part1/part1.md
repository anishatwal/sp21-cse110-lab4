### Part 1a
1. values added: 20
2. final result: 20
3. values added: 20
4. error because `result` is declared with `let` so it is block scoped and, therefore, is undefined at line 13
5. error because `result` is declared with `const` so its value cannot be updated at line 7
6. error because `result` is declared with `const` so its value cannot be updated at line 7

### Part 1b
1. 3 is printed because the for loop on line 6 runs is broken out of when `i` is set to `prices.length` so at line 12 `i`'s value is `prices.length` which is 3, as seen on line 19 since prices is `[100,200,300]`
2. 150 is printed because the last time that the for loop is run through is when `i=2` so on line 7 `discountedPrice` would be `prices[2] * (1-0.5)` = `300 * 0.5` = `150`
3. 150 is printed because the last time that the for loop is run through is when `i=2` so on line 8 `finalPrice` is set to `Math.round(150 * 100) / 100` = `150`
4. `[50,100,150]` is returned because on line 16 `discounted` is returned and as seen on line 3 `discounted` is an array, and the for loop on line 6 goes through the prices of each item, calculates the discounted price, and pushes the final price to the discounted array so `discounted` is the array of the final discounted prices  
5. error because `i` is declared with `let` on line 6, which is block scoped, so its scope is within the for loop so at line 12 `i` is undefined
6. error because `discountedPrice` is declared with `let` on line 7, which is block scoped, so its scope is within the for loop so at line 13 `discountedPrice` is undefined 
7. 150 is printed because `finalPrice` is declared with `let` on line 4 so the block of its scope is the whole function, so the last time that the for loop is run through is when `i=2` so on line 8 `finalPrice` is set to `Math.round(150 * 100) / 100` = `150`, making `finalPrice` defined as 150 on line 14
8. `[50,100,150]` is returned because `discounted` is declared with `let` on line 3 so the block of its scope is the whole function, so on line 16 `discounted` is returned and as seen on line 3 `discounted` is an array, and the for loop on line 6 goes through the prices of each item, calculates the discounted price, and pushes the final price to the discounted array so `discounted` is the array of the final discounted prices
9. error because `i` is declared with `let` on line 6, which is block scoped, so its scope is within the for loop so at line 11 `i` is undefined 
10. 3 is printed because `length` is declared with `const` on line 4 so the block of its scope is the whole function, so it is set to `prices.length` so its value is 3, as seen on line 17 since prices is `[100,200,300]`, and this value is not updated 
11. `[50,100,150]` is returned because `discounted` is declared with `const` on line 3 so the block of its scope is the whole function and this variable is never updated or re-declared throughout the function because it is only pushed to, so on line 14 `discounted` is returned and as seen on line 3 `discounted` is an array, and the for loop on line 6 goes through the prices of each item, calculates the discounted price, and pushes the final price to the discounted array, which does not create errors with `let` on lines 6 and 7 because their scopes are an iteration of the for loop so they are not re-declared, so `discounted` is the array of the final discounted prices 
12. A. student.name
    B. student["Grad Year"]
    C. student.greeting()
    D. student["Favorite Teacher"].name
    E. student.courseLoad[0]
13. A. '32' because int 2 maps to its exact string representation '2' and the strings are concatenated
    B. 1 because cannot subtract strings so string '3' maps to int 3 and the integers are subtract
    C. 3 because null maps to int 0 and the integers are added
    D. '3null' because null maps to the string 'null' and the strings are concatenated
    E. 4 because true maps to int 1 and the integers are added
    F. 0 because false maps to int 0 and null maps to int 0 and the integers are added
    G. '3undefined' because undefined maps to the string 'undefined' and the strings are concatenated
    H. NaN because cannot subtract strings so string '3' maps to int 3 and undefined maps to NaN and arithmetic involving NaN always produced NaN
14. A. true because string '2' maps to int 2 and 2 is greater than 1
    B. false because since both '2' and '12' are strings, alphabetically 1 is less than 2
    C. true because string '2' maps to int 2 and the value of 2 is equal to the value of 2
    D. false because there is not type coercion with === so the types of 2 and '2' are not equal since 2 is an int and '2' is a string
    E. false because true maps to int 1 and the values of 1 and 2 are not equal
    F. true because Boolean(2) is the boolean true so the types and values of true and Boolean(2) are equal
15. === checks for strict equality, meaning that the type and the value of datas are the same, while == checks for loose equality, meaning that it also performs type coercion
16. [answer file](part1b-question16.js)
17. [2,4,6] because in `modifyArray` on line 2 `newArr` is declared with `const` as an empty array, the for loop on line 3 runs until `i` is `array.length` which is 3 (since the first parameter of `modifyArray` is `[1,2,3]`), within the for loop the result of calling the function `doSomething` with each item in `array` is pushed to `newArray` which is then returned as the result of `modifyArray`, also the function `doSomething` just takes the input of the array item and doubles its value
18. [answer file](part1b-question18.js)
19. 1 4 3 2 because the console logs for 1 and 4 do not have any delays so they are printed as the code is execute, then the console log for 3 has a delay of 0 seconds so it is printed immediately after the code is executed, lastly the console log for 2 has a delay of 1 second so it is printed 1 second after the code is executed