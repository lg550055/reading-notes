# HTML Links, JS Functions, and Intro to CSS Layout + Pair Programming

Lets begin with Pair Programing

## Pair Programming
> Iterative loops. Code reviews. Fast feedback. Error checking and linting. These are software engineering practices that have proven to dramatically improve the quality of code developers produce. What if you can could get all of this, instantaneously, while typing code line by line and character by character? You can, with pair programming, a technique common to many agile work environments.
*Code Fellows*

- Two developers share a signle workstation
- There's a Driver and a Navigator
  - The Driver has the keyboard: types code and does version control
  - The Navigator verbally guides the Driver, thinks about the big picture, scans for typos or bugs, and may use a second computer to research

**Pair Programming is more efficent.**  While it takes a little longer to complete a task, the quality is better and there's less of a need to debug later.  ***Pairs find solutions faster and get unstuck faster.***


---

## HTML Links
Links are the core of web navigation

- Between or within pages
- To other sites
- Email links

#### Anatomy of links
`<a href="http://www.imdb.com">IMDB</a>`
Opening tag with destination attribute (href), followed by text shown to user, followed by closing tag

Link references (href attribute value) can be absolute or relative:
- Absolute: full url to destination
- Relative: path to file of own page
  - same folder: `<a href="reviews.html">Reviews</a>`
  - child folder: `<a href="music/listings.html">Listings</a>`
  - parent folder: `<a href="../index.html">Home</a>`
  - grand parent folder: `<a href="../../index.html">Home</a>`


---

## JS Functions
Functions are fundamental in JS; take input, followed by steps to calculate an output.

- Functions have to be declared by the keyword `function`
- Take the form `function functionName(parameters){code}`
  - Functions with no name are 'anonymous' functions
  - Functions can take 0 or more parameters
- Have to be 'called' to execute
- Functions can be assigned to a variable, which makes them 'function expressions'


---

## Intro to CSS Layout
Layout is about where is element sits on a page with the objective of creating attractive pages

- Each element is its own box
  - Block elements start on a new line, e.g. h1, p, ul
  - Inline elements flow between sorrounding text, e.g. img

An element's positioning depends on its `position` property:
- Normal (default): block elements begin on a new line just below the previous element
- Relative: does not affect the possition of sorrounding elements but shifts the element to, for example the bottom, of where it would have appeared in Normal
- Absolute: element is taken out of normal flow and appears on a particluar place on its containing element
- Fixed: a case of Absolute, places the element in a particular spot of the browser window (think floating header)
- Float: element taken out of the Normal flow and position to the far right or left of its containg element; around which other content can flow


---

[Back to table of contents](../README.md)