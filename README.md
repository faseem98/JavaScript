# JAVASCRIPT - INTRODUCTION

JavaScript is a cross-platform, object-oriented scripting language used to add interactivity, functionality and dynamic behavior to websites.

JavaScript was developed by Brendan Eich in 1995. 

Initially, it was created under the name "Mocha" and later renamed to "LiveScript".

Eventually, to leverage the popularity of Java, it was renamed once more to "JavaScript". Despite the name similarity, JavaScript and Java are entirely different programming languages.

# PREREQUISITES TO LEARN JAVASCRIPT

Here are some criteria and prerequisites that can be helpful for learning JavaScript :-
- Basic Understanding of HTML and CSS. 
- Text Editor or Integrated Development Environment (IDE). 
- Web Browser. 

# FEATURES OF JAVASCRIPT

Some of the key features of JavaScript include :-
- Client-Side Scripting: It allows developers to create dynamic and interactive web pages that can respond to user actions without reloading the entire page.
- Cross-Platform: JavaScript is supported by all major web browsers. 
- Dynamic Typing: JavaScript is dynamically typed, meaning that variable types are determined at runtime. 
- Event Handling: JavaScript allows developers to respond to user interactions like clicks, mouse movements and keyboard input. 
- DOM Manipulation: JavaScript can interact with and manipulate the Document Object Model (DOM). 
- Asynchronous Programming: JavaScript supports asynchronous operations through features like callbacks, Promises, and async/await.
- Object-Oriented: JavaScript supports classes and inheritance with the introduction of ES6 (ECMAScript 2015).
- Community and Ecosystem: JavaScript has a vast ecosystem of libraries and frameworks (e.g., React, Angular, Vue.js) for various purposes, from front-end development to server-side scripting (Node.js).

# ADVANTAGES OF JAVASCRIPT

- Speed
- Simplicity
- High performance
- Versatile
- Platform independent
- Object - oriented language

# USES OF JAVASCRIPT

- Web applications
- Mobile applications
- Games development
- Server applications
- Client side validations
- Animate Elements

# YOUR FIRST JAVASCRIPT PROGRAM

Now we can see how to embed JavaScript code into an HTML page.

To insert JavaScript into an HTML page, you use the <script> element. There are two ways to use the <script> element in an HTML page:

- Embed JavaScript code directly into the HTML page.
- Reference an external JavaScript code file.

### Embed JavaScript code in an HTML page:

Placing JavaScript code inside the <script> element directly is not recommended and should be used only for proof of concept or testing purposes.

    <script>alert('Hello, World!')</script>

In the <script> element, we use the alert() function to display the Hello, World! message.

### Include an external JavaScript file:
To include a JavaScript from an external file:

First, create a file whose extension is .js e.g., app.js and place it in the js subfolder. Note that placing the JavaScript file in the js folder is not required however it is a good practice.

Then, use the URL to the JavasScript source code file in the src attribute of the <script> element.
The following shows the contents of the app.js file:

index.js file:

    alert('Hello, World!');

And the following scrit tag content in helloworld.html file:

    <script src="js/index.js"></script>


If you launch the helloworld.html file in the web browser, you will see an alert that displays the Hello, World! message.
