# Class 12 - Chart.js, Canvas

## Statement

This set of readings leads us into using the < canvas > element which opens a big window into building more interesting and dynamic pages. The canvas element allows us to use chart.js, which is a way to display data in visually appealing charts, graphs and more.

---
---

### JavaScript Canvas

1. What does the < canvas > allow a developer to acheive?

    The HTML < canvas > element is a powerful tool for developers that allows them to achieve dynamic and interactive graphics and animations within a web page. It provides a blank slate where developers can use JavaScript to draw shapes, images, text, and animations directly onto the web page.

2. What is the importance of the closing </ canvas > tag?

    To create valid HTML documents, all elements must be properly opened and closed. This helps browsers and parsers understand the hierarchy and nesting of elements within the page. The closing < /canvas > tag indicates the end of the < canvas > element's content, ensuring that the browser knows where the canvas ends. This structure adheres to HTML standards and best practices, ensuring consistent rendering and behavior across different web browsers. In complex web pages, HTML elements are often nested within each other. The proper opening and closing of elements, including the < canvas> element, ensure that nesting issues don't occur. When using JavaScript to interact with the < canvas> element, closing the tag is essential. JavaScript can reference the < canvas> element using its unique identifier or by querying the DOM (Document Object Model). The closing tag helps ensure that the JavaScript code operates within the expected context and can manipulate the canvas as intended.

3. Explain what the getContext() method does.

    The getContext() method in HTML5's < canvas> element is used to obtain a rendering context for the canvas. It returns an object that provides a set of methods and properties for drawing and manipulating graphics on the canvas. The argument you pass to getContext () determines the type of rendering context you want; '2d' is the most common for 2D graphics. Once you have the context, you can use its methods like fillRect (), drawImage (), and fillText () to draw shapes, images, and text on the canvas. Essentially, getContext () is the gateway to creating dynamic and interactive graphics in web applications.

---

### Chart.js Documentation

1. What is Chart.js and how it can be brought into your project?

    Chart.js is a popular JavaScript library for creating interactive and visually appealing charts and graphs on web pages. It simplifies the process of data visualization and offers various chart types, including bar charts, line charts, pie charts, and more.

    Chart.js is like a magic tool for making cool charts on websites. To use it in your project, you first need to tell your project where to find Chart.js. You can either download it from the Chart.js website or use a special link called a "CDN" to include it in your project. Next, you create a place on your webpage where you want the chart to appear using a < canvas > element. You give this canvas a special name, like "myChart." Then, in your code, you tell Chart.js to use that canvas to draw your chart. You can customize how your chart looks and what data it shows. That's it! Chart.js makes it easy to turn data into pretty charts for your website without too much hassle.

2. List 3 different Chart types you can create using Chart.js.

    Bar Chart: A bar chart is used to display data in rectangular bars with lengths proportional to the values they represent. It's great for comparing data across categories. For example, you can use a bar chart to show sales figures for different products.

    Line Chart: A line chart is ideal for showing trends over time. It connects data points with lines, making it easy to visualize changes in data. Line charts are often used for displaying stock prices, temperature trends, or other time-series data.

    Pie Chart: A pie chart represents data in a circular graph, where each "slice" of the pie represents a proportion of the whole. Pie charts are useful for showing the composition of a whole, such as the distribution of expenses in a budget or the market share of different products.

    These are just a few examples, and Chart.js offers even more chart types, including radar charts, polar area charts, and scatter plots, to cater to various data visualization needs.

---

### Easily Create Stunning Animated Charts with Chart.js

1. What are some advantages to displaying data via a chart over a table?

    Displaying data via a chart is often more advantageous than using a table because charts make it easier to see trends and patterns at a glance. In a chart, data is presented visually, using shapes and colors to represent information. This visual representation helps our brains quickly grasp the significance of the data, making it easier to understand complex information. Tables, on the other hand, present data in rows and columns, which can be less intuitive and require more effort to analyze. Charts are especially useful when you want to show comparisons, trends over time, or the relative proportions of different data points, making data more accessible and engaging for your audience.

2. How could Chart.js aid your previously created applications visually?

    In our application of the sales data from salmon-cookie we could use that data to build out a chart of the cookie sales from each store.

---

### Bookmark and Review

[Drawing Shapes with Canvas](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes)

[Applying Style and Colors - Canvas API](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors)

[Drawing Text - Canvas API](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_text)

[Download chart.js on GitHub](https://github.com/chartjs/Chart.js)

---
---

## Things I want to know more about

I want to dive deeper into the animated charts, they look really cool.

[Radar Charts](https://www.chartjs.org/docs/latest/charts/radar.html)
