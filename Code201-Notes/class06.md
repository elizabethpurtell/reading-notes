# Class 06 - Problem Domain, Objects, and the DOM

## Statement

This section of reading is going to help me grasp a better understanding of objects and the DOM with how they relate to JavaScript.

---
---

### JavaScript Object Basics

1. How would you describe an object to a non-technical friend you grew up with?

        Hey, you know how in Star Wars, there are characters, right? Well, think of an object in JavaScript like creating your own character sheet for a Star Wars RPG!

        Imagine you're making a character, and you want to give them cool abilities and traits, just like your favorite Star Wars heroes. An object in JavaScript is like a character sheet where you can write down all the things that make your character special.

        For instance, if you're making a Jedi character, your object could have a "lightsaberColor" property with the value "blue" to show they have a blue lightsaber. You could also give them a "forcePower" property with a value like "strong" or "weak," just like the different levels of Force abilities in Star Wars.

        But the really neat part is that you can add more than just those things to your character sheet. You can put in their name, age, home planet, and even make a space for their backstory. It's like you're creating a whole Star Wars character profile right in your code!

        So, in JavaScript, an object is like making your own Star Wars character with all the traits and details that you want, just as if you were getting ready to join the epic adventure in a galaxy filled with jedis, droids, and starships.

2. What are some advantages to creating object literals?

        Creating object literals in JavaScript offers several advantages. Object literals provide a straightforward way to define and initialize objects with a syntax that resembles everyday language. They are concise and don't require additional function calls or constructors. Object literals allow immediate property assignment, making them great for setting initial states. These literals are flexible and support nested properties, arrays, and dynamic property names. Their similarity to JSON simplifies data interchange. Object literals can be easily modified, cloned, or extended, aligning well with functional programming principles. They also help manage the global namespace and can be optimized for better performance.

3. How do objects differ from arrays?

        Objects are suitable for storing structured data with named attributes, while arrays are designed for ordered collections of values accessed by numerical indices.

4. Give an example for when you would need to use bracket notation to access an object’s property instead of dot notation.

        For Example: 
        const person = {
          "first name": "John",
          "last name": "Doe",
          age: 30,
        };
        const propertyName = "age";
        console.log(person[propertyName]);

        The value of the propertyName variable is used to dynamically access the age property of the person object.

        So, whenever you encounter property names that are not valid identifiers or you need to access properties dynamically using variables, you would use bracket notation.

5. Evaluate the code below. What does the term this refer to and what is the advantage to using this?
        "This" is referring to this particular dog named spot.
        const dog = {
          name: 'Spot',
          age: 2,
          color: 'white with black spots',
          humanAge: function (){
            console.log(`${this.name} is ${this.age*7} in human years`);
          }
        }

[JS Object Basics](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Basics)

---

### Introduction To The DOM

1. What is the DOM?

        The Document Object Model (DOM) is like a digital map that shows all the different parts of a webpage, such as text, images, and buttons. It helps web browsers understand how everything is arranged and what each piece does. Just like a map guides you through a city, the DOM guides the browser to show you the webpage correctly.

2. Briefly describe the relationship between the DOM and JavaScript.

        Imagine the DOM as a blueprint of a house, showing where all the rooms and furniture are. JavaScript is like a magical tool that lets you interact with this house. You can use JavaScript to move furniture around, change the color of the walls, or even add new rooms to the house. So, the DOM provides the structure of the house (webpage), and JavaScript helps you make changes and do cool things with it.

---

### Bookmark and Review

[Understanding the problem domain is the hardest part of programming](http://simpleprogrammer.com/2013/07/15/understanding-the-problem-domain-is-the-hardest-part-of-programming)

[What’s the difference between primitive values and object references in JavaScript?](https://betterprogramming.pub/intermediate-javascript-whats-the-difference-between-primitive-values-and-object-references-e863d70677b)

---
---

## Things I want to know more about

I would like to understand the Web API and how it works.
