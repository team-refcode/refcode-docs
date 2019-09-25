---
layout: default
title: Sprint 3
parent: Level 2 Course
nav_order: 4
permalink: /curriculum/level-2/03-sprint-plan
---

# Sprint 3

CSS grid, flexbox, responsive CSS

## Homework Review

- What are media queries? 

- What is flexbox used for?
  - What directions can flexbox items be ordered? 
  - How can flexbox items be spaced? 
  
- What is grid used for? 
  - How is grid different than flexbox?
  
### Exercise: class names 📝

[Matching class names](https://docs.google.com/spreadsheets/d/1jhtMS3pUmA2Pj-Pt8Z_RJ80224rv1IVC1MPSkCryHZQ/edit?usp=sharing) 

1. Create a copy of the google sheet. 
1. Copy class names from the "class list" sheet (bottom) over to the correct element in the "no classes" sheet

### Exercise: flexbox layout 📝

1. Create a "fork" of the CSS [flexbox starter template](https://codepen.io/cocarson-the-lessful/pen/MWgxXya)
1. Fill out the flexbox css properties to create a layout that [looks like this](https://codepen.io/cocarson-the-lessful/full/qBWvKpp)

### Exercise: grid layout 📝

1. Create a "fork" of the CSS [grid starter template](https://codepen.io/cocarson-the-lessful/pen/RwbdJev?editors=1100)
1. Fill out the css grid properties to create a layout that [looks like this](https://codepen.io/cocarson-the-lessful/full/qBWvKpp)

## Let's talk about SASS

Sass is a CSS pre-processor. What is a pre-processor? Well it's code that we can write that is turned into CSS code - kind of like Markdown is turned into HTML! 

Why write Sass instead of css? Sass comes with a few super powers that help us write more maintainable css code. Features like variables, nesting, functions and more make it easier to manage our CSS as the number of styles grows large.

### 1. Install SASS

Navigate to https://sass-lang.com/install to install Sass on your computer. Looks for the **command line** instructions for Mac or Windows.

### 2. Running SASS

Sass is run using the command line. Run Sass by giving it an input `.scss` file and an`.css` file to create.

Example:

```
sass source/stylesheets/index.scss build/stylesheets/index.css
```

### Experimenting with Sass

In class experiments with Sass variables and nesting.



---
<< [Back to curriculum overview](../level-2)
