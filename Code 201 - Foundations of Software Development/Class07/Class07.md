## HTML Tables :

**HTML tables allow web authors to arrange data into rows and columns.**

### Defining an HTML Table : 
**An HTML table is defined with the `<table>` tag.**

**Each table row is defined with the `<tr>` tag. A table header is defined with the `<th>` tag. By default, table headings are bold and centered. A table data/cell is defined with the `<td>` tag.**

**Example :**
```
<table style="width:100%">
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
    <th>Age</th>
  </tr>
  <tr>
    <td>Jill</td>
    <td>Smith</td>
    <td>50</td>
  </tr>
  <tr>
    <td>Eve</td>
    <td>Jackson</td>
    <td>94</td>
  </tr>
</table>
```
### HTML Table - Adding a Border :
**If you do not specify a border for the table, it will be displayed without borders.**

**A border is set using the CSS border property:**

**Example:**
```
table, th, td {
  border: 1px solid black;
}
```
### HTML Table - Collapsed Borders :
**If you want the borders to collapse into one border, add the CSS border-collapse property:**

**Example:**
```
table, th, td {
  border: 1px solid black;
  border-collapse: collapse;
}
```
# Functions, Methods, and Objects”

## Creating a JavaScript Object

Using the JavaScript Keyword new:

```javascript
var person = new Object();
person.firstName = "John";
person.lastName = "Doe";
person.age = 50;
person.eyeColor = "blue";
```

### Updating an object

```javascript
var person = { firstName: "John", lastName: "Doe", age: 50, eyeColor: "blue" };

var x = person;
x.age = 10; // This will change both x.age and person.age
delete person lastname // this will delete the person lastname proberty
```

### Creatin many objects with constructor

```javascript
function Vehicle(name, maker) {
   this.name = name;
   this.maker = maker;
}
let car1 = new Vehicle(’Fiesta’, 'Ford’);
let car2 = new Vehicle(’Santa Fe’, 'Hyundai’)
console.log(car1.name);    //Output: Fiesta
console.log(car2.name);    //Output: Santa Fe
```

### What is this?

The JavaScript this keyword refers to the object it belongs to.

It has different values depending on where it is used:

- In a method, this refers to the owner object.
- Alone, this refers to the global object.
- In a function, this refers to the global object.
- In a function, in strict mode, this is undefined.
- In an event, this refers to the element that received the event.
- Methods like call(), and apply() can refer this to any object.

### Arrays are objects

Objects are an unordered map from string keys to values, arrays are an ordered list of values (with integer keys). That's the main difference. They're both non-primitive, as they're composed of multiple values, which also implies pass-by-reference in JavaScript.

Arrays are also a kind of object, though, so you can attach extra properties to them, access their prototype and so on.

In your revised example, you're only taking advantage of the fact that an array is actually an object, i.e. you can set any property on them. You shouldn't do that. If you don't need an ordered list of values, use a plain object.

### Browser object model

The Browser Object Model (BOM) is used to interact with the browser.

The default object of browser is window means you can call all the functions of window by specifying window or directly.

