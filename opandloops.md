# Operators and Loops


## Operators
As you can imagine, an operator conducts and operation among one to three operands.  For example the `+` operator adds two numbers (or concatenates two strings if the operands are strings)

**JS has unary, binary and one special ternary operator**

#### Operator Examples
- Unary: `typeof(operand)` -returns a string indicating the type of the unevaluated operand
- Binary: `*` -returns the multiplication of two operands
- Ternary (there's only one in JS): condition ? val1 : val2 -returns val1 if condition is `true`, otherwise val2

#### Types of Operators
- Assignment - e.g. `=` assigns value of right operand to left operand
- Comparison - e.g. `==` equal, `true` if operands are equal
- Arithmetic - e.g. `*` multiplies
- Bitwise - e.g. `|` bitwise OR
- Logical - e.g. `&&` logical AND
- String - e.g. `+` concatenates two strings
- Conditional (ternary) operator - *see above*
- Comma `,` - evaluates both of its operands and returns the value of the last operand
- Relational - e.g. `in` returns true if the specified property is in the specified object


## Expressions
> An expression is any valid unit of code that resolves to a value.


## Loops
Loops repeat an action some number of times.  There are many kinds of loops, but they all essentially do the same thing.  Here, we focus on `for` and `while` loops

#### `For` loops
For loops repeat until a specified condition evaluates to `false`.  A for loop looks like this:

`for` ([initialExpression]; [conditionExpression]; [incrementExpression]) {
  code that repeats;
}

#### `While` loops
A while loop repeats as long as a its condition evaluates to `true`. A while statement looks as follows:

`while` (condition) {
  code that repeats;
}


For more info, visit [Loops and iteration](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Loops_and_iteration)

---

[Back to home page](index.md)