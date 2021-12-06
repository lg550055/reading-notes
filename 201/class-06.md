# Problem Domain, Objects, and the DOM

## Problem Domain
A thorough understanding of the problem domain is an essential first step of efficient programming.  Without this, you can't see what you are trying to buld!

#### Take the time to thoroughly understand the problem domain
- Ask  questions
- Draw the key elements / issues
- Research
- Ask more questions

> You can often make the problem domain easier by cutting out cases and narrowing your focus to a particular part of the problem

***Remember: don't fall into the trap of beginning to code before understanding the problem domain***


---

## Objects

### Primitive values vs Object references
JS has 8 data types: 7 primitve values and `objects`

- Primitive values: boolean, Null, Undefined, Number, BigInt, String, Symbol
- Object references (which include arrays, functions, etc.)

#### Key differences

- Primitive values
    - are immutable
    - assigned variables store them directly
- Objects references
    - are mutable
    - assigned variables contain a reference to them (the memory address where the object is stored)

### Object literals
An object literal is a comma-separated list of name-value pairs inside of curly braces.

Values can be primitives or objects.

There are different way to access the value:
- Square braces `object[name]`
- Dot notation 'object.name`
- Loops

---

## DOM

> The Document Object Model (DOM) is a cross-platform and language-independent interface that treats an XML or HTML document as a tree structure wherein each node is an object representing a part of the document. The DOM represents a document with a logical tree.

> A web page is a document that can be either displayed in the browser window or as the HTML source. In both cases, it is the same document but the Document Object Model (DOM) representation allows it to be manipulated.


---

[Back to table of contents](../README.md)