![image](https://static.javatpoint.com/images/javascript/bom.jpg)

| Method       | Description                                                                             |
| ------------ | --------------------------------------------------------------------------------------- |
| alert()      | displays the alert box containing message with ok button.                               |
| confirm()    | displays the confirm dialog box containing message with ok and cancel button.           |
| prompt()     | displays a dialog box to get input from the user.                                       |
| open()       | opens the new window.                                                                   |
| close()      | closes the current window.                                                              |
| setTimeout() | performs action after specified time like calling function, evaluating expressions etc. |

Example:

```javascript
//Example of alert() in javascript
function msg() {
  alert("Hello Alert Box");
}

//Example of confirm() in javascript
function msg() {
  var v = confirm("Are u sure?");
  if (v == true) {
    alert("ok");
  } else {
    alert("cancel");
  }
}
```
## Global object

In JavaScript, there's always a global object defined. In a web browser, when scripts create global variables, they're created as members of the global object.

###  Strings Object

The String object lets you work with a series of characters; it wraps Javascript's string primitive data type with a number of helper methods.

As JavaScript automatically converts between string primitives and String objects, you can call any of the helper methods of the String object on a string primitive.

`var val = new String(string);`

#### String Properties

Property | Description
--------- | ---------
constructor |	Returns the string's constructor function
length	| Returns the length of a string
prototype	| Allows you to add properties and methods to an object

#### String Methods

Method | Description
------- | -------
charAt()	| Returns the character at the specified index (position)
charCodeAt()	| Returns the Unicode of the character at the specified index
concat()	| Joins two or more strings, and returns a new joined strings
endsWith()	| Checks whether a string ends with specified string/characters
fromCharCode()	| Converts Unicode values to characters
includes()	| Checks whether a string contains the specified string/characters
indexOf()	| Returns the position of the first found occurrence of a specified value in a string
lastIndexOf()	| Returns the position of the last found occurrence of a specified value in a string
localeCompare()	| Compares two strings in the current locale
match()	| Searches a string for a match against a regular expression, and returns the matches
repeat()	| Returns a new string with a specified number of copies of an existing string
replace()	| Searches a string for a specified value, or a regular expression
search()	| Searches a string for a specified value, or regular expression, and returns the position of the match
slice()	| Extracts a part of a string and returns a new string
split()	| Splits a string into an array of substrings
startsWith()	| Checks whether a string begins with specified characters
substr()	| Extracts the characters from a string, beginning at a specified start position
substring()	| Extracts the characters from a string, between two specified indices
toLocaleLowerCase()	| Converts a string to lowercase letters, according to the host's locale
toLocaleUpperCase()	| Converts a string to uppercase letters, according to the host's locale
toLowerCase()	| Converts a string to lowercase letters
toString()	| Returns the value of a String object
toUpperCase()	| Converts a string to uppercase letters
trim()	| Removes whitespace from both ends of a string
valueOf()	| Returns the primitive value of a String object

## Number object

JavaScript has only one type of number.

Numbers can be written with, or without, decimals:

```javascript
var x = 3.14;     // A number with decimals
var y = 34;       // A number without decimals
var x = 123e5;    // 12300000
var y = 123e-5;   // 0.00123
```


#### Number Properties

Property | Description
-------- | -----------
constructor	|  Returns the function that created JavaScript\'s Number prototype
MAX\_VALUE	|  Returns the largest number possible in JavaScript
MIN\_VALUE	|  Returns the smallest number possible in JavaScript
NEGATIVE\_INFINITY	|  Represents negative infinity (returned on overflow)
NaN	Represents |  a "Not\-a\-Number" value
POSITIVE\_INFINITY	|  Represents infinity (returned on overflow)
prototype	|  Allows you to add properties and methods to an object



#### Number Methods

Method       | Description
------------ | -------------
isFinite() | Checks whether a value is a finite number
isInteger() | Checks whether a value is an integer
isNaN()	| Checks whether a value is Number.NaN
isSafeInteger()	| Checks whether a value is a safe integer
toExponential(x) | Converts a number into an exponential notation
toFixed(x) | Formats a number with x numbers of digits after the decimal point
toLocaleString() | Converts a number into a string, based on the locale settings
toPrecision(x) | Formats a number to x length
toString() | Converts a number to a string
valueOf() | Returns the primitive value of a number



## Math Object

The Math object allows you to perform mathematical tasks.

Math is not a constructor. All properties/methods of Math can be called by using Math as an object, without creating it:

```javascript
var x = Math.PI;            // Returns PI
var y = Math.sqrt(16);      // Returns the square root of 16
```

#### Math Object Properties

Property	| Description
------------- | -------------
E	| Returns Euler's number (approx. 2.718)
LN2	| Returns the natural logarithm of 2 (approx. 0.693)
LN10	| Returns the natural logarithm of 10 (approx. 2.302)
LOG2E	| Returns the base-2 logarithm of E (approx. 1.442)
LOG10E	| Returns the base-10 logarithm of E (approx. 0.434)
PI	| Returns PI (approx. 3.14)
SQRT1_2	| Returns the square root of 1/2 (approx. 0.707)
SQRT2	| Returns the square root of 2 (approx. 1.414)


#### Math Object Methods

Method	| Description
-------- | --------
abs(x)	| Returns the absolute value of x
acos(x)	| Returns the arccosine of x, in radians
acosh(x)	| Returns the hyperbolic arccosine of x
asin(x)	| Returns the arcsine of x, in radians
asinh(x)	| Returns the hyperbolic arcsine of x
atan(x)	| Returns the arctangent of x as a numeric value between -PI/2 and PI/2 radians
atan2(y, x)	| Returns the arctangent of the quotient of its arguments
atanh(x)	| Returns the hyperbolic arctangent of x
cbrt(x)	| Returns the cubic root of x
ceil(x)	| Returns x, rounded upwards to the nearest integer
cos(x)	| Returns the cosine of x (x is in radians)
cosh(x)	| Returns the hyperbolic cosine of x
exp(x)	| Returns the value of Ex
floor(x)	| Returns x, rounded downwards to the nearest integer
log(x)	| Returns the natural logarithm (base E) of x
max(x, y, z, ..., n)	| Returns the number with the highest value
min(x, y, z, ..., n)	| Returns the number with the lowest value
pow(x, y)	| Returns the value of x to the power of y
random()	| Returns a random number between 0 and 1
round(x)	| Rounds x to the nearest integer
sin(x)	| Returns the sine of x (x is in radians)
sinh(x)	| Returns the hyperbolic sine of x
sqrt(x)	| Returns the square root of x
tan(x)	| Returns the tangent of an angle
tanh(x)	| Returns the hyperbolic tangent of a number
trunc(x)	| Returns the integer part of a number (x)

## Date Object
The Date object is used to work with dates and times.

Date objects are created with new Date().

There are four ways of instantiating a date

```javascript
var d = new Date();
var d = new Date(milliseconds);
var d = new Date(dateString);
var d = new Date(year, month, day, hours, minutes, seconds, milliseconds);
```