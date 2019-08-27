---
layout: default
title: Structuring HTML Pages

parent: Learning Modules
permalink: /modules/structuring-html-pages
---

# Structuring HTML Pages
Before we get started writing HTML, it's important to understand its basic structure. Just like any other language, if you don't use the right words or put them in the right order, it won't make any sense! In most cases, the browser will try to figure out the right formatting, but we should try our best to format it correctly ourselves.

## Background
HTML stands for **H**yper**t**ext **M**arkup **L**anguage. It's the standard markup used for creating web pages. It was based off of an older markup language, SGML, which was originally designed to enable the sharing of machine-readable large-project documents in government, law, and industry. This the origin for where all the specific rules for how a HTML page should be written.

## Basic Template
Below is the basic HTML that we will be using in this program. You can copy this snippet when building out new pages.

```html
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">

  <title>Site Name</title>
  <meta name="description" content="Page Name">
  <meta name="author" content="Your Name">
</head>
<body>
    Content goes here...
</body>
</html>
```

So what does all this mean?

## The Doctype
First, we have the Document Type Declaration, or doctype. This is simply a way to tell the browser what type of document it’s looking at. In the case of HTML files, it means the specific version and flavor of HTML.

## The `html` Element
We’ve included the lang attribute with a value of en, which specifies that the document is in English.

## The `head` Element
The first line inside the head is the one that defines the character encoding for the document. In nearly all cases, `utf-8` is the value you’ll be using in your documents. A full explanation of character encoding is beyond the scope of this program.

Next, we have some meta data that's used by the browser to help display your page. This information is also used to find your site in searches.

## The `body` Element
The body element represents the main content of the document.


