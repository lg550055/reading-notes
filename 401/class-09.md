# Dunder Methods

Dunder Methods are a set of predefined methods that begin and end with double underscores.  They are commonly use to add additional functionality to a class, for example:

- Object initialization
    - __init__ -object constructor
- Object representation
    - __str__  -"nicely printable string representation of an object"
    - __repr__  -official string representation; should be unambiguous
- Enable iteration
    - __len__, __getitem__, __reversed__  -allows specific iteration over a class object
- Operator overloading
    - __eq__, __lt__  -allow comparisons
    - __add__  -defines add (+) operation between class objects
- Method invocation
    - __call__  -makes an object callable (like a function)
- Context manager support
    -__enter__, __exit__ -needed to use the `with`


*Note: operator overloading adds functionality beyond the predefined.*

> *A context manager is a simple “protocol” that allows your object to be used with the `with` statement. Basically, it adds __enter__ and __exit__*

---

### Resources

- [Dunder Methods](https://dbader.org/blog/python-dunder-methods)

---

[Back to table of contents](../README.md)