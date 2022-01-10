# Introduction to React and Components
> Components are like JavaScript functions. They accept arbitrary inputs (called “props”) and return React elements describing what should appear on the screen -*reactjs.org*

## Component-Based Architecture
1. What is a “component”?  A, usually brief, reusable, self-contained piece of code with specific functionality.
2. What are the characteristics of a component?
  - Reusability.  Keep code DRY
  - Replaceable by other components
  - Context agnostic.  Self-contained, with specific functionality independent of context.
  - Extensible.  Can build upon other components.
  - Encapsulated.  Self-contained.
  - Independent.  Minimal dependencies on other components.
3. What are the advantages of using component-based architecture?
  - Ease of deployment.  Replace old with new without impacting system
  - Reduced cost.  Leverage third-party components
  - Reusable.
  - Manage technical complexity.  Isolate functionality.
  - Reliability.  The reliability of each individual component enhances the reliability of the whole system.
  
## Props
1. What is “props” short for?  Properties.
2. How are props used in React?  Pass data from one component to another.
2. What is the flow of props?  Uni-directional; one-way from parent to child.

***Prop data is read-only; a child should not modify data coming from its parent component***

---

[Back to table of contents](../README.md)