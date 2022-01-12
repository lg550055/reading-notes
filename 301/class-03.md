# Passing Functions as Props

## Lists and keys
1. What does .map() return?  An array
2. If I want to loop through an array and display each value in JSX, how do I do that in React?  Pass the resulting array from mapping each element into a JSX element
3. Each list item needs a unique **key**
4. What is the purpose of a key?  Help React track which elements have changed, or have been added or removed.

## The spread operator
1. What is the spread operator?  Is syntax to expand an iterable object into the list of arguments
2. List 4 things that the spread operator can do.
  - Spread an array into separate arguments
  - Copy an array
  - Concatenate or combine arrays
  - Add to state in React
3. Give an example of using the spread operator to combine two arrays.  `const helloWorld = {...hello,...world}` where each of hello and world are arrays
4. Give an example of using the spread operator to add a new item to an array.  `const obj3 = {...obj1, newItem}`
5. Give an example of using the spread operator to combine two objects into one.  `const obj3 = {...obj1, ...obj2}`

## How to Pass Functions Between Components
1. In the video, what is the first step that the developer does to pass functions between components?  Creates the function in the state location
2. In your own words, what does the increment function do?  Increments the property counter of the subject person by 1.
3. How can you pass a method from a parent component into a child component?  As a prop
4. How does the child component invoke a method that was passed to it from a parent component?  In this case, inside the onClick as this.increment

---

### Resources

- [React Docs - lists and keys](https://reactjs.org/docs/lists-and-keys.html)
- [The Spread Operator](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)
- [How to Pass Functions Between Components](https://www.youtube.com/watch?v=c05OL7XbwXU)
- [React Tutorial through ‘Declaring a Winner’](https://reactjs.org/tutorial/tutorial.html)
- [React Docs - Lifting State Up](https://reactjs.org/docs/lifting-state-up.html)

---

[Back to table of contents](../README.md)