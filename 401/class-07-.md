# Python Scope

## Scope
Scope determines the visibility of a name in the code.  A name is only accesible by the code in its scope.

- A name is an identifier of a variable, function, class or other object that can be assigned (or defined) a name.
- The assignment location is the scope.  For example, a name assigned inside a function has local scope, and a name assigned at the top level of a module has global scope.

> Python **scopes are implemented as dictionaries** that map names to objects.  These dictionaries are commonly called **namespaces**.  Stored in the special attribute __dict__.

Use scope it to minimize bugs related to name collision.

#### LEGB - Local, Enclosing, Global, Built-in scopes

> Whenever you use a name, Python searches through different scope levels (or namespaces) to determine whether the name exists or not. If the name exists, then you’ll always get the first occurrence of it.

- **Local** -only visible within the block of a function
  - created when the function is called (and destroyed when the function returns)
- **Enclosing** -for nested functions, the names of the encolsing function are visible to the inner function
  - names defined in the enclosing scope are know as `nonlocal`
  - created when the outer function is called
  - the inner function can read (but not assign) names in the enclosing scope that are created prior to the inner function being called
  - if you want to modify a name in the enclosing space from the inner function, use the `nonlocal` keyword prior to the assignment.
- **Global** -visible everywhere in the module
  - created the moment you start a program
  - there is only one global scope per program execution
  - names are available to all parts of the code
  - assign global names from a local scope by preceding the assignment with the `global` keyword.  However, this is considered **bad practice** because it is:
    - difficult to debug
    - hard to understand
    - impossible to reuse
- **Built-in** -a special scope created when running a script or an interactive session, it contains built-in keywords, functions, etc...

***Note:  Keep in mide that using `global` and `nonlocal` modifies standard behavior.***

#### Best practices

- Write self-contained functions that rely on local names
- Use uniqe object names regardles of the scope
- Use global names as constants / avoid global name modification
- Avoid cross-module modification
- Don't override the built-in names

---

### Resources

- [Python Scope](https://realpython.com/python-scope-legb-rule/)
- [More of Big O](https://www.youtube.com/watch?v=5Uqawfl0VHQ)

---

[Back to table of contents](../README.md)