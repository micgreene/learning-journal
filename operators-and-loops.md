# Notes for Class 8 (6/9/20)

## Operators and Loops

### Comparison Operators: Evaluating Conditions
- Is equal to `==`: Compares 2 values to see if they are the same.
- Strict equal to `===`: Compares 2 values to check for both data type and value.
- is not equal to `!=`: Compares two values to se3 if they are NOT the same.
- Strict is not equal to `!==`: Compares 2 values to check that _both_ the data type and value are NOT the same.
- Greater than `>`: checks if number of left is greater than number on right.
- Less than `<`: checks if number on left is less than number on right.
- Greater than or equal to `>=`: checks if number on left is greater than or equal to number on right.
- Less than or equal to `<=`: checks if number on left is less than or equal to number on right.

### Structure
(some variable)(asignment operator)(comparison): `X = (score >= pass)`

### Logic Operators
- Logical and `&&`: this tests more than one condition. `((2 < 5) && (3 >= 2))` equals true because BOTH comparisons are true
- Logical or `||`: this operator tests at LEAST one condition `((2 < 5) || (2 < 1))` still equals true because at least one comparison is true
- Logical not `!`: takes a single boolen value and inverts it `!(2 < 1)` returns true since comparison is NOT logical

### Loops
1. For Loops
  - the most common loop, lets you run a specific script for a certain number of times.
  - structure: `for (var i = 0; i < 10; i++){document.write(i);}` establishes variable i as 0. then checks the variable against the comparison, as long as i < 10 it will run again. finally, increments i by 1 to take away one round of running the code until the comparison becomes false.

1. While loops
  - runs a script as long as a comparison remains true.
  - structure: `while (i < 10){i++;}` variable needs to be established beforehand, outside of loop. this will run until i becomes 
  
1. Do While loops
  - the main difference between a while loop and a do while loop is the do while provides its script before the while loop keyword, meaning the script will always run at least once.
  - Structure: `do{ i++;}while (i < 10);` this will increment i by 1 one time at least then will continue as long as the while comparison is true.
