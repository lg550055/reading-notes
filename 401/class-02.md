# Testing and Modules
Best practices in software development include test-driven-development and the use of modules.  This summary introduces each concept briefly.

## TDD with Python
> Test-Driven Development, TDD, is a strategy to think and write tests first. -[TDD with Python](https://code.likeagirl.io/in-tests-we-trust-tdd-with-python-af69f47e6932)

TDD facilitates conscious software development by requiring incremental assembly of small pieces that have proven to work.

#### Test best practices
- Test names should be descriptive
- Write a simple test based on common input and output
- The test file name should follow the module name preceded by 'test_'.  E.g. for module 'modulename.py' use 'test_modulename.py'
- Separate tests files and directories from the production code in a mirror structure of test directories and files
- Follow the AAA convention:
  - **Arrange** - get your input
  - **Act** - execute the code
  - **Assert** - check if the output is what was expected

#### TDD Cycle
1. Write a unit test, which will fail because the feature code has yet to be written
2. Write the feature that passes the test
  - Begin with minimal code, not the whole feature
  - Then incrementally add functionality
3. Refactor the code as needed

---

## Modules
> A module is a file containing Python definitions and statements. The file name is the module name with the suffix .py appended. - [If name = main](https://www.geeksforgeeks.org/what-does-the-if-__name__-__main__-do/)

Modules break a program into smaller components which allowing us to keep things:
- simpler
- more maintainable
- reusable

> Python files can act as either reusable modules, or as standalone programs.

The Python interpreter defines a special variable __name__, which takes one of two values:
- __main__ if the program is running directly
- 'modulename' if the program is imported

This allows you flexibility on the programs behavior depending on its use (standalone or imported).

For example, developers use `if __name__ == __main__` to specify behavior when the program is run directly (i.e. not imported as a module).

---

## Bonus - Intro to Recursion
Recursion is the act of a function calling itself.  It is a well-established practice in computer science that allows simple or powerful solutions to specific problems.

Recursion is based on mathematical induction, which proves a statement by ascertaining it is true for the first element and the nth element.

Similarly, in computer science a recursive function has a clearly defined output for what is called the base case and calls itself for all other subsets of the problem.

While recursion is initially harder to comprehend than iterative methods, it is very useful especially in cases where the number or depth of the input is unknown and variable.

[Learn more](https://www.geeksforgeeks.org/recursion/)

---

[Back to table of contents](../README.md)