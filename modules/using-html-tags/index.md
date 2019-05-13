# Using HTML Tags
How we build HTML pages is based off the history of how the web was first imagined and implemented. In the beginning, the web was developed to be a sharing place for scientific documentation. It was expanded to share news articles and blog posts. While the uses of the web has expanded drastically from the early days, the underlying principles and structure remain largely intact. The tags available in HTML reflect the history of the web as a way to create documents.

## What is a Tag?
Let's look at the following tag:

```html
<h1>Welcome to my Website!</h1>
```

This can be broken up into "tag name" and "tag contents". The tag name is "h1" - meaning heading 1, and the content is "Welcome to my Website!". We, and the browser, know how to parse out the content by looking at the opening `<>` and closing `</>` tags, then rendering that as a `h1`.

## Basic Tags for writing HTML content

Tag	| Semantic Meaning
----|-----------------
`<h1> - <h6>` | Headings
`<p>` | Paragraph
`<b>` | A keyword or term (not bold!)
`<ul>` | Unordered List
`<ol>` | Ordered List
`<li>` | List Item (must be nested inside a `<ul>` or `<ol>`!)
`<span>` | Inline-level element intentionally without semantic meaning
`<a>` | Link
`<img>` | Image

## Container Tags for grouping elements

Tag	| Semantic Meaning
----|-----------------
`<main>` | The top-level main content (only one pre page)
`<nav>` | Navigation
`<article>` | Container that makes sense on its own
`<section>` | Generic document or application section
`<header>` | Header of the document or section
`<aside>` | Ordered List
`<footer>` | Footer of the document or section
`<div>` | Container element intentionally without semantic meaning


## Attributes
Let's look at a tag that is slightly different than the `h1` example above:

```html
<img src="/flower.png" />
```

There are a couple of things going on here with the `img` tag. First, there's not a opening tag, content, then a closing tag - so there's no content here!

Secondly, there is additional information next to the tag name (`src="/flower.png"`). This is called an **tag attribute**, or just attribute for short. Remember, it's not content because it's not in between the opening `<>` and closing `</>` tags. Attributes are special. They allow us to add additional information to a tag that isn't rendered to the page. In this case, we want to render an image, not the path to the image.

Lastly, this is a *self-closing* tag. While that may sound complicated, it just means there isn't any content to this tag. So, instead of doing something like this:

```html
<img src="/flower.png"></img>
```

we just combine the open and closing tags to make it

```html
<img src="/flower.png" />
```

Most tags will have content, so we don't run into this situation too often. However, all images will work like this so it's good to know.

## Exercise
Take a newspaper and dissect the different sections. Draw attention to the similarities in a newspaper to a news website. Further dive into the content to identify the following HTML elements:

* `body`
* `header`
* `<h1> - <h5>`
* `<img>`
* `<a>`
* `<nav>`
* `<article>`
* `<section>`
* `<header>`
* `<aside>`
* `<footer>`
