# Class 06: JavaScript

## Making Dynamic Pages with JavaScript

---
---

### What is JavaScript?

```md

What is JavaScript?
JavaScript is a scripting language that enables you to create dynamically updating content, control multimedia, animate images, and pretty much everything else.

```

[Quote link](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/What_is_JavaScript)

### Who wrote it and when?

JavaScript was invented by Brendan Eich in 1995, and became an ECMA standard in 1997.

ECMA-262 is the official name of the standard. ECMAScript is the official name of the language.

Class notes

- Variables- different ways to declare them
- var- OLD WAY do not use!
- const - constant, can NOT be changed
- We use JS to interact w/webpages
- It’s an object-oriented-programming language
- Turns websites into applications by user interaction
- Debugging- finding errors then fixing them
- Uses a console
- Functions! Makes code reusable (in class 7)
- input/output
- JS is not JAVA! 2 different things made by Oracle
- In HTML, JS is inserted between a < script tag >
- JavaScript is the default scripting language in HTML.
- A JavaScript function is a block of JavaScript code, that can be executed when "called" for.
- You can place any number of scripts in an HTML document.
- Scripts can also be placed in external files like myscript . js
- Scripts can be placed in the < body >, or in the < head > section of an HTML page, or in both.
-

### What can JS do?

- JS can change HTML attribute values
- JS can change HTML Styles - css
- JS can hide/show HTML Elements
- JS can hide HTML Elements

### External JavaScript Advantages

Placing scripts in external files has some advantages:

- It separates HTML and code
- It makes HTML and JavaScript easier to read and maintain
- Cached JavaScript files can speed up page loads

### JavaScript Display Possibilities

JavaScript can "display" data in different ways:

- Writing into an HTML element, using innerHTML.
- Writing into the HTML output using document.write().
- Writing into an alert box, using window.alert().
- Writing into the browser console, using console.log().

### JavaScript statements are composed of

Values, Operators, Expressions, Keywords, and Comments.

- Semicolons separate JavaScript statements.
- JavaScript ignores multiple spaces. You can add white space to your script to make it more readable.
- For best readability, programmers often like to avoid code lines longer than 80 characters.
- JavaScript statements can be grouped together in code blocks, inside curly brackets {...}.The purpose of code blocks is to define statements to be executed together.
- JavaScript statements often start with a keyword to identify the JavaScript action to be performed.

### JS Keywords

*JavaScript keywords are reserved words. Reserved words cannot be used as names for variables.*

| Keyword     | Descriptions |
| ----------- | ----------- |
|var| Declares a variable|
|let| Declares a block variable|
const| Declares a block constant|
|if| Marks a block of statements to be executed on a condition|
|switch| Marks a block of statements to be executed in different cases|
|for| Marks a block of statements to be executed in a loop|
|function| Declares a function|
|return| Exits a function|
|try |Implements error handling to a block of statements|

---

