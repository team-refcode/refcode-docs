# Linking pages in HTML
Links are a vital part of HTML and the very reason why the web exists. In HTML, links are created using the **anchor tag**, `<a>`.

## Why is it called an "anchor" tag?
It's called an *anchor* tag because one end of a link that leads to another document - sort of how an anchor on a boat starts at one point and ends at another. Originally, they weren't designed to link to outside pages; they were meant to jump to locations within a single large document. Today, we use anchor tags as links to other pages, and these tags are more commonly referred to as "A" tags.

## Creating a link

<table>
  <tr>
    <th>steps</th>
    <th><code>html</code></th>
    <th>renders</th>
  </tr>
  <tr>
    <td>Create an empty <em>a</em> tag</td>
    <td><code>&lt;a&gt;&lt;/a&gt;</code></td>
    <td><a></a></td>
  </tr>
  <tr>
    <td>Specify the target in the opening tag</td>
    <td><code>&lt;a href="https://refcode.org"&gt;&lt;/a&gt;</code></td>
    <td><a href="https://refcode.org"></a></td>
  </tr>
  <tr>
    <td>Then add the text that should work as a link</td>
    <td><code>&lt;a href="https://refcode.org"&gt;Link to Refcode&lt;/a&gt;</code></td>
    <td><a href="https://refcode.org">Link to Refcode</a></td>
  </tr>
</table>

Notice that the link does not render in the browser until we add content to the tag.

## Using links as navigation
We use links to go to any page on the web, including our own pages! Navigation menus at the top of websites are just links that take you to pages in the same website.

For instance, a navigation might just be a bunch of links grouped in a `<nav>` tag:

```html
<nav>
  <a href="/index.html">Home</a>
  <a href="/about.html">About</a>
  <a href="/projects/index.html">Projects</a>
  <a href="/links.html">Other Links</a>
</nav>
```

In this example, you see the relative path symbol `/` used; this is shorthand for "use the top level directory for this site." If this site was located at `https://refcode.org`, then the above would be the same as

```html
<nav>
  <a href="https://refcode.org/index.html">Home</a>
  <a href="https://refcode.org/about.html">About</a>
  <a href="https://refcode.org/projects/index.html">Projects</a>
  <a href="https://refcode.org/links.html">Other Links</a>
</nav>
```
