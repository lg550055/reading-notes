# HTML basics
## Topics covered
1. Wireframe and Design
2. Html basics
3. Semantics

### Wireframe and Design

Wireframing is a high-level process to plan information hierarchy and design

1. Begin with a quick hand-drawn black and white sketch
2. Refine the sketch; focus on **clarity and simplicity**
3. If needed, for collaboration for example, create digital sketchs

Steps to make a wireframe

1. Do your research: understand your audience and requirements
2. Map your user flow: have a clear vision of how the user will interact
3. >Draft, don’t draw. Sketch, don’t illustrate
4. Add detail and begin testing
5. Turn your wireframes into prototypes

Read [this guide](https://careerfoundry.com/en/blog/ux-design/how-to-create-your-first-wireframe/) to learn more


---

### Html basics

Html is the code used to structure a web page and its content.  It consists elements that enclose different portions of content to make it appear or act a certain way.

Elements have four main parts:
1. Opening tag: name of the element wrapped in opening and closing angle brackets
2. Content: content of the element
3. Closing tag: same as the opening tag, except that it includes a forward slash before the element name
4. Element: all three above together

Elements can also have attributes, which contain information that is not part of the content.  They always have the following:

1. Space between it and the element name
2. The attribute name followed by an equal sign
3. he attribute value wrapped by opening and closing quotation marks

*Elements can, and usually appear inside other elements*

Empty elements have no content, e.g. the `<img>` element

#### Markig up text

- Headings use an `<h1>` up to `<h6>` tag
- Paragraphs use a `<p>` tag
- Lists:
  - Unorder (bullet) lists use an `<ul>` tag
  - Ordered (numbered) list usa an `<ol>` tag
  - List elements use a `<li>` tag

#### Links
Links are a very important element since they provide navigation.
To add a link use an `<a href="url">` tag with an `href=""` attribute followed by content and a closing `</a>` tag

---

### Semantics

In programming, Semantics refers to the meaning of a piece of code.  In HTML, for example, the `<h1>` element is a semantic element, which gives the text it wraps the role of "a top level heading on your page."

Benefits of using correct semantic elements:
- Search engines use them to identify important content
- Screen readers use them to help the visually impaired
- Finding content is much easier
- Helps developers understand the type of content data

Here are examples of the close to 100 semantic elements:

- `<article>`
- `<aside>`
- `<footer>`
- `<header>`
- `<nav>`
- `<section>`

Refer to [this documentation](https://developer.mozilla.org/en-US/docs/Web/HTML/Element) for more information

---

[Back to home page](index.md)