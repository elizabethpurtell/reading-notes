# Class 04 - HTML Links, JS Functions, and Intro to CSS Layout

## Statement

This section is taking me deeper into understanding the full spectrum of the inherent layout of pages. Better understanding of these layouts will help me design much faster using CSS.

---
---

### Learn HTML - Creating Hyperlinks

1. To create a basic link, we wrap text or other content inside what element?
    - We wrap the content within an '< a >' element.

2. The href attribute contains what information?
    - < href > attribute contains the web address, it's also called the Hypertext Reference or target.

3. What are some ways we can ensure links on our pages are accessible to all readers?
    - By adding link text you assure the screen readers are able to describe what the link goes to.
    - Each link should have a unique link text.
    - The link should describe if you are going to download something.

---

### CSS Layout, Normal Flow CSS Layout - Positioning

1. What is meant by “normal flow”?
    - This is the basic layout of an html page if zero CSS has been applied to the page.

2. What are a few differences between block-level and inline elements?
    - Block-level elements are laid out on a new line each time, whereas inline will fill the line its on until there is no more room.
    - Block-level elements span 100% of the width of the parent element, and are as tall as the child content. The total width and height is the content plus padding plus border width and height.
    - Inline elements sit on the same line with adjacent text nodes. Whatever doesn't fit on the line will wrap to the next line.

3. ___ positioning is the default for every html element.
    - "Static" positioning- means to put the elements into their normal position in the document flow, nothing different or special.

4. Name a few advantages to using absolute positioning on an element.
    - An absolute element no longer exists in the normal document flow. It gets its own layer.
    - You can change the "positioning context", which is the element the absolutely positioned element is positioned relative to.
    - The absolutely positioned element will be displayed outside of the < html > element and be positioned relative to the initial viewport.

5. What is a key difference between fixed positioning and absolute positioning?
    - "whereas absolute positioning fixes an element in place relative to its nearest positioned ancestor (the initial containing block if there isn't one), fixed positioning usually fixes an element in place relative to the visible portion of the viewport. " [Positioning html](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Positioning)

---

### Learn JS, Functions – Reusable Blocks of Code

1. Describe the difference between a function declaration and a function invocation.
    - *Function declaration* creates a new function, while a *function invocation* executes the code inside the function's body with specific arguments, if any, passing the result back to the caller. *Function declarations* define the function, while *function invocations* actually use or execute the function.

2. What is the difference between a parameter and an argument?
    - The key difference between a *parameter* and an *argument* is that a parameter is a variable name defined in the function declaration, while an *argument* is the actual value passed to the function when it is called. *Parameters* act as placeholders for the *arguments* that will be received by the function during its invocation.

---

### Miscellaneous - 6 Reasons for Pair Programming

1. Pick 2 benefits to pair programming and reflect on how these benefits could help you on your coding journey.
    - Greater Efficiency brought by 2 or more brains I find to be very true for large and/or complex projects. As a freelancer the last many years, I often reach out to others for a "second set of eyes" to help catch problems or give a second perspective. When you don't have that extra viewpoint you end up taking 2-3x as long on a project because you are eternally rechecking and not "seeing" your issues.
    - Work environment readiness: This aspect of pair programming will be absolutely detrimental to finding a new position within the programming world. I could come with all the training in the world, but if I am unable to work on a team and understand the continuous communication needs and languages then I will not be a good asset. By learning to work with other coders in team environments I will have a leg up on those that are learning completely alone.

---

### Bookmark and Review

[Functions](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Functions)

[6 Reasons for Pair Programming](https://www.codefellows.org/blog/6-reasons-for-pair-programming/)

---
---

## Things I want to know more about

I'd like to get a stronger foundation *in my brain* of the set of the standard measurements built into block and inline elements.

As a self-paced student, I do wish there were other opportunities for me to work with other students in things such as pair programming.
