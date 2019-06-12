# Introduction to CSS Layout

CSS page layout techniques allow us to take elements contained in a web page and control where they are positioned relative to their default position in normal layout flow, the other elements around them, their parent container, or the main viewport/window.

## Normal Flow
Normal flow is how the browser lays out HTML pages by default when you do nothing to control page layout. Everything in normal flow has a value of `display` that determines how they behave in the flow.

Most elements, such as `<p>` and `<div>` use `display: block`, which mean they display below one another and don't overlap. However, some elements like `<a>` use `display: inline`, which means it remains inline with the rest of the text, and doesn’t break onto a new line.


### Floats
Applying a float value such as left can cause block level elements to wrap alongside one side of an element, like the way images sometimes have text floating around them in magazine layouts.

The `float` property has four possible values:

* `left` — Floats the element to the left.
* `right` — Floats the element to the right.
* `none` — Specifies no floating at all. This is the default value.

### Position
The `position` property allows you to precisely control the placement of boxes inside other boxes. `static` positioning is the default in normal flow, but you can cause elements to be laid out differently using other values; for example, you could use `fixed` to have an element always stick to the top left of the browser viewport.

