## HTML Lists : 

### Unordered HTML List :
**An unordered list starts with the `<ul>` tag. Each list item starts with the `<li>` tag. The list items will be marked with bullets (small black circles) by default:**

**Example :**
```
<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>

```

### Ordered HTML List : 
**An ordered list starts with the `<ol>` tag. Each list item starts with the `<li>` tag. The list items will be marked with numbers by default:**

**Example :**
```
<ol>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>

```

### HTML Description Lists :
HTML also supports description lists. A description list is a list of terms, with a description of each term. The `<dl>` tag defines the description list, the `<dt>` tag defines the term (name), and the `<dd>` tag describes each term:

**Example :**
```
<dl>
  <dt>Coffee</dt>
  <dd>- black hot drink</dd>
  <dt>Milk</dt>
  <dd>- white cold drink</dd>
</dl>
```
![list image](https://744025.smushcdn.com/1245953/wp-content/uploads/2020/02/HTML-LISTS.jpg)

 ## CSS Box Model :
 
 In web development, the CSS box model refers to how HTML elements are modeled in browser engines and how dimension of those HTML elements are derived from CSS properties. It is a fundamental concept for the composition of HTML webpages.
 ![box image](https://www.washington.edu/accesscomputing/webd2/student/unit3/images/boxmodel.gif)

### The compounents of the CSS box model:
- The content area, bounded by the content edge, contains the "real" content of the element, such as text, an image, or a video player. Its dimensions are the content width (or content-box width) and the content height (or content-box height). It often has a background color or background image.

- The padding area, bounded by the padding edge, extends the content area to include the element's padding. Its dimensions are the padding-box width and the padding-box height.

- The border area, bounded by the border edge, extends the padding area to include the element's borders. Its dimensions are the border-box width and the border-box height.

- The margin area, bounded by the margin edge, extends the border area to include an empty area used to separate the element from its neighbors. Its dimensions are the margin-box width and the margin-box height.

## CSS Overflow

The overflow property specifies whether to clip the content or to add scrollbars when the content of an element is too big to fit in the specified area, and works only for block elements with specified height

### CSS Border Styles:
This featuer let us to choose how we can display the borders like :

1. dotted - Defines a dotted border
2. dashed - Defines a dashed border
3. solid - Defines a solid border
4. double - Defines a double border
5. groove - Defines a 3D grooved border. The effect depends on the border-color value
6. ridge - Defines a 3D ridged border. The effect depends on the border-color value
7. inset - Defines a 3D inset border. The effect depends on the border-color value
8. outset - Defines a 3D outset border. The effect depends on the border-color value
9. none - Defines no border
10. hidden - Defines a hidden border

![image](https://s3.amazonaws.com/webucator-how-tos/2304.png)

### CSS Margins :
The CSS margin properties are used to create space around elements, outside of any defined borders. With CSS, you have full control over the margins. There are properties for setting the margin for each side of an element (top, right, bottom, and left).

### CSS Padding :
The CSS `padding` properties are used to generate space around an element's content, inside of any defined borders.With CSS, you have full control over the padding. There are properties for setting the padding for each side of an element (top, right, bottom, and left).

### Center Align Text :
**To just center the text inside an element, use `text-align: center;`**

**Example:**
```
.center {
  text-align: center;
  border: 3px solid green;
}
```
### CSS border-image Property :

**Definition and Usage:**
The `border-image` property allows you to specify an image to be used as the border around an element.

The border-image property is a shorthand property for:

1. border-image-source
2. border-image-slice
3. border-image-width
4. border-image-outset
5. border-image-repeat

**Omitted values are set to their default values.**

### CSS box-shadow Property :

**Definition and Usage : The `box-shadow` property attaches one or more shadows to an element.**

### JavaScript Switch Statement :

**Use the switch statement to select one of many code blocks to be executed.**

**Syntax :**
```
switch(expression) {
  case x:
    // code block
    break;
  case y:
    // code block
    break;
  default:
    // code block
}

```

**This is how it works:**
- The switch expression is evaluated once.
- The value of the expression is compared with the values of each case.
- If there is a match, the associated block of code is executed.
- If there is no match, the default code block is executed.

### The break Keyword :
**When JavaScript reaches a `break` keyword, it breaks out of the switch block. This will stop the execution of inside the block.**
**It is not necessary to break the last case in a switch block. The block breaks (ends) there anyway.**

### The default Keyword :
**The `default` keyword specifies the code to run if there is no case match:**


### JavaScript Loops :

**Loops are handy, if you want to run the same code over and over again, each time with a different value.**

#### Different Kinds of Loops
**JavaScript supports different kinds of loops:**

1. `for` - loops through a block of code a number of times
2. `for/in` - loops through the properties of an object
3. `for/of` - loops through the values of an iterable object
4. `while` - loops through a block of code while a specified condition is true
5. `do/while` - also loops through a block of code while a specified condition is true

### The For Loop
**The for loop has the following syntax:**
```
for (statement 1; statement 2; statement 3) {
  // code block to be executed
}
```
-  Statement 1 is executed (one time) before the execution of the code block.

- Statement 2 defines the condition for executing the code block.

- Statement 3 is executed (every time) after the code block has been executed.

### The While Loop:

**The while loop loops through a block of code as long as a specified condition is true.**

**Syntax**

```
while (condition) {
  // code block to be executed
}
```
![loop image](https://www.incredible-web.com/media/7242/loops.png)