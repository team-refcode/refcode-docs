---
layout: default
title: Using Classes in CSS

parent: Learning Modules
permalink: /modules/using-class-css-selectors
---

# Using Classes in CSS
CSS is the way we style HTML on the web. A CSS stylesheet is a list of CSS rules that apply to our HTML document. A CSS rule is composed of a **selector** and a set of **properties**. The selector tells us what to target and the properties are the styles we apply to *all* elements that match the selector.

We already know how we can use HTML tag names as selectors, such as the following:

```css
div {
    display: block;
}

p {
    color: #EEE;
}
```

The above will apply `display:block` to *all* `div` elements on the page and style all `p` elements with `color: #EEE`. But what if we did not want to make every `div` display as a block or every `p` to be a light grey? Instead of a selector that would target *all* elements on a page, we need a more **specific** selector.

## How to use Class and ID selectors
We can also define our own selectors in the form of class and ID selectors. The benefit of this is that you can have the same HTML element, but style it differently depending on the class or ID.

In the CSS, a class selector is a name preceded by a period `.` and an ID selector is a name preceded by a hash character `#`.

Just like when we use a HTML tag as a selector, our styles will not be applied if the corresponding element is not on the page. In our HTML page, we can add the `class` attribute to the beginning of any tag such as:
```html
<div class="homepage article">
</div>
```

or

```html
<p>This is an example of some text that will have <a href="/about.html" class="internal-link">a link</a> contained inside it.</p>
```

### Example

```css
#main-container {
    display: block;
}

.intro {
    color: #EEE;
}
```

```html
<div id="main-container">
  <h1>Hello</h1>
  <p class="intro">Greetings!</p>

  <p>This is some other content</p>
</div>

```

## Differences between Class and ID selectors
The difference between an ID and a class is that an ID can be used to identify one element, whereas a class can be used to identify more than one.

With classes you can also have more than on class on an element, but you cannot have more than one ID.

This is OK:
```html
<div class="container article large-text">
</div>
```

This is not OK:
```html
<div id="container article large-text">
</div>
```

We can write a selector to target one or multiple classes! Let's take the following example:

```html
<article class="short large-text">
</article>

<article class="short">
</article>

<article class="long small-text">
</article>
```

We could create rules that target elements in many different ways:

```css
article {
    color: #333;
}

.short {
    border-bottom: 1px solid #666;
}

.large-text {
    font-size: 150%;
}

.small-text {
    font-size: 80%;
}

.short.large-text {
    color: #EEE;
    border-bottom: 4px solid #999;
}
```
