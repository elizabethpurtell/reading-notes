# Class 07 - HTML Tables and JS Constructor Functions, Object-Oriented Programming, HTML Tables

## Statement

This class gives a basic overview of how tables work in HTML and the basics of understanding constructors with functions. We are taking the next steps in building more complex Javascript code. Using these two main things we could begin to gather data and place it into tables within our JS.

---
---

### Domain Modeling

1. Explain why we need domain modeling.

      Domain modeling in JavaScript is essential because it provides a structured way to represent real-world entities and their interactions within software applications. It helps organize code by defining classes, properties, and methods, making it easier to manage complexity, promote code reusability, and create a clear and maintainable software architecture. Domain modeling also facilitates communication and collaboration among developers, ensuring that the codebase accurately reflects the application's underlying business logic and requirements.

---

### HTML Table Basics

1. Why should tables not be used for page layouts?

      Using tables for webpage layouts in HTML is discouraged because it contradicts semantic markup principles, leading to accessibility issues for users with disabilities and SEO concerns. Tables create complex, hard-to-maintain layouts, resulting in slower page loading times and compatibility issues with older browsers. They also hinder responsive design and future-proofing. To achieve flexible and accessible layouts, it's better to use semantic HTML elements (e.g., < header >, < main >) along with CSS for styling and positioning, adhering to modern web standards and best practices.

2. List and describe 3 different semantic HTML elements used in an HTML < table >.

      The < td > table data element is the smallest container inside a table. Each cell will automatically go to the right creating the first row.

      The < tr > table row element organizes the rows by being added to the beginning and ending of the td elements. 

      The < th > table header element will create a header, that will allow for better readability and accessibility.

---

### Introducing Constructors

1. What is a constructor and what are some advantages to using it?

      In JavaScript, a constructor is a special function used to create and initialize objects based on a predefined blueprint. The advantages of using constructors include code reusability, encapsulation of object creation logic, prototype inheritance for shared methods and properties, consistency in object structure, custom initialization options, and improved code readability by making your intent to create specific object types clear. Constructors are a fundamental tool in JavaScript's object-oriented programming paradigm.

2. How does the term "this" differ when used in an object literal versus when used in a constructor?

      In an object literal, the "this" keyword refers to the object itself and allows you to access its properties and methods. In a constructor function, "this" refers to the instance being created with the "new" keyword, and it allows you to set and access properties specific to that instance. Essentially, "this" in an object literal refers to the object it's contained within, while in a constructor, it refers to the instance of the object being created.

---

### Object Prototypes Using A Constructor

1. Explain prototypes and inheritance via an analogy from your previous work experience. NOTE: This is a very common front end developer interview question.

      Think of prototypes and inheritance like templates and variations in graphic design. A prototype is your base design template, defining the core elements and style. Inheritance is creating variations of that design by maintaining the core elements while making specific changes, like altering colors or adding new elements. Just as variations inherit the essence of the prototype, objects in JavaScript inherit properties and methods from their prototypes, allowing for efficient code reuse and customization.

---

### Bookmark and Review

[HTML Table Advanced Features and Accessibility](https://developer.mozilla.org/en-US/docs/Learn/HTML/Tables/Advanced)

---
---

## Things I want to know more about

Prototypal Instantiation
