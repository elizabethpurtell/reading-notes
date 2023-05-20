# Class 04: Structure Web Pages with HTML

## Reflection and Discussion

---
---

[Wireframe and Design](https://careerfoundry.com/en/blog/ux-design/how-to-create-your-first-wireframe/)

“Wireframing is a practice used by UX designers which allows them to define and plan the information hierarchy of their design for a website, app, or product. This process focuses on how the designer or client wants the user to process information on a site, based on the user research already performed by the UX design team.”

**What is wireframing?**

In very basic terms, wireframing is an outline for a digital site. It’s a way to lay out everything that you want to include in a page, then organize it with the best readable and user-friendly design possible. Wireframing allows the designer to plan out all that is needed to build a site and then play with it before writing all the code that is needed to build it. They are always done in black/white/greys so you aren’t distracted by color.

**How do you make a wireframe?**

There are several ways to make wireframes. You can draw them out on paper, a whiteboard, or build them with a design program. There are several design programs out there like Adobe XD, Figma, Invision and Balsamic. If done by paper then you can cut out and play with your different ideas.

[Some ideas here for making wireframes](https://careerfoundry.com/en/blog/ux-design/website-app-wireframe-examples/)

### 6 Steps to Build a Wireframe

1. Research! - your audience, your website address, etc.
2. Prepare your research for quick reference
3. Prepare your user flow to keep yourself on track while building
4. Draft an outline of your site using these questions to lead your design:
    - How can you organize the content to support your users’ goals?
    - Which information should be most prominent?
    - Where should your main message go?
    - What should the user see first when arriving at the page?
    - What will the user expect to see on certain areas of the page?
    - Which buttons or touch points does the user need to complete the desired actions?
5. Add detail and get testing!
    - Usability conventions, such as putting the navigation at the top next to your logo, having a search box on the top right, and so on
    - Simple, instructional wording for i.e. calls-to-action
    - Trust-building elements: What do you need to build trust in your customers and where would be the best place to put these elements?
    - Tooltips to indicate any functionality that could be included in a prototype transition
6. Time to turn your wireframe into a prototype!

**Three principles you need for a good wireframe**

1. Clarity: Your wireframe needs to answer the questions of what that site page is, what the user can do there, and if it satisfies their needs.
2. Confidence: Ease of navigation through your site and clear calls-to-action increase user confidence in your brand.
3. Simplicity: Too much information, copy, or links, can be distracting to the user and will have a detrimental affect on your users’ ability to achieve their goals.

---

## What is HTML?

HTML (HyperText Markup Language) is the code that is used to structure a web page and its content.
HTML is a markup language that defines the structure of your content. HTML consists of a series of elements, which you use to enclose, or wrap, different parts of the content to make it appear a certain way, or act a certain way. The enclosing tags can make a word or image hyperlink to somewhere else, can italicize words, can make the font bigger or smaller, and so on.

**The main parts of our element are as follows:**

- The opening tag: This consists of the name of the element (in this case, p), wrapped in opening and closing angle brackets. This states where the element begins or starts to take effect — in this case where the paragraph begins.
- The closing tag: This is the same as the opening tag, except that it includes a forward slash before the element name. This states where the element ends — in this case where the paragraph ends. Failing to add a closing tag is one of the standard beginner errors and can lead to strange results.
- The content: This is the content of the element, which in this case, is just text.
- The element: The opening tag, the closing tag, and the content together comprise the element.

**Attributes that set a value always have:**

- A space between it and the element name (or the previous attribute, if the element already has one or more attributes).
- The attribute name followed by an equal sign.
- The attribute value wrapped by opening and closing quotation marks.

### Nesting elements

You can put elements inside other elements too — this is called *nesting*. If we wanted to state that our cat is very grumpy, we could wrap the word "very" in a "strong" element, which means that the word is to be strongly emphasized: You do however need to make sure that your elements are properly nested.

### Void elements

Some elements have no content and are called void elements. Take the "<img>" element that we already have in our HTML page:

[Mozilla HTML Basics](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics)

### Semantics

In programming, Semantics refers to the meaning of a piece of code — for example "what effect does running that line of JavaScript have?", or "what purpose or role does that HTML element have" (rather than "what does it look like?".)

### Semantics in JavaScript

In JavaScript, consider a function that takes a string parameter, and returns an <li> element with that string as its textContent. Would you need to look at the code to understand what the function did if it was called build('Peach'), or createLiWithContent('Peach')?

**Semantics in CSS**

In CSS, consider styling a list with li elements representing different types of fruits. Would you know what part of the DOM is being selected with div > ul > li, or .fruits__item?

**Semantics in HTML**

In HTML, for example, the h1 element is a semantic element, which gives the text it wraps around the role (or meaning) of "a top level heading on your page."

#### Some of the benefits from writing semantic markup are as follows:

- Search engines will consider its contents as important keywords to influence the page's search rankings (see SEO)
- Screen readers can use it as a signpost to help visually impaired users navigate a page
- Finding blocks of meaningful code is significantly easier than searching through endless divs with or without semantic or namespaced classes
- Suggests to the developer the type of data that will be populated
- Semantic naming mirrors proper custom element/component naming

#### Semantic elements

These are some of the roughly 100 semantic elements available. [Here](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)
[Great resource for learning HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)
[Semantics](https://developer.mozilla.org/en-US/docs/Glossary/Semantics)

---
---

### Answer

1. **What is HTML and why do we use it?**

    HTML is a markup language that allows us to give structure to a website by using elements. We use it so that the page has structure and not just a big collection of overwhelming text.

2. **What are the 3 main parts of an HTML element?**

    The opening tag (or start tag) marks where the element's content begins (<p> in the example above). The closing tag (or end tag) marks the end of the element's content (</p> above).

3. **What is it called when you give an element extra information?**

    Attributes contain extra information about the element that you don't want to appear in the actual content.

4. **What is a semantic element?**

    In programming, Semantics refers to the meaning of a piece of code.

---
