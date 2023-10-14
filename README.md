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

# BROWSER SPECIFIC FUNCTIONS

Let's see 3 browser-specific functions to interact with the users,

1. alert
- shows a message.
2. prompt
- shows a message asking the user to input text. It returns the text or, if Cancel button or Esc is clicked, null.
3. confirm
- shows a message and waits for the user to press “OK” or “Cancel”. It returns true for OK and false for Cancel/Esc.

All these methods are modal - they pause script execution and don’t allow the visitor to interact with the rest of the page until the window has been dismissed.

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

# STRINGS & TEMPLATE LITERALS

- A string is a sequence of one or more characters that may consist of letters, numbers, or symbols.
  
- JavaScript template literals allows you to work with a string template more easily.

- Before ES6, you use single quotes (') or double quotes (") to wrap a string literal.
 
- ES6 template literals provide the syntax that allows you to work with strings more safely and cleanly.
 
- In ES6, you create a template literal by wrapping your text in backticks (`)
 
#### Variable Substitutions

- Template literals allow variables in strings.
  
- Automatic replacing of variables with real values is called string interpolation.

  **Syntax**: ${variable_name}
    
See the following example:

    let firstName = 'John',
    lastName = 'Doe';

    let greeting = `Hi ${firstName}, ${lastName}`;
    console.log(greeting); // Hi John, Doe
    
#### Getting the length of the string
- The length property returns the length of a string.

        let str = "Good Morning!";
        console.log(str.length);  // 13

#### Accessing characters
- To access the characters in a string, you use the array-like [] notation with the zero-based index. 

        let str = "Hello";
        console.log(str[0]); // "H"

- To access the last character of the string, you use the length - 1 index.

        let str = "Hello";
        console.log(str[str.length -1]); // "o"

#### Concatenating strings via + operator
- To concatenate two or more strings, you use the + operator.

        let name = 'John';
        let str = 'Hello ' + name;
        console.log(str); // "Hello John"

# OPERATORS

JavaScript has a variety of operators that allow you to perform different operations on values. 

Here are some of the most common types of operators in JavaScript:

1. **Arithmetic Operators**: These operators perform basic mathematical operations.
   - Addition: `+`
   - Subtraction: `-`
   - Multiplication: `*`
   - Division: `/`
   - Modulus (Remainder): `%`

3. **Assignment Operators**: Used to assign values to variables.
   - Assignment: `=`
   - Addition Assignment: `+=`
   - Subtraction Assignment: `-=`
   - Multiplication Assignment: `*=`
   - Division Assignment: `/=`

4. **Comparison Operators**: Used to compare values and return a Boolean result.
   - Equal to: `==`
   - Not equal to: `!=`
   - Strict equal to: `===`
   - Strict not equal to: `!==`
   - Greater than: `>`
   - Less than: `<`
   - Greater than or equal to: `>=`
   - Less than or equal to: `<=`

5. **Logical Operators**: Used to perform logical operations on Boolean values.
   - Logical AND: `&&`
   - Logical OR: `||`
   - Logical NOT: `!`

6. **Unary Operators**: Operate on a single operand.
   - Increment: `++`
   - Decrement: `--`
   - Unary plus: `+`
   - Unary minus: `-`
   - Typeof: `typeof`
   - Delete: `delete`

7. **Ternary (Conditional) Operator**: A shorthand for an `if-else` statement.
   - Example: `condition ? expression1 : expression2`

8. **Bitwise Operators**: Perform bitwise operations on integers.
   - Bitwise AND: `&`
   - Bitwise OR: `|`
   - Bitwise XOR: `^`
   - Bitwise NOT: `~`
   - Left shift: `<<`
   - Right shift: `>>`
   - Zero-fill right shift: `>>>`

9. **Other Operators**:
   - Comma Operator: `,` (Used to separate expressions, evaluating them from left to right and returning the rightmost value)
   - Conditional (Ternary) Operator: `? :` (Used for conditional expressions)
   - instanceof (Used to test if an object is an instance of a particular class)
   - in (Used to check if an object has a certain property)

These operators are essential for performing different operations and controlling the flow of your JavaScript code.

# CONDITIONAL BRANCHING

- Sometimes, we need to perform different actions based on different conditions.

- We can use the if...else statement, the conditional operator (?) and the switch statement for conditional branching.

## The if...else statement :
- The if...else statement executes a statement if a specified condition is truthy.
- If the condition is falsy, another statement in the optional else clause will be executed.

**Syntax**:

    if (condition)
    statement1

    // With an else clause
    if (condition)
      statement1
    else
      statement2

#### The Nested if...else statement :
- Multiple if...else statements can be nested to create an else if clause. 

**Syntax**:

    if (condition1)
      statement1
    else if (condition2)
      statement2
    else if (condition3)
      statement3
    // …
    else
      statementN

## Conditional (ternary) operator : 
- The conditional (ternary) operator is the only JavaScript operator that takes three operands: a condition followed by a question mark (?), then an expression to execute if the condition is truthy followed by a colon (:), and finally the expression to execute if the condition is falsy.
- This operator is frequently used as an alternative to an if...else statement.

**Syntax**:

     condition ? exprIfTrue : exprIfFalse

#### Conditional chains :
The ternary operator is right-associative which means it can be "chained" similar to an if … else if … else if … else chain.

**Syntax**:

    function example() {
      return condition1 ? value1
        : condition2 ? value2
        : condition3 ? value3
        : value4;
    }

## The switch statement : 
- The switch statement evaluates an expression matching the expression's value against a series of case clauses and executes statements after the first case clause with a matching value until a break statement is encountered.
- The default clause of a switch statement will be jumped to if no case matches the expression's value.

**Syntax**:

    switch (expression) {
      case value1:
        statements
      case value2:
        statements
      // …
      case valueN:
        statements
      default:
        statements
    }

# LOOPS

- Loops are used in JavaScript to perform repeated tasks based on a condition.
- There are four types of loops in JavaScript.
 1. for loop
 2. while loop
 3. do-while loop
 4. for-in loop

## for loop : 
- The JavaScript for loop iterates the elements for the fixed number of times.
- It should be used if number of iteration is known.

**Syntax**:

    for (initialization; condition; increment)  
    {  
        code to be executed  
    }  

## while loop : 
- The JavaScript while loop iterates the elements for the infinite number of times.
- It should be used if number of iteration is not known.

**Syntax**:

    while (condition)  
    {  
        code to be executed  
    }  

## do-while loop : 
- The JavaScript do while loop iterates the elements for the infinite number of times like while loop.
- The code is executed at least once whether condition is true or false.

**Syntax**:

    do{  
        code to be executed  
    }while (condition);  

## for-in loop : 
- The JavaScript for in loop is used to iterate the properties of an object.

**Syntax**:

    for (variable in object)
    {  
         code to be executed  
    } 

# ARRAYS

- An array is a type of data structure where you can store an ordered list of elements.

- Array elements are numbered, starting with zero.

## Declaration of an Array : 
There are basically two ways to declare an array.

1. Creating an array using array literal:

        let arrayName = [value1, value2, ...];

2. Creating an array using the JavaScript new keyword:

        let arrayName = new Array();

## Accessing array elements :
- We can get an element by its index in square brackets.

        let fruits = ["Apple", "Orange", "Plum"];
        alert( fruits[0] ); // Apple
        alert( fruits[1] ); // Orange
        alert( fruits[2] ); // Plum
  
- We can replace an element in an array.

       fruits[2] = 'Pear'; // now ["Apple", "Orange", "Pear"]
  
- We can add a new element to the array.

       fruits[3] = 'Lemon'; // now ["Apple", "Orange", "Pear", "Lemon"]
  
- The total count of the elements in the array is its length:

       let fruits = ["Apple", "Orange", "Plum"];
       alert( fruits.length ); // 3

## JavaScript Array Methods :
Let's see the list of important JavaScript array methods,

- concat() : It returns a new array object that contains two or more merged arrays.
- every() : It determines whether all the elements of an array are satisfying the provided function conditions.
- filter() : It returns the new array containing the elements that pass the provided function conditions.
- find() : It returns the value of the first element in the given array that satisfies the specified condition.
- forEach(): It invokes the provided function once for each element of an array.
- includes() : It checks whether the given array contains the specified element.
- indexOf() : It searches the specified element in the given array and returns the index of the first match.
- map() : It calls the specified function for every array element and returns the new array
- pop() : It removes and returns the last element of an array.
- push() : It adds one or more elements to the end of an array.
- reverse() : It reverses the elements of given array.
- reduce(function, initial) :It executes a provided function for each value from left to right and reduces the array to a single value.
- some() : It determines if any element of the array passes the test of the implemented function.
- shift() : It removes and returns the first element of an array.
- slice() : It returns a new array containing the copy of the part of the given array.
- sort() : It returns the element of the given array in a sorted order.
- splice() : It add/remove elements to/from the given array.
- unshift() : It adds one or more elements in the beginning of the given array.

## Deep Dive into Map, filter and reduce array methods :
- Map, filter and reduce are three of the most useful and powerful high-order array methods.

**Map method**:
- The map() method is used for creating a new array from an existing one, applying a function to each one of the elements of the first array.

**Syntax**:

    var new_array = arr.map(function callback(element, index, array) {
        // Return value for new_array
    }[, thisArg])

**Example**:

    const numbers = [1, 2, 3, 4];
    const doubled = numbers.map(item => item * 2);
    console.log(doubled); // [2, 4, 6, 8]

**Filter method**:
- The filter() method takes each element in an array and it applies a conditional statement against it.
- If this conditional returns true, the element gets pushed to the output array.
- If the condition returns false, the element does not get pushed to the output array.

**Syntax**:

    var new_array = arr.filter(function callback(element, index, array) {
        // Return true or false
    }[, thisArg])

**Example**:

    const numbers = [1, 2, 3, 4];
    const evens = numbers.filter(item => item % 2 === 0);
    console.log(evens); // [2, 4]

**Reduce method**:
- The reduce() method reduces an array of values down to just one value.
- To get the output value, it runs a reducer function on each element of the array.

**Syntax**:

    arr.reduce(callback[, initialValue])

**Example**:

    const numbers = [1, 2, 3, 4];
    const sum = numbers.reduce(function (result, item) {
      return result + item;
    }, 0);
    console.log(sum); // 10

# FUNCTIONS

- In JavaScript, a function is a reusable block of code that performs a specific task or set of tasks. 
- Functions are fundamental building blocks in JavaScript.
- They allow you to encapsulate logic, organize your code and make it more modular and maintainable.

**Syntax**:

    function functionName(parameters) {
      // Code to be executed
      return result; // Optional
    }

**function**: The keyword used to declare a function.

**functionName**: The name of the function (can be any valid identifier).

**parameters**: Optional input values that the function can accept.

**{}**: A pair of curly braces that enclose the code block to be executed when the function is called.

**return**: An optional keyword used to specify the value that the function should return. If omitted, the function returns undefined.

- Here's an example of a simple function,
  
        function add(a, b) {
          return a + b;
        } 

- You can call this function by providing arguments,

        const result = add(3, 4); // result will be 7

- Functions can also be assigned to variables, passed as arguments to other functions, and returned from other functions. 

## Function Declaration ways :
- In JavaScript, you can declare functions using several methods:-
  
1. Function Declaration:
   
        function myFunction() {
          // Function code here
        }

2. Function Expression:
        
        const myFunction = function() {
          // Function code here
        };

3. Arrow Function (ES6):

        const myFunction = () => {
          // Function code here
        };

4. Function Constructor (not recommended):

        const myFunction = new Function('arg1', 'arg2', 'return arg1 + arg2;');

- Function Declarations and Expressions are the most common and recommended ways to declare functions in JavaScript. 
- Arrow functions are especially useful for concise, inline functions. 
- Function Constructor should be avoided unless you have specific reasons to use it.

## Types of Functions :
1. Named function
2. Anonymous function
3. Immediately invoked function expression

#### **Named Function**:
- Named function is the function that we define it in the code and then call it whenever we need it.

**Example**:

    function oddOrEven(number){
     if(number%2 == 0) {
      return "Even number"
     } else {
      return "Odd number"
     }
    }

#### **Anonymous Function**:
- The anonymous functions don’t have names.
- They need to be tied to something: variable or an event to run.

**Example**:

    let oddOrEven = function(number){
         if(number%2 == 0) {
          return "Even number"
         } else {
          return "Odd number"
         }
    }

#### **Immediately invoked function expression**:
- Invoked function expression runs as soon as the browser encounters it.

**Example**:

    // Regular Function. 
        function Greet() { 
            console.log("Welcome to JavaScript!"); 
        }; 
    // Execution of Regular Function. 
        Greet(); 
  
    // IIFE creation and execution. 
    (function() { 
        console.log("Welcome to JavaScript!");  
    })(); 

**Output**:

    Welcome to JavaScript!
    Welcome to JavaScript!

# ARROW FUNCTIONS

- Arrow functions were introduced in ES6.
  
- Arrow functions allow us to write shorter function syntax.

**Syntax**:
    
    const functionName = (arg1, arg2, ?..) => {  
        //body of the function  
    }  

- There are three parts in an Arrow Function,

1. **Parameters**: Any function may optionally have the parameters.
2. **Fat arrow notation**: It is the notation for the arrow (=>).
3. **Statements**: It represents the instruction set of the function.

- Some arrow functions have parentheses around the parameters and others don't.
  
        //Example with parentheses
        const addNums = (num1, num2) => num1 + num2;
        
        //Example without parentheses
        const addTwo = num => num + 2;
  
- The number of parameters an arrow function has determines whether or not we need to include parentheses.

- An arrow function with zero parameters requires parentheses.
 
        const hello = () => "hello";
        console.log(hello());
        //Result: "hello"

- An arrow function with one parameter does not require parentheses. In other words, parentheses are optional.

        const addTwo = num => num + 2;

- An arrow function with multiple parameters requires parentheses.

        const addNums = (num1, num2) => num1 + num2;
        console.log(addNums(1, 2));
        //Result: 3

# OBJECTS

- A JavaScript object is a collection of named values.

- It is a common practice to declare objects with the const keyword.

**Example**:

    const person = {firstName:"John", lastName:"Doe", age:50, eyeColor:"blue"};

## Creating Objects :

- There are different ways to create new objects,
  
1. **using an Object literal** : The simplest way to create an object is by using object literals, which allow you to define key-value pairs within curly braces.

        var person = {
          firstName: "John",
          lastName: "Doe",
          age: 30,
        };

2. **using the JavaScript Keyword new** :  You can create a new JavaScript object using new Object(), and then add properties.

        const person = new Object();
        person.firstName = "John";
        person.lastName = "Doe";
        person.age = 50;
   
3. **using Constructor Function** : You can create objects by defining constructor functions and then using the new keyword to instantiate objects from them.

        function Person(firstName, lastName, age) {
          this.firstName = firstName;
          this.lastName = lastName;
          this.age = age;
        }
        
        var person = new Person("John", "Doe", 30);

4. **using Object.create()** : You can create an object based on a prototype using the Object.create() method. This method creates a new object with the specified prototype object.

        class Person {
          constructor(firstName, lastName, age) {
            this.firstName = firstName;
            this.lastName = lastName;
            this.age = age;
          }
        }
        
        var person = new Person("John", "Doe", 30);

## Objects and properties :

- A JavaScript object has properties associated with it.
  
- The properties of an object define the characteristics of the object.

        const myCar = {
          make: "Ford",
          model: "Mustang",
          year: 1969,
        };
        
## Accessing properties :

- We can access a property of an object by its property name.

- Property accessors come in two syntaxes: dot notation and bracket notation.

        // Dot notation
        myCar.make = "Ford";
        myCar.model = "Mustang";
        myCar.year = 1969;
        
        // Bracket notation
        myCar["make"] = "Ford";
        myCar["model"] = "Mustang";
        myCar["year"] = 1969;

## Modifying properties :

- We can change the values of object properties by assigning new values.

        person.age = 31; // Modify the 'age' property
        person['lastName'] = 'Smith'; // Modify the 'lastName' property

## Adding properties :

- We can add new properties to an object at any time.

        person.city = 'New York'; // Add a new 'city' property

## Deleting properties :

- We can remove properties from an object using the delete keyword.

        delete person.city; // Remove the 'city' property

## Object Methods : 

- Object Methods are functions that are defined as properties of an object.
  
- The functions can be called to perform specific actions or operations on the object or its data.

**Example**:

        const person = {
          firstName: 'John',
          lastName: 'Doe',
          fullName: function() {
            return this.firstName + ' ' + this.lastName;
          }
        };
        
        console.log(person.fullName()); // Outputs: "John Doe"

   In the example above, the fullName property of the person object is a method. When called using person.fullName(), it returns the full name of the person by concatenating the firstName and lastName properties.

- Object methods are often used for a variety of purposes, including:
  
1. Modifying object properties.
2. Calculating and returning values based on object properties.
3. Interacting with the object's state or data.
4. Performing actions related to the object.

   Here's another example that demonstrates a method used to modify an object's property:

        const counter = {
          count: 0,
          increment: function() {
            this.count++;
          },
          reset: function() {
            this.count = 0;
          }
        };
        
        counter.increment(); // Increment the count property
        console.log(counter.count); // Outputs: 1
        
        counter.reset(); // Reset the count property
        console.log(counter.count); // Outputs: 0





