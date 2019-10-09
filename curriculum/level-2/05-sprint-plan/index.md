---
layout: default
title: Sprint 5
parent: Level 2 Course
nav_order: 6
permalink: /curriculum/level-2/05-sprint-plan
---

# Sprint 5
Command line Git, JavaScript variables

## JavaScript

1. JavaScript is the most popular programming language in the world
1. Started out as a language to make websites interactive, now capable of building entire applications
   - What is the difference between a website and a web application? 
1. High average salary for JavaScript developer
1. JavaScript runs on browsers or outside of browsers with Node.js
1. Two versions of JavaScript -> ES6 and ES5

### Running JavaScript in the browser

JavaScript can be run in the browser by typing in the console. Right click and select "Insepct" to open the developer tools. Select the "Console" tab from the developer tools to open the JavaScript console. This is an interactive area where you can type JavaScript code to be executed by the browser.

 - Open up the console, type `console.log('hello world');` and press enter
 - Try adding two numbers together `2 + 2`
 
 ### Running JavaScript from and HTML page
 
 Using the `<script>` tag
 
 1. In an HTML file, add a `<script>` tag to the bottom of the body element. 
 1. Trying typing the `console.log('hello world');` code from earlier. 
 1. Open the page in your browser and open the console. You should see the same `hello world` message printed in the console.
 
 Using a separate JavaScript file
 
 1. Create new file called `main.js` in your project folder
 1. Copy the `console.log('hello world');` code from the `<script>` tag into the new `main.js` file
 1. Replace the `<script>` tag and the code inside with `<script src="./main.js"></script>`
 1. Reload the page to see if `hello world` still prints in the console.
 
### JavaScript programming fundamentals

#### Variables
 
Variables are used to store a value for later use. To create a variable, use a special keyword to "declare" that you want a variable, then the name of the variable. To assign the variable to a "value" use an `=` sign followed by the value.

Keywords:
 - `let` -> declares a variable whose value will later change
 - `const` -> declares a variable whose value will never change (it's "constant")
 - `var` -> Old ES5 variable declaration
 
Variable name constraints:
 - Cannot be a reserved word (let, const, if, for, ...)
 - Should be meaningful
 - Cannot start with a number
 - Cannot contain a space or hyphen
 - Case sensitive
 
#### Types

There are a numebr of "Types" in JavaScript. Each "Type" uses a different syntax. 

They are:
 - `String` -> a set of characters surrounded by quotes
   - Example: `'Hello world'`
 - `Number` -> an integer or decimal number
   - Example: `12` or `1.2`
 - `Boolean` -> a true or false value
   - Example: `true` or `false` 
 - `null` -> a special value the represents and empty or unknown value
 - `undefined` -> when a value has not been assigned
 - `Object` -> a special type that store a collection of value
   - `{ name: 'Carson', height: 176' }`
   

---
<< [Back to curriculum overview](../level-2)
