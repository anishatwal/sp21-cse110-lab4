### Part 1a
1. values added: 20
2. final result: 20
3. values added: 20
4. error because result is declared with let so it is block scoped and, therefore, is undefined at line 13
5. error because result is declared with const so its value cannot be updated at line 7
6. error because result is declared with const so its value cannot be updated at line 7

### Part 1b
1. 3 is printed because the for loop on line 6 runs is broken out of when i is set to prices.length so at line 12 i's value is prices.length which is 3, as seen on line 19 since prices is `[100,200,300]`
2. 150 is printed because the last time that the for loop is run through is when i=2 so on line 7 discountedPrince would be `prices[2] * (1-0.5)` = `300 * 0.5` = `150`
3. 