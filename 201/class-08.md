# CSS Layout

Basic layout tenets:

- CSS treats each HTML element as its own box
- It is common to group elements inside a `<div>` (or other block-level element)
- The containing element is **always** the direct parent
- Elements in normal flow start on a new line even if they
do not take up the full width

#### Overlapping Elements
A more advanced feature, but one that opens up interesting design opportunities

> When you use relative, fixed, or absolute positioning, boxes can overlap
> Elements that appear later in the HTML code sit on top
- Control which element sits on top with the z-index property
- It's value is a number; the higger the number, the closer the element is to the front

#### Fixed, Liquid and Grid Layouts
> Composition in any visual art is the placement or arrangement of visual elements

- Fixed layouts do not change size with the browser window; which make them unsuitable for applications displayed across different screen sizes
- Liquid layouts stretch and contract with the browser window
  - They tend to use percentages on legth properties
  - To avoid overly long content, use max-width (and min-width for the opposite)
- Grid layouts set consistent proportions and spaces between items
  - help create a professional looking design
  - create continuity between pages
  - help users predict where to find information
  - make it easier to add content in a consistent way

---

[Back to table of contents](../README.md)