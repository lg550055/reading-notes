# Debugging
The art of finding errors in your code.

- Console and Dev Tools
- Common sources of errors
- Handling errors

### Execution
- Order of execution
- Execution contexts (correspond to variable scope)
  - global context
  - function context

##### Memory stack
> JS processes one line of code at a time.  When a statement need data from another function, it stacks the new function on top of the current task *(which may be stacked on top of a previous one)*

> If a function is called a second time, the variables may have different values

##### Execution context
> Each time a script enters a new execution context, there are two activities:
1. Prepare
  - Create new scope
  - Create variables and functions
  - Determine value of `this`
2. Execute
  - Assign values to variables
  - Reference and run functions
  - Execute statements

> *Each execution context:*
>> - *creates is own ***variables object***, which contains details of all variables and functions*
>> - *has access to its parent's variables object*

### Errors
When there is an error, without error handling code, JS creates and Error object, which can help you find the error.

##### Error object properties:
- name -type of execution
- message - description
- fileNumber -JS file name
- lineNumber -Line of error

##### 7 types of Error objects:
- Error -generic error; base of all other types
- SyntaxError -syntax not followed
- ReferenceError -to variable not declared or within scope
- TypeError -data type can't be coerced
- RangeError -number out of range
- URIError -URI methods used incorrectly
- EvalError -eval() used incorrectly

### Dealing with Errors
- Debug to fix errors
  - Where
    1. Review error message
    2. How far is script running
    3. Use breakpoints
  - What exactly
    1. Evaluate breakpoints
    2. Break down code into smaller parts of functionality
- Handle errors

##### Using the Console
The console is your friend!

- `console.log()` can write several values separated by comma
- `console.table()` outputs a table of objects or arrays
- `console.assert()` tests if a condition is met

##### Beakpoints
Pause code execution to check values at that point

***Set multiple breakpoints to run code step by step***

- Don't forget about conditional breakpoints
- Use keyword 'debugger' in your code to create a breakpoint

### Handling Errors
> Use `try`, `catch` and `finally` if you know your code may fail.

##### Throwing Errors
If you know something may cause a problem, you can generate your own error message with `throw`.

##### Debugging Tips
- Try another browser
- Console.log values; see how far code runs
- Strip code back; down to bare minimum if necessary
- Explain code to a colleague
- Search
- Use a code playground like jsfiddle
- Use online validation tools


---

[Back to table of contents](../README.md)