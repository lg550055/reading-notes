# In memory storage

## Understanding the JavaScript Call Stack

1. What is a ‘call’?  A function invocation.
2. How many ‘calls’ can happen at once?  One.
3. What does LIFO mean?  Last in, first out.
4. Give an example of a call stack and the functions that would need to be invoked to generate that call stack.  A data structure with calls stacked on top of one another.  The first call is at the bottom of the stack, then the second...  However, the processing happens from top to bottom.  Thus the last call to be brought into the stack is the processed first.
5. What causes a Stack Overflow?  When the number of calls exceeds the capacity of the stack.  A common cause is a recursive program calling itself too many times.

## JavaScript error messages

1. What is a ‘refrence error’?  Variable not declared or within scope
2. What is a ‘syntax error’?  Syntax not followed
3. What is a ‘range error’?  Number out of range
4. What is a ‘tyep error’?  Data type can't be coerced
5. What is a breakpoint?  Pause code execution to check values at that point
6. What does the word ‘debugger’ do in your code?  Creates a breakpoint

--- 

### Resources

- [Understanding the JavaScript Call Stack](https://medium.freecodecamp.org/understanding-the-javascript-call-stack-861e41ae61d4)
- [JavaScript error messages](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)

---

[Back to table of contents](../README.md)