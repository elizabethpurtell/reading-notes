# Class 08 - CSS Layout

## Statement

Learning Flexbox will speed up my designs and help with continuity and usablity of my future pages.

---
---

### Learn CSS - Flexbox

1. Flexbox is designed for one-dimensional content. Explain what this means.

      Flexbox primarily deals with the layout of elements along a single axis, either horizontally or vertically, but not both at the same time. This is in contrast to the Grid layout, which is designed for two-dimensional content arrangement along both the horizontal and vertical axes.

2. Explain the difference between the main axis and cross axis.

      The main axis is the primary direction in which the elements are arranged (either horizontally or vertically), and the cross axis is the perpendicular direction. You can control how elements distribute and align themselves along these axes.

3. How can using certain properties of flexbox negatively impact accessibility?

      *Reordering Content*- Screen readers and other assistive technologies rely on the order of content in the HTML source code to provide a meaningful reading order. If you use the order property to change the visual order significantly, it can confuse users who rely on screen readers.

      *Insufficient Spacing and Overlapping*- This can make it difficult for users with motor disabilities or vision impairments to interact with or perceive content properly. It's important to ensure that there is sufficient spacing and no content overlap to improve accessibility.

      *Lack of Keyboard Navigation Support*- Keyboard users should be able to navigate and interact with the elements in the Flexbox layout using the tab and arrow keys. Failing to implement proper keyboard support can make the content inaccessible to users who rely on keyboards or other assistive devices.

      *Inadequate Use of ARIA Roles and Attributes*- When using Flexbox, it's essential to use ARIA roles and attributes appropriately to convey the structure and relationships of the content. Failure to do so can result in screen readers not providing the expected information to users with disabilities.

      *Lack of Semantic HTML*- Using non-semantic elements or divs without appropriate roles can make it challenging for screen readers to interpret and convey the content's meaning.

      *Fixed or Inflexible Layouts*- If it's used to create fixed-width or inflexible layouts, it can cause issues for users with varying screen sizes or zoom levels. Ensure that your Flexbox layouts adapt to different screen sizes and text zoom settings.

---

### CSS Layout - Flexbox

1. What are some advantages of using flexbox over float?

      Simplified vertical alignment, equal height columns, no need for clearing floats, dynamic sizing and flexibility, content order control, direction-agnostic, automatic equal widths, nested flex containers, better support for modern browswers, maintainability and grid-like layouts.

2. How does this topic connect with your long term goals?

      Flexbox is a great way to order out your pages while building and designing for a client. As my skills grow I am working towards becoming a full stack developer and using flexbox in my css is an important part of designing my pages.

---

### Bookmark and Review

[Learn CSS - Layout](https://web.dev/learn/css/layout/)
---
---

## Things I want to know more about

I want to dive deeper into using Flexbox with CSS Grid.
