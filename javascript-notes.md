
# Class 6 Notes (Class 2 - 6/6/2020)

### JavaScript
**Front end browser language used to create dynamic elements and applications**

Uses conditionals:
- if
- if else

Uses operators to set up logarithms:
- (+ - =)

Uses a variety of data types:
- string
- boolen
- number

Uses variables to store information:
- number x = 6;
- now x == 6;
### Javascript Examples:

`var today = new Date();`
`var hourNow = today.getHours();`
`var greeting;`

`if(hourNow > 18){`
    `greeting = 'Good evening!';`
`}   else if (hourNow > 12){`
    `greeting = 'Good afternoon';`
`}   else if (hourNow > 0){`
    `greeting = 'Good morning!';`
`}   else {`
    `greeting = 'Welcome!';`
`}`

`document.write('<h3>' + greeting + '</h3>');`
