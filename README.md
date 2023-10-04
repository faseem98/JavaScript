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

Then, use the URL to the JavaScript source code file in the src attribute of the <script> element.
The following shows the contents of the app.js file:

app.js file:

    alert('Hello, World!');

And the following script tag content in helloworld.html file:

    <script src="js/app.js"></script>


If you launch the helloworld.html file in the web browser, you will see an alert that displays the Hello, World! message.

# VARIABLE DECLARATION

Variables are used to store reusable values. 

In JavaScript, you can declare variables using three different keywords: 
1. var
2. let
3. const

#### var: 
- var is traditionally used to declare variables.

- It is not commonly used in modern JavaScript.

Scope : Global, Local
       
    var myVar = 10;

#### let: 
- Introduced in ES6 (ECMAScript 2015).

- It allows you to declare variables that can be reassigned. 

Scope : Global, Local, Block

    let myVar = 10;

#### const: 
- Also introduced in ES6, const is used to declare variables that should not be reassigned. 

- It is typically used for constants.

Scope : Global, Local, Block

    const myVar = 10;

#### Naming Variables:
- When declaring variables, it's a good practice to use let or const over var to avoid unexpected behavior. 

- You can declare multiple variables in a single line using commas.

      let x = 5, y = 10, z = 15;
       
- Always choose meaningful variable names to make your code more readable and maintainable.

- There is a list of reserved words, which cannot be used as variable names because they are used by the language itself.
For example: let, class, return, and function are reserved.

- Variable names are case-sensitive, and they can contain letters, digits, underscores, or dollar signs. They must start with a letter, underscore, or dollar sign (not a digit). 

- valid variable names:

      let myVariable;
      let _privateVar;
      let $specialVar;

- invalid variable names:

      let 123abc; // Invalid: starts with a digit
      let my-variable; // Invalid: contains a hyphen

# DATA TYPES

A value in JavaScript is always of a certain type. For example, a string or a number.

We can put any type in a variable. For example, a variable can at one moment be a string and then store a number:

       // no error
       let message = "hello";
       message = 123456;
   
Programming languages where the data types of variables are determined by the value they hold at runtime and can change throughout the program are called “dynamically typed”.

Thus, JavaScript is a dynamically typed language.

There are 8 basic data types in JavaScript.

Seven primitive data types:

- number - for numbers of any kind, integer or floating-point, integers are limited by ±(253-1).
- bigint - for integer numbers of arbitrary length.
- string - for strings. A string may have zero or more characters, there’s no separate single-character type.
- boolean - for true/false.
- null - for unknown values, a standalone type that has a single value null.
- undefined - for unassigned values, a standalone type that has a single value undefined.
- symbol - for unique identifiers.

And one non-primitive data type:

- object - for more complex data structures.

#### typeof operator: 
It allows us to see which type is stored in a variable.
