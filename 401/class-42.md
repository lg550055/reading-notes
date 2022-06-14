# Pythonisms

### Dunder Methods

Dunder Methods are special methods you can use to enrich your classes:

- Initialization of new objects
- Object representation
- Enable iteration
- Operator overloading (comparison)
- Operator overloading (addition)
- Method invocation
- Context manager support (with statement)

### Iterators

> Understanding iterators is a milestone for any serious Pythonista

Iterators work by calling the `__iter__` and `__next__` methods in sequence.

The iteration ends when the last element is reached, in which case the next iteration raises StopIteration.

### Generators

> Generator functions are syntactic sugar for writing objects that support the iterator protocol. Generators abstract away much of the boilerplate code needed when writing class-based iterators.

> Calling a generator function doesn’t even run the function. It merely creates and returns a generator object

Instead of a return statement, generators use a yield statement that suspends the function and retains its local state.

---

### Resources

- [Dunder Methods](https://dbader.org/blog/python-dunder-methods)
- [Iterators](https://dbader.org/blog/python-iterators)
- [Generators](https://dbader.org/blog/python-generators)
- [What are Generators video](https://realpython.com/lessons/what-are-python-generators/)
- [Decorators](https://realpython.com/primer-on-python-decorators/)

---

[Back to table of contents](../README.md)