[How Computers Work- Playlist](https://www.youtube.com/playlist?list=PLzdnOPI1iJNcsRwJhvksEo1tJqjIqWbN-)

---

[JavaScript Guide](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide)

[JavaScript Reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference)

[Use Replit to play with JS](https://replit.com/~)

---

### JavaScript Values

The JavaScript syntax defines two types of values:

1. Fixed values are called Literals.
2. Variable values are called Variables.

### JavaScript Literals

The two most important syntax rules for fixed values are:

1. Numbers are written with or without decimals
2. Strings are text, written within double or single quotes

### Variables

Variables are containers for storing data (storing data values).In a programming language, variables are used to store data values. JavaScript uses the keywords var, let and const to declare variables.
An equal sign is used to assign values to variables.

- You declare a variable by using keywords var, let and const
- its like a tag you put on a box
- declaring means you are creating a variable for the first time
- the variable needs to match what you are assigning it

#### 4 ways to declare a JS Variable

- using var (old way no longer using)
- using let
- using const
- using nothing

---

### JavaScript Let

- Variables defined with let can not be redeclared.
- Variables defined with let must be declared before use.
- Variables defined with let have block scope.

### Why is it important to use Let instead of the old var

- Redeclaring a variable using the var keyword can impose problems.
Redeclaring a variable inside a block will also redeclare the variable outside the block.
- Redeclaring a variable using the let keyword can solve this problem.
Redeclaring a variable inside a block will not redeclare the variable outside the block:
- Let Hoisting
Variables defined with var are hoisted to the top and can be initialized at any time. Meaning: You can use the variable before it is declared.
- Variables defined with let are also hoisted to the top of the block, but not initialized. Meaning: Using a let variable before it is declared will result in a ReferenceError.

### JavaScript const

- JavaScript const variables must be assigned a value when they are declared
- If you want a general rule: always declare variables with const.
- If you think the value of the variable can change, use let.
- Variables defined with const cannot be Redeclared.
- Variables defined with const cannot be Reassigned.
- Variables defined with const have Block Scope.

#### Use const when you declare

- A new Array
- A new Object
- A new Function
- A new RegExp

### JavaScript Operators

- uses arithmetic operators ( + - * / ) to compute values
- uses an assignment operator ( = ) to assign values to variables

#### Equal Signs =

- In JavaScript, the equal sign ( = ) is an "assignment" operator, not an "equal to" operator.
- equal signs do not mean things are actually equal in JS
- two equal signs = = means equal to
- three equal signs = = = means strictly true

### JavaScript Expressions

An expression is a combination of values, variables, and operators, which computes to a value.
The computation is called an evaluation.

### JavaScript Comments

Not all JavaScript statements are "executed".
Code after double slashes // or between /*and*/ is treated as a comment.
Comments are ignored, and will not be executed

#### JavaScript Identifiers

- All JavaScript variables must be identified with unique names.
- These unique names are called identifiers.
- Identifiers can be short names (like x and y) or more descriptive names (age, sum, totalVolume).
- *Numbers are not allowed as the first character in names.*
- **Hyphens are not allowed in JavaScript. They are reserved for subtractions.**

*The general rules for constructing names for variables (unique identifiers) are:*

- Names can contain letters, digits, underscores, and dollar signs.
- Names must begin with a letter.
- Names can also begin with $ and _
- Names are **case sensitive** (y and Y are different variables).
- Reserved words (like JavaScript keywords) cannot be used as names.

### Unicode

JavaScript uses the Unicode character set.
Unicode covers (almost) all the characters, punctuations, and symbols in the world.

#### JavaScript Data Types

- JavaScript variables can hold numbers like 100 and text values like "John Doe".
- In programming, text values are called text strings.
- JavaScript can handle many types of data, but for now, just think of numbers and strings.
- Strings are written inside double or single quotes. Numbers are written without quotes.
- If you put a number in quotes, it will be treated as a text string.

#### JavaScript has 8 Datatypes

1. String
2. Number
3. Bigint
4. Boolean
5. Undefined
6. Null
7. Symbol
8. Object

#### The Object Datatype

The object data type can contain:

1. An object
2. An array
3. A date

#### You can declare many variables in one statement

- Start the statement with let and separate the variables by comma
- A declaration can span multiple lines

#### Value = undefined

In computer programs, variables are often declared without a value. The value can be something that has to be calculated, or something that will be provided later, like user input.
*A variable declared without a value will have the value undefined.*

---

### Dynamic Components

- ' document.write( username ) '- is a way you can write js to html

---

#### Standard Objects

| Object      | Define |
| ----------- | ----------- |
| Object     | fundamental language constructs     |
| Function     | fundamental language constructs     |
| Boolean    | fundamental language constructs     |
| Symbol     | fundamental language constructs     |
| Number    | base objects representing numbers, dates, and mathematical calculations    |
| BigInt    | base objects representing numbers, dates, and mathematical calculations      |
| Math     | base objects representing numbers, dates, and mathematical calculations     |
| Date     | base objects representing numbers, dates, and mathematical calculations     |
| String     | represent strings and support manipulating them     |
| RegExp     | represent strings and support manipulating them      |

---
---

## Answer

1. What are variables in JavaScript?
    - Variables are objects that you can store information
2. What does it mean to declare a variable?
    - Declaring means you are creating a variable for the first time
3. What is an “assignment” operator, and what does it do?
    - Assignment operators assign values to JS variables using the equal sign ( = ) .
4. What is information received from the user called?
    - When the user gives an answer ( by pressing okay/submit ) to our questions, it's called "input value". The user input is then stored in a variable to be used as information in our program.

---
---
