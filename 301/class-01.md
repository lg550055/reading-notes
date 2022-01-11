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

### Resources

- [Component-Based Architecture](https://www.tutorialspoint.com/software_architecture_design/component_based_architecture.htm)
- [What is Props and How to Use it in React](https://itnext.io/what-is-props-and-how-to-use-it-in-react-da307f500da0#:~:text=%E2%80%9CProps%E2%80%9D%20is%20a%20special%20keyword,way%20from%20parent%20to%20child)
- [React Tutorial through ‘Passing Data Through Props’](https://reactjs.org/tutorial/tutorial.html)
- [React Docs - Hello world](https://reactjs.org/docs/hello-world.html)
- [React Docs - Introducing JSX](https://reactjs.org/docs/introducing-jsx.html)
- [React Docs - Rendering elements](https://reactjs.org/docs/rendering-elements.html)
- [React Docs - Components and props](https://reactjs.org/docs/components-and-props.html)

---

[Back to table of contents](../README.md)