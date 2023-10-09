# Class 14 - Documentation, Project Selection, & Team Workflow

## Statement

This section of readings dive deeper into the ways we can make build more seemless webpages that are interactive, interesting and user-friendly.

---
---

### CSS Transforms

1. What does a CSS transform allow the developer to do to an element?

    A CSS transform allows developers to change how an element looks and behaves on a webpage. It can be used to do things like rotate, scale, or move an element. For example, you can rotate an image, make a button grow bigger when you hover over it, or slide in a menu from the side of the screen. Transforms are like magical tools that give developers the power to make elements on a webpage move and change shape in creative and interactive ways, adding flair and interactivity to websites.

2. Provide an example of a transform and how you could see that being used on a website.

    Let's say you have a button on your website, and when a user hovers their mouse pointer over it, you want the button to grow slightly in size to give it a subtle interactive effect. You can achieve this using CSS transforms.

    Here's the HTML and CSS code for such an effect:

    HTML-

```html

   <button class="grow-button">Hover me!</button>

```

```css

  .grow-button {
  width: 100px;
  height: 40px;
  background-color: #3498db;
  color: #fff;
  border: none;
  transition: transform 0.2s; /* Add a smooth transition for the transform */
}

.grow-button:hover {
  transform: scale(1.1); /* On hover, make the button 10% larger */
}

```

---

### CSS Transitions & Animations

1. What does a CSS transition allow the developer to do to an element?

    A CSS transition allows a developer to control how an element changes from one state to another smoothly over a specified duration when a particular property is modified. In simpler terms, it lets you create gradual and visually pleasing effects when elements on a webpage change.

2. How does a CSS animation differ from a CSS transition?

    CSS transitions are best for creating simple and smooth property changes triggered by events, while CSS animations offer greater flexibility and control for creating a wide range of complex animations that can loop, run automatically, or respond to specific events over a defined timeline using keyframes.

---

### 8 simple CSS3 transitions that will wow your users

1. What are some benefits to using CSS transitions on websites?

    Using CSS transitions on websites offers several advantages. They enhance the user experience by smoothing transitions between different states or actions, making the interface more intuitive and engaging. CSS transitions can improve readability by gently highlighting changes in content, such as fading in new information or gradually revealing hidden elements. These effects can also be accessible to users with disabilities, providing clear visual cues and preventing sudden disruptions. Additionally, transitions contribute to responsive design, ensuring that web content adapts gracefully to different screen sizes and orientations. They are typically performance-optimized, resulting in smooth animations that don't strain device resources. From a development perspective, CSS transitions are relatively simple to implement, requiring minimal code and offering cross-browser compatibility. Overall, they are a valuable tool for creating visually appealing and user-friendly websites that enhance user engagement and accessibility while maintaining performance and compatibility.

2. How does this topic fit in with your long-term goals?

    As I want to move deeper into front end web design, using animations and transitions will be an essential portion of my code so I can create smooth running beautiful designs.

### Bookmark and Review

[Pure CSS Bounce Animation](http://codepen.io/dp_lewis/pen/gCfBv)

[6 Buttons animated](http://codepen.io/retyui/pen/ByoaXV)

[CSS3 Animations: Keyframes](http://codepen.io/akshaychauhan/pen/oAfae)

[404](http://codepen.io/kieranfivestars/pen/MYdQxX)

---
---

## Things I want to know more about

I want to look deeper into using animations with keyframes. I have had a comprehensive amount of training in Autodesk: Maya and am interested in seeing the differences, and using my knowledge from Maya to make these animations more complex.
