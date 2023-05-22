# Class 05: CSS: Cascading Style Sheets

## Design web pages with CSS

---
---
## What is CSS?

- Using CSS, you can control exactly how HTML elements look in the browser, presenting your markup using whatever design you like.
- CSS is a rule-based language — you define the rules by specifying groups of styles that should be applied to particular elements or groups of elements on your web page.
- CSS properties have different allowable values, depending on which property is being specified. In our example, we have the color property, which can take various color values. We also have the font-size property. This property can take various size units as a value.
- As there are so many things that you could style using CSS, the language is broken down into modules.

---

### Great links for reference

[CSS References](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference)
[CSS Tools: Reset CSS](https://meyerweb.com/eric/tools/css/reset/)
[What is CSS?](https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps/What_is_CSS)
[Backgrounds and Borders](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Backgrounds_and_Borders)

---
---

### Answer

1. **What is the purpose of CSS?**

    Using CSS, you can control exactly how HTML elements look in the browser, presenting your markup using whatever design you like.

2. **What are the three ways to insert CSS into your project?**

    - External CSS-With an external style sheet, you can change the look of an entire website by changing just one file
    - Internal CSS-An internal style sheet may be used if one single HTML page has a unique style.The internal style is defined inside the "< style >" element, inside the head section.
    - Inline CSS-An inline style may be used to apply a unique style for a single element.To use inline styles, add the style attribute to the relevant element. The style attribute can contain any CSS property.

3. **Write an example of a CSS rule that would give all < p > elements red text.**

    Example: '< p style="color:red;" >' This is a paragraph.'< /p >'

---

## Using CSS flexbox

[Flexbox Learning](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox)

Flexbox is a one-dimensional layout method for arranging items in rows or columns. Items flex (expand) to fill additional space or shrink to fit into smaller spaces.

### Specifying what elements to lay out as flexible boxes

To start with, we need to select which elements are to be laid out as flexible boxes. To do this, we set a special value of display on the parent element of the elements you want to affect. In this case we want to lay out the < article > elements, so we set this on the < section >:

```md

section {
  display: flex;
}

```

This causes the < section > element to become a flex container and its children to become flex items.

### The flex model

When elements are laid out as flex items, they are laid out along two axes:

- The main axis is the axis running in the direction the flex items are laid out in (for example, as a row across the page, or a column down the page.) The start and end of this axis are called the main start and main end.
- The cross axis is the axis running perpendicular to the direction the flex items are laid out in. The start and end of this axis are called the cross start and cross end.

The parent element that has "display: flex" set on it (the < section > in our example) is called the flex container.
The items laid out as flexible boxes inside the flex container are called flex items (the < article > elements in our example).

### Columns or rows?

Flexbox provides a property called flex-direction that specifies which direction the main axis runs (which direction the flexbox children are laid out in). By default this is set to row, which causes them to be laid out in a row in the direction your browser's default language works in (left to right, in the case of an English browser).
flex-direction: column;

### Wrapping

One issue that arises when you have a fixed width or height in your layout is that eventually your flexbox children will overflow their container, breaking the layout.

### flex-flow shorthand

At this point it's worth noting that a shorthand exists for flex-direction and flex-wrap: flex-flow.

### flex: shorthand versus longhand

*flex is a shorthand property that can specify up to three different values:*

- The unitless proportion value we discussed above. This can be specified separately using the flex-grow longhand property.
- A second unitless proportion value, flex-shrink, which comes into play when the flex items are overflowing their container. This value specifies how much an item will shrink in order to prevent overflow. This is quite an advanced flexbox feature and we won't be covering it any further in this article.
- The minimum size value we discussed above. This can be specified separately using the flex-basis longhand value.
- We'd advise against using the longhand flex properties unless you really have to (for example, to override something previously set). They lead to a lot of extra code being written, and they can be somewhat confusing.

### Flexible sizing of flex items

Let's now return to our first example and look at how we can control what proportion of space flex items take up compared to the other flex items.
First, add the following rule to the bottom of your CSS:

```md

article {
  flex: 1;
}

```

This is a unitless proportion value that dictates how much available space along the main axis each flex item will take up compared to other flex items. In this case, we're giving each < article > element the same value (a value of 1), which means they'll all take up an equal amount of the spare space left after properties like padding and margin have been set. This value is proportionally shared among the flex items: giving each flex item a value of 400000 would have exactly the same effect.
You can also specify a minimum size value within the flex value. Try updating your existing article rules like so:

```md

article {
  flex: 1 200px;
}

article:nth-of-type(3) {
  flex: 2 200px;
}

```

This basically states, "Each flex item will first be given 200px of the available space. After that, the rest of the available space will be shared according to the proportion units."
Horizontal and vertical alignment
You can also use flexbox features to align flex items along the main or cross axis.

```md

div {
  display: flex;
  align-items: center;
  justify-content: space-around;
}

```

centered horizontally and vertically. We've done this via two new properties.

align-items controls where the flex items sit on the cross axis.

By default, the value is *stretch*, which stretches all flex items to fill the parent in the direction of the cross axis. If the parent doesn't have a fixed height in the cross axis direction, then all flex items will become as tall as the tallest flex item. This is how our first example had columns of equal height by default.
The center value that we used in our above code causes the items to maintain their intrinsic dimensions, but be centered along the cross axis. This is why our current example's buttons are centered vertically.
You can also have values like *flex-start* and *flex-end*, which will align all items at the start and end of the cross axis respectively. See align-items for the full details.
You can override the align-items behavior for individual flex items by applying the align-self property to them. For example, try adding the following to your CSS:

```md

button:first-child {
  align-self: flex-end;
}

```

*justify-content* controls where the flex items sit on the main axis.

- The default value is flex-start, which makes all the items sit at the start of the main axis.
- You can use flex-end to make them sit at the end.
center is also a value for justify-content. It'll make the flex items sit in the center of the main axis.
- The value we've used above, space-around, is useful — it distributes all the items evenly along the main axis with a bit of space left at either end.
- There is another value, space-between, which is very similar to space-around except that it doesn't leave any space at either end.
- The justify-items property is ignored in flexbox layouts.

Ordering flex items
Flexbox also has a feature for changing the layout order of flex items without affecting the source order. This is another thing that is impossible to do with traditional layout methods.

```md

button:first-child {
  order: 1;
}

```

- By default, all flex items have an order value of 0.
- Flex items with higher specified order values will appear later in the display order than items with lower order values.
- Flex items with the same order value will appear in their source order. So if you have four items whose order values have been set as 2, 1, 1, and 0 respectively, their display order would be 4th, 2nd, 3rd, then 1st.
- The 3rd item appears after the 2nd because it has the same order value and is after it in the source order.
- You can set negative order values to make items appear earlier than items whose value is 0. For example, you could make the "Blush" button appear at the start of the main axis using the following rule:

```md

button:last-child {
  order: -1;
}

```

### Nested flex boxes

It's possible to create some pretty complex layouts with flexbox. It's perfectly OK to set a flex item to also be a flex container, so that its children are also laid out like flexible boxes.
The HTML for this is fairly simple. We've got a < section > element containing three < article >s. The third < article > contains three < div >s, and the first < div > contains five < button >s:

```md

section - article
          article
          article - div - button
                    div   button
                    div   button
                          button
                          Button

```

First of all, we set the children of the < section > to be laid out as flexible boxes.

```md

section {
  display: flex;
} 

```

Finally, we set some sizing on the button. This time by giving it a flex value of 1 auto. This has a very interesting effect, which you'll see if you try resizing your browser window width. The buttons will take up as much space as they can. As many will fit on a line as is comfortable; beyond that, they'll drop to a new line.
button {
  flex: 1 auto;
  margin: 5px;
  font-size: 18px;
  line-height: 1.5;
}

[CSS tricks for flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

Items will be laid out following either the main axis (from main-start to main-end) or the cross axis (from cross-start to cross-end).

- main axis – The main axis of a flex container is the primary axis along which flex items are laid out. Beware, it is not necessarily horizontal; it depends on the flex-direction property (see below).
- main-start | main-end – The flex items are placed within the container starting from main-start and going to main-end.
- main size – A flex item’s width or height, whichever is in the main dimension, is the item’s main size. The flex item’s main size property is either the ‘width’ or ‘height’ property, whichever is in the main dimension.
- cross axis – The axis perpendicular to the main axis is called the cross axis. Its direction depends on the main axis direction.
- cross-start | cross-end – Flex lines are filled with items and placed into the container starting on the cross-start side of the flex container and going toward the cross-end side.
- cross size – The width or height of a flex item, whichever is in the cross dimension, is the item’s cross size. The cross size property is whichever of ‘width’ or ‘height’ that is in the cross dimension.

## What is grid layout?

A grid is a collection of horizontal and vertical lines creating a pattern against which we can line up our design elements. They help us to create layouts in which our elements won't jump around or change width as we move from page to page, providing greater consistency on our websites.

A grid will typically have columns, rows, and then gaps between each row and column. The gaps are commonly referred to as gutters.
