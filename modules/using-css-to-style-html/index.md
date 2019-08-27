---
layout: default
title: Using CSS to Style HTML

parent: Learning Modules
permalink: /modules/using-css-to-style-html
---

# Using CSS to Style HTML
CSS is a language for specifying how documents are presented to users — how they are styled, laid out, etc.

## CSS Rules
Web browsers apply CSS rules to a document to affect how they are displayed. A CSS rule is formed from:

* A **selector**, which selects the element(s) you want to apply the updated property values to. For example, I want to apply my CSS rule to all the paragraphs in my HTML document.
* A set of **properties**, which have values set to update how the HTML content is displayed. For example, I want my element's background to be red.

```css
h1 {
    font-size: 40px;
    background-color: black;
    color: white;
}

h2 {
    font-size: 30px;
    color: darkgray;
}
```

> What are the selectors in the above snippet? 
> What are the properties?


## CSS Stylesheet
A set of CSS rules contained within a **stylesheet** determines how a webpage should look. 

To apply a CSS stylesheet to our webpage, we need to use the `<link>` tag. This is a special tag that defines a link between a document and an external resource. There are two attributes required for the link tag to apply CSS to our page

* `href` - location of the linked document
* `rel` - this will always be "stylesheet" because that's how the file is related

```html
<link rel="stylesheet" href="style.css">
```
