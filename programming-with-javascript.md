# Class 7 Notes (6/8/20)

## Programming with Javascript

### How Javascript makes web pages more interactive

1. **Access Content**
  - You can use JS to select any element, attribute, or text from an HTML page.
  
1. **Modify Content**
  - You can use JS to add/remove any element, attribute, or text from an HTML page
  
1. **Program Rules**
  - You can specify a set of steps for the browser to follow which allows it to access or change the contents of a page.
  
1. **React to Events**
  - You can specify a certain script to run in response to certain events.
  
  
  ### Solving Coding Problems
  Approach each situation uniquely:
  1. **Define the Goal**
    - What do I need this script/page to do?
  1. **Design the Script**
    - Design conceptualy how the code will operate and what pieces need to be created.
    - Use flowcharts tp path out logic visually.
  1. **Code Each Step**
    - Go through multiple iterations until optimal efficiency is discovered.
    
    
 ### Expressions
 An _expression_ evaluates into (results in) a single value. 
 
 There are two types:
    
 1. Single Assignment Expressions
   - Example: `var string = 'strang';`
 2. Expressions That Use Two or More Values
   - Example: `var area = 3 * 2;
      
 ### Operators
 - Assignment Operators
   + `this = 'that';`
 - Arithmetic Operators
   + `3 * 2;`  `3 / 2;`  `3 + 2;`  `3 - 2;`
   + `++` - increment  `--` = decrement
   + `%` - modulus (returns remainder)
      
 - String Operators
   + `greeting = 'hi ' + 'guy';`
 - Comparison Operators
 _compares two values to see if true or false then returns boolean_
   + `buy = 3 > 5;` - false
 - Logical Operators
 _Combines mutiple comparison opertors and returns boolean_
   + `buy = (5 > 3) && (2 < 4);` - true
      

### Functions

**A function is a set of instructions which may potentially receive input and then return a result.**
Functions save time by allowing us to call code that might need to be repeated or recycled quickly instead of hard coding all scripts.

When we **CALL** a function, we are requesting it to run:
`Math.random();`

A Function will often take a **PARAMETER** and give back a **RETURN VALUE**

`function addUs(int a, int b){
  result = a + b;  
  return result;
 }`
 
 `addUs(3,4);` - when run, result would return 7
 
 We can return **multiple values** using **ARRAYS**:
 
 ` function getSize(width, height, depth){
  var area = width * height;
  var volume = width * height * depth;
  var sizes = [area, volume];
  return sizes;
 }`
