# Using JavaScript with HTML

JavaScript is a programming language that is used to change a website after the site has **rendered**. JavaScript is most often used to *respond to user actions*. This is called making a site **interactive**. Besides responding user action, JavaScript can also create and modify the DOM (HTML elements).

Let's review the three primary programming languages that are used to build websites:

 - HTML: the **content** of the page
 - CSS: **styles** the content
 - JavaScript: interaction and DOM updates
 
## JavaScript Examples

Using JavaScript to show different prices based on slider value.

https://mailchimp.com/pricing/calculator/standard/

![JavaScript slider example](./js-example-mc.gif)

### ❓ Question ❓

Can someone find another example of JavaScript on a site they regulary use?

## Add JavaScript to an HTML page

Remember how there are multiple ways to add CSS to an HTML page? (hint: using the `<style>` tag or linking an `.css` file) Adding JavaScript is done in a similiar way, but with a few key differences.

### 1. The `<script>` tag

The `<script>` tag is a special HTML tag which is used to writing script languages inside of an HTML file. When writing JavaScript inside of a `<script>` tag, we should specify that the script is written in the JavaScript language.

Here's an example:

```html
<script type="text/javascript">

 // JavaScript code goes here
 
</script>
```

#### ❓ Where does the `<script>` tag go? ❓

What are the options? 

The `<script>` tag can be placed anywhere in either the `<head>` or the `<body>` of the HTML document. However, there is a difference between them!

What happens happen if the `<script>` tag is placed in the `<head>` of the document? Consider a really long JavaScript file (5 million lines of code).

✅ `<script>` tags should be located at the end of the `<body>`

### 2. External script

Alternatively we can link to a JavaScript file using the `src` attribute on the script tag. JavaScript file always end with the `.js` file extension.

Example: 

```html

<script src="./my-first-javascript.js"></script>

```

##  💃 Exercise! 🕺

In your web project do the following:

1. Create a new JavaScript file called: `main.js`
1. Add the following code to `main.js`: `alert("Hello world!");`
1. Add a `<script>` tag to your `index.html` page with the **src** attribute set to the new JavaScript file path

Example:

`index.html`

```html
<!DOCTYPE html>
<html>

<head>
	<title>My HTML page</title>
	<meta charset="UTF-8" />
</head>

<body>
 <h1>This is my page</h1>
 
 <script src="./main.js"></script>
</body>

</html>
```

`main.js`

```js
alert("Hello world!");
```
