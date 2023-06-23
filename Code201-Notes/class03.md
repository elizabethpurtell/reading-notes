# Class 03 - Lists, The Box Model, and Loops

## Statement

This is a review of the basics from Code 102 covering HTML, CSS and JS. This review will help with diving deeper into JS in the coming labs.

---
---

### Learn HTML, Ordered and Unordered Lists

1. When should you use an unordered list in your HTML document?
    Unordered lists are used for a set of items that have no specific order and uses bullet points to separate.

2. How do you change the bullet style of unordered list items?
    You can change the bullet style by changing the style with 'list-style-type' property applied to the element.

3. When should you use an ordered list vs an unorder list in your HTML document?
    Ordered lists are used when it changes the meaning of the list if the items aren't in a specific order. Some examples would be displaying directions or steps to build something. Unordered lists don't require a specific listing because nothing changes if the order is mixed up.

4. Describe two ways you can change the numbers on list items provided by an ordered list?
    You can change the numbers in an ordered list by changing the attribute to either 'reversed', which reverses the list order, or change the attribute 'type' to several different options like lowercase letters or uppercase Roman numerals.

---

### Learn CSS, The Box Model

1. Describe the CSS properties of margin and padding as characters in a story. What is their role in a story titled: “The Box Model”?

    In the world of "The Box Model," Margin and Padding were inseparable characters. Margin created space and distance between objects, while Padding provided warmth and protection. They balanced the needs of elements, maintaining boundaries and enhancing the user experience. Together, they taught us the importance of personal space and nurturing surroundings in web design. [ChatGPT Story](https://chat.openai.com/share/c2837386-8962-4d3b-9da1-ae788c1a61e4)

2. List and describe the four parts of an HTML elements box as referred to by the box model.

- Content box: The content is displayed in here. I think of it like a closet in a house.

- Padding box: The area directly around the content. I consider this area the 'personal space' around each content item.

- Border box: This wraps the content and any padding. This is the structure of the closet surrounding the content.
  
- Margin box: This is the outermost layer, wrapping the content, padding, and border as whitespace between this box and other elements. I think of this as the house that the closet ( content ) resides in.

---

### Learn JS, Arrays, Operators & Expressions, Conditionals, Loops

1. What data types can you store inside of an Array?

- Numbers: Integers, floating-point numbers, or even special numeric values like NaN or Infinity.
- Strings: Textual data enclosed in single quotes ('') or double quotes ("").
- Booleans: The values true or false, representing logical conditions.
- Objects: JavaScript objects, which can hold key-value pairs or complex data structures.
- Functions: JavaScript functions, which can be stored and called later.
- Arrays: Arrays can store other arrays, enabling the creation of multi-dimensional arrays.
- Null: A special value denoting the absence of any object value.
- Undefined: A value assigned to variables that have been declared but not assigned any value.
- Symbols: Unique and immutable values used as object property identifiers.

  It's important to note that JavaScript arrays are not restricted to a specific data type, allowing flexibility in mixing different data types within the same array. For example, an array could contain a combination of numbers, strings, and objects all in one.

2. Is the people array a valid JavaScript array? If so, how can I access the values stored? If not, why?

    I believe it's a valid JavaScript array, it's a multidimensional array.

``` md

    const people = [['pete', 32, 'librarian', null], ['Smith', 40, 'accountant', 'fishing:hiking:rock_climbing'], ['bill', null, 'artist', null]];

 ```

3. List five shorthand operators for assignment in JavaScript and describe what they do.

- ' += ': adds the value on the right-hand side to the existing value of the variable on the left-hand side, and then assign the result back to the variable. It is commonly used for concatenating strings or incrementing numeric values.

- ' -=': subtracts the value on the right-hand side from the existing value of the variable on the left-hand side, and then assigns the result back to the variable. It is used to decrement numeric values.

- ' *= ': multiplies the value on the right-hand side with the existing value of the variable on the left-hand side, and then assigns the result back to the variable. It is used for multiplying numeric values.

- ' /= ': divides the existing value of the variable on the left-hand side by the value on the right-hand side, and assigns the result back to the variable. It is used for dividing numeric values.

- ' %= ': divides the existing value of the variable on the left-hand side by the value on the right-hand side and assigns the remainder back to the variable. It is used for calculating the remainder when dividing numeric values.

4. Read the code below and evaluate the last expression and explain what the result would be and why.

- a is assigned the value 10, which is a numeric data type.
- b is assigned the value 'dog', which is a string data type.
- c is assigned the value false, which is a boolean data type.

- a + c is asking to add 10 to 'false', and false numeric amount is zero.
- the expression then becomes 10 + 'dog', becoming '10dog' a string.

```md

 let a = 10;
 let b = 'dog';
 let c = false;

 // evaluate this
 (a + c) + b;

 ```

5. Describe a real world example of when a conditional statement should be used in a JavaScript program.

    A real world example might be an app that gives suggestions on what to wear each day dependent on the temperature and weather outside. It could evaluate the data given by an external API that monitors the local weather. The JS program would store the temperature data in a variable, then would have conditional statements based on the different temperatures, which would return a message to the user about what type of clothing would be appropriate.

6. Give an example of when a Loop is useful in JavaScript.

    A good example of a useful loop in JS would be one where you want to check the grades of all the students in a particular class.

---

### Bookmark and Review

[Learn HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)

[The Box Model](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/The_box_model)

[Learn JavaScript](https://developer.mozilla.org/en-US/docs/Learn/JavaScript)

[Template Literals](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Template_literals)

---
---

## Things I want to know more about

- String Interpolation or a template literal, its another type of string concatenation. Uses the '${ function name }' in order to remove having to use all the addition signs in the string concatenation.
