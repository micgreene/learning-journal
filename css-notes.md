# Notes for Class 5 (6/6/2020)
- [Home](https://micgreene.github.io/learning-journal/)

### CSS
**Cascading Style Sheets**'
A file created and attached to an HTML file in order to add style and aesthetic to the structure of a website.

### Color
- **RGB**
  - Uses hex code definitions for levels of Red, Green, Blue to creae hues.
- **HSL** (Hue, Saturation, Light)
  - Hue: simply, the specific color of the item
  - Saturation: how 'neon' or 'washed out' a color looks
  - Light:
  
 **Hex Codes**
   - Hexadecimal input for specific colors
   - Example: `#000000 - #000`
 
 ### Layout Examples
 p{
  color:black;
 }

**Elements of CSS**
- Selector: elemeent, universal, class, idcan have parent & sibling
- Property: "color" is the property
- Value: "black" is the value of the property in this case.
- Declaration: The property value pair.

### Linking to VSCode
1. **First, ensure that an _"index.html"_ -AND- a _"style.css"_ file have both been created in VSCode and committed to your repository**

1. **Next, link your .css file to your .html. In your .html fie, under "Title", include the line:**

  - `<link rel="stylesheet" href="style.css">`

`body
{
    background-color: rgba(214, 233, 176, .5);
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    color: rgb(31, 44, 4);
}

/*Header Section*/
header
{
    margin: 0px auto;
    width : 960px;
    background-color: rgb(214, 233, 176);
    height: 190px;
}

header > img
{
    width: 150px;
    margin-left: 10px;
    margin-top: 10px;

    float: left;

}

h1
{
    text-align: center;
    padding: 30px;
    margin-right: 150px;
}

header > nav
{
    float: left;
}

header > nav >ul >li
{
    /*display: inline-block;*/
    width: 100px;
    border: 1px solid black;
    text-align: left;
    border-radius: 25px;
    margin: 5px;
    padding: 5px;
    margin-right: 30px;
    background-color: darkgreen;

}`
