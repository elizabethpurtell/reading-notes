# Class 13 - Introduction to Persistence with Local Storage

## Statement

Comprehending both local storage and server-side operations empowers you as a developer to create robust, efficient, and secure web applications while providing a seamless and secure user experience. It also allows you to make informed decisions about where and how to store and manage data based on the specific requirements of your projects.

---
---

### Local Storage and How To Use It On Websites

1. Why would a developer use local storage for a web application?

    Developers use local storage in web applications because it allows them to store small amounts of data on a user's device, like a computer or smartphone. This data stays even after the user closes the web page or browser, which is handy for saving preferences, user settings, or temporary information, such as a shopping cart in an online store. Local storage is simple to use with JavaScript, and it helps improve the user experience by remembering things without needing to fetch data from a server every time, making the web app faster and more responsive.

2. What information should not be stored in local storage?

    Sensitive or private information, such as passwords, credit card details, or personal identification data, should not be stored in local storage. Local storage is not secure and is accessible by JavaScript running on the same webpage, which means it can be vulnerable to malicious scripts or attacks. Instead, sensitive data should be securely handled on the server-side using encryption and proper security measures. Storing such information in local storage could expose it to potential risks, compromising the user's privacy and security.

3. Local storage can store what type of data? How would you convert it to that type before storing?

    Local storage can store data in the form of strings. This means that before storing other data types like numbers or objects, you need to convert them to strings. You can do this using JavaScript's built-in functions like JSON.stringify () for objects or simply using string concatenation for numbers. For example, to store a number as a string in local storage, you can do something like localStorage.setItem ( 'myNumber', '42'), where '42' is a string representation of the number 42. When you retrieve the data from local storage, you can convert it back to its original type using parseInt () or parseFloat () for numbers or JSON.parse ()` for objects. This way, you can work with various data types while storing and retrieving them from local storage as strings.

---

### Bookmark and Review

[“The Past, Present, and Future of Local Storage for Web Applications”](http://diveinto.html5doctor.com/storage.html)

---
---

## Things I want to know more about

I am interested in eventually creating my own servers to store my pages. I want to find out what all is involved in doing this.
