# React and Forms

## Forms
1. What is a ‘Controlled Component’?  An input form element whose value is controlled by React (instead of having its own value as in normally happens in plain HTML)
2. Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why?  Update state as the user enters the response because the value of the input is always the value stored in state.
3. How do we target what the user is entering if we have an event handler on an input field?  We use a handler for the onChange event.

## The Conditional (Ternary) Operator Explained
1. Why would we use a ternary operator?  To shorten conditional statements, often into 1 line of code.
2. Rewrite the following using a ternary statement:
if(x===y){
  console.log(true);
} else {
  console.log(false);
}

`x===y ? console.log(true) : console.log(false)`

---

### Resources

- [React Docs - Forms](https://reactjs.org/docs/forms.html)
- [The Conditional (Ternary) Operator Explained](https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff)
- [React Bootstrap - Forms](https://react-bootstrap.github.io/components/forms/)
- [React Docs - conditional rendering](https://reactjs.org/docs/conditional-rendering.html)

---

[Back to table of contents](../README.md)