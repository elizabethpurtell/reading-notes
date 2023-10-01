# Class 09 - Forms and JS Events

## Statement

In this set of reading we are learning about capturing information from our users and then using the information within the scripts we have made before. We learn about making a form so that those who aren't coding can easily input the information that we need to build out usable data.

---
---
###
 HTML Forms

1. Why are forms so important in web development?

        Forms are an important part of web development because they facilitate user interaction, data collection, and communication. Properly designed forms enhance the user experience, enable data validation, and support various functions that make websites more interactive and useful.

2. When designing a form, what are some key things to keep in mind when it comes to user experience?

        When designing a form for optimal user experience, prioritize clarity and simplicity with concise labels and instructions, minimize form length, provide logical flow, and use clear error handling. Make required fields evident, employ real-time validation, optimize for mobile, and ensure a prominent call to action. Address privacy and security concerns, confirm submissions, handle errors gracefully, test thoroughly, and prioritize accessibility. Continuously gather user feedback and make iterative improvements to create a user-friendly and efficient form that enhances the overall website experience.

3. List 5 form elements and explain their importance.

    1. *Text Input Field:* Text input fields allow users to enter alphanumeric text, such as names, email addresses, or search queries. They are fundamental for collecting user-generated content and data. Text input fields should be designed with clear labels and proper validation to ensure accurate data entry and a positive user experience.

    2. *Radio Buttons and Checkboxes:* Radio buttons and checkboxes are used for selecting options from a predefined list or making multiple selections. Radio buttons are typically used when users can choose only one option from a set, while checkboxes allow for multiple selections. These elements are crucial for user choices, such as gender selection or filtering search results by category.

    3. *Dropdown Menus:* Dropdown menus provide users with a list of options in a compact format, conserving screen space and reducing visual clutter. They are beneficial when there are many choices, like selecting a country or state in an address form. Dropdown menus improve usability and make it easier for users to select from a predefined set of options.

    4. *Textarea:* Textareas are larger input fields that enable users to enter longer text, such as comments, reviews, or messages. They are important for gathering detailed information or user feedback. Proper sizing and clear instructions can enhance the user experience when users need to provide more extensive responses.

    5. *Submit Button:* The submit button is the action element that users click to send their form data to the server for processing. It's a critical component that finalizes the user interaction with the form. The submit button should be prominently placed, clearly labeled, and accompanied by proper feedback, such as a confirmation message or a loading indicator, to inform users of the form's status after submission.

---

### Introduction To Events.

1. How would you describe events to a non-technical friend?

        JavaScript events are like triggers that make things happen on a web page. Imagine them as buttons or sensors that respond when you interact with a webpage, like clicking a button or moving your mouse over an image. When an event occurs, it can make text change, show or hide things, or even play videos. These events make websites feel dynamic and interactive, like they're responding to your actions, making the web more engaging and user-friendly.

2. When using the addEventListener() method, what 2 arguments will you need to provide?

        Event Type (String): This is the first argument and specifies the type of event you want to listen for, such as "click," "keydown," "mouseover," or "submit." It defines the specific interaction or action that will trigger the event handler function.

        Event Handler Function (Function): The second argument is a reference to the function that should be executed when the specified event occurs. This function will be responsible for defining what happens in response to the event. It can be an inline function or a reference to a named function.

3. Describe the event object. Why is the target within the event object useful?

        The event object in JavaScript is a built-in object that contains information about an event when it occurs in the browser. It serves as a container for various details related to the event, including the event type, the target element that triggered the event, and additional data specific to the event type.

        The target property within the event object is exceptionally useful because it references the DOM element that initially triggered the event. This is valuable because it allows you to precisely identify which element on the webpage was interacted with to trigger the event. This information is crucial when you have multiple elements with event listeners, as it enables you to determine which specific element caused the event to occur. Consequently, you can then use this knowledge to tailor your JavaScript code to respond appropriately to that particular element's interaction, facilitating dynamic and context-aware web interactions.

4. What is the difference between event bubbling and event capturing?

    Event bubbling and event capturing are two phases in the event propagation process in the Document Object Model (DOM) of web browsers. They describe the order in which events are triggered when an event occurs on an element that is nested within other elements.

    Event bubbling starts with the target element and moves up the DOM hierarchy, while event capturing starts at the root and moves down to the target. Understanding these two phases is important when dealing with nested elements and controlling the order in which event handlers are executed.

    Here are the key differences between the two:

    Event Flow Direction:

        Event Bubbling: In event bubbling, the innermost element's event is handled first, and then the event bubbles up from the target element to the outermost (document) element. It starts at the target and moves up the DOM hierarchy to the root element.

        Event Capturing: Event capturing, also known as trickling, is the opposite. It starts at the root element and moves down to the target element, triggering events on each ancestor element along the way.    

    Phases:

        Event Bubbling: Bubbling occurs during the "bubbling phase" of event propagation. This is the default behavior for most DOM events.

        Event Capturing: Capturing happens during the "capturing phase" of event propagation. It's less commonly used but can be explicitly enabled for specific events.

    Order of Execution:

        Event Bubbling: Events are handled first by the target element, then its parent, and so on, until reaching the root element (document). This means the innermost element's event handler is executed before the outer elements.

        Event Capturing: Events are processed in the opposite order. Starting from the root element, the event travels down the DOM hierarchy, so the outermost element's event handler is executed before the inner elements.

    EventListener Options:

        When adding event listeners using "addEventListener", you can specify whether you want to use event capturing by setting the third parameter to true (capture) or false (bubbling). If you omit this parameter or set it to false, the event will use bubbling by default.

---

### Bookmark and Review

[HTML5 Input Types](https://developer.mozilla.org/en-US/docs/Learn/Forms/HTML5_input_types)

[Event Reference and listings](https://developer.mozilla.org/en-US/docs/Web/Events)

---
---

## Things I want to know more about

    What is the most intricate way a `target` property will be used in javascript?

    I decided to ask the AI this question and this is the answer I recieved:
    
    The `target` property in JavaScript is commonly used to identify the DOM element that triggered an event, making it a fundamental part of event handling. While its usage can vary depending on the specific needs of an application, here's an example of a more intricate way the `target` property can be used:

    Consider a complex web application with a dynamic user interface where various elements can be added, modified, or removed dynamically. You want to implement a feature where users can edit the text content of any element on the page by double-clicking on it. To achieve this, you might do the following:

    1. Attach a single event listener to the document or a container element, capturing the double-click event (`dblclick`).

    2. In the event handler function, access the `event.target` property to determine which element was double-clicked.

    3. Check if the clicked element is of a type that can be edited (e.g., a `div`, `span`, or `p` element) and doesn't have any existing input fields within it.

    4. If the clicked element meets the criteria, create a new editable input field dynamically and replace the original content with the input field.

    5. Attach a blur event listener to the input field to capture when the user finishes editing.

    6. When the input field loses focus (on blur), update the content of the original element with the edited text from the input field.

    7. Remove the input field from the DOM to restore the original appearance.

    8. Ensure you handle cases where the user cancels the edit or encounters an error gracefully.

    In this scenario, the `target` property plays a crucial role in determining which element was double-clicked and needs to be edited. By dynamically creating and manipulating DOM elements based on the `target`, you can provide a sophisticated and user-friendly editing feature that adapts to various parts of the web page.

    This example showcases a more intricate use of the `target` property in JavaScript, where it helps manage dynamic interactions within a complex web application.
