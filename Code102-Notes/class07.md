# Class 07:  Programming with JavaScript

## Control Flow, Operators & Functions

---
---

### Control Flow

Control flow means that when you read a script, you must not only read from start to finish but also look at program structure and how it affects order of execution.

- The control flow is the order in which the computer executes statements in a script.
- Code is run in order from the first line in the file to the last line, unless the computer runs across the (extremely frequent) structures that change the control flow, such as *conditionals and loops.*
Conditional structure: ‘If…else’

- The control flow is the order in which the computer executes statements in a script. Code is run in order from the first line in the file to the last line, unless the computer runs across the (extremely frequent) structures that change the control flow, such as conditionals and loops.

```md

if (isEmpty(field)) {
  promptUser();
} else {
  submitForm();
}

```

### JavaScript Functions

- A JavaScript function is a block of code designed to perform a particular task.
- A JavaScript function is executed when "something" invokes it (calls it).

### JavaScript Function Syntax

A JavaScript function is defined with the function keyword, followed by a name, followed by parentheses ().

- Function names can contain letters, digits, underscores, and dollar signs (same rules as variables).
- The parentheses may include parameter names separated by commas:
(parameter1, parameter2, ...)
- The code to be executed, by the function, is placed inside curly brackets: {}

- Function parameters are listed inside the parentheses () in the function definition.

- Function arguments are the values received by the function when it is invoked.

- Inside the function, the arguments (the parameters) behave as local variables.

### Function Invocation

The code inside the function will execute when "something" invokes (calls) the function:

- When an event occurs (when a user clicks a button)
- When it is invoked (called) from JavaScript code
- Automatically (self invoked)

### Function Return

- When JavaScript reaches a return statement, the function will stop executing.
- If the function was invoked from a statement, JavaScript will "return" to execute the code after the invoking statement.
- Functions often compute a return value. The return value is "returned" back to the "caller":

### Why Functions?

- With functions you can reuse code
- You can write code that can be used many times.
- You can use the same code with different arguments, to produce different results.

### The () Operator

- The () operator invokes (calls) the function
- Accessing a function with incorrect parameters can return an incorrect answer
- Accessing a function without () returns the function and not the function result

### Functions Used as Variable Values

Functions can be used the same way as you use variables, in all types of formulas, assignments, and calculations.

### Local Variables

Variables declared within a JavaScript function, become LOCAL to the function.
Local variables can only be accessed from within the function.
Since local variables are only recognized inside their functions, variables with the same name can be used in different functions.
Local variables are created when a function starts, and deleted when the function is completed.

### JavaScript Operators

The Addition Operator + adds numbers
The Assignment Operator = assigns a value to a variable.
The Multiplication Operator (*) multiplies numbers

### Types of JavaScript Operators

There are different types of JavaScript operators:

- Arithmetic Operators: are used to perform arithmetic on numbers
- Assignment Operators: assign values to JavaScript variables.
- Comparison Operators:
- String Operators:
- Logical Operators:
- Bitwise Operators:
- Ternary Operators:
- Type Operators:

### JavaScript String Comparison

All the comparison operators above can also be used on strings
avaScript String Addition
The + can also be used to add (concatenate) strings
The += assignment operator can also be used to add (concatenate) strings
When used on strings, the + operator is called the concatenation operator.
Adding two numbers, will return the sum, but adding a number and a string will return a string

### JavaScript Bitwise Operators

Bit operators work on 32 bits numbers.
Any numeric operand in the operation is converted into a 32 bit number. The result is converted back to a JavaScript number.

### Operators and Operands

The numbers (in an arithmetic operation) are called operands.
The operation (to be performed between the two operands) is defined by an operator.

### Incrementing/Decrementing

The increment operator (++) increments numbers.
The decrement operator (--) decrements numbers.

### Operator Precedence

Operator precedence describes the order in which operations are performed in an arithmetic expression.
As in traditional school mathematics, the multiplication is done first.
Multiplication (*) and division (/) have higher precedence than addition (+) and subtraction (-).
And (as in school mathematics) the precedence can be changed by using parentheses.
When using parentheses, the operations inside the parentheses are computed first.
When many operations have the same precedence (like addition and subtraction or multiplication and division), they are computed from left to right.

---

[Link to W3 Assignment Operator quick sheet](https://www.w3schools.com/js/js_assignment.asp)
[Expressions and Operators MDNwebdocs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators)
[Functions MDNwebdocs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions)

---
---

## Answer

1. What is control flow?

    Control flow is the steps the computer takes in a sequence in order to complete the instructions in a script.

2. What is a JavaScript function?

    A JS function is a chunk of code that has a specific task, usually by taking input then giving an output.

3. What does it mean to invoke - or call - a function?

    It means you are telling that function to run its course.

4. What are the parenthesis () for when you define a function?

    The parentheses () operator are what invokes (calls) the function.

---
---
