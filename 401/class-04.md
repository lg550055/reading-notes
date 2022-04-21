# Classes, Objects and Pytest Fixtures and Coverage

## Classes and Objects overview
> Objects are an encapsulation of variables and functions into a single entity. Objects get their variables and functions from classes. Classes are essentially a template to create your objects.

Use dot notation to access class variables and functions.

> The __init__() function, is a special function that is called when the class is being initiated. It's used for asigning values in a class.

---

## Thinking Recursively
Break problems into small, easily solved pieces.

A recursive function calls on itself to repeat some action until a condition is met, at which time the whole problem is solved.  This condition is called the base case.

Keep in mind that each recursive call has its own execution context.  This may require you to pass accumulators or declare global variables.

---

## Pytest Fixtures and Coverage
Pytest is a library for testing Python code.

#### Fixtures
> In testing, a fixture provides a defined, reliable and consistent context for the tests.

Fixtures are decorators that allow us to pass functions into tests as data and modify their behavior as needed.

> Tests don’t have to be limited to a single fixture. They can depend on many fixtures; and fixtures can use other fixtures.  (But beware of compounding errors.  Keep it as simple as possible.)

Fixtures have explicit names and are activated by declaring their use from test functions, modules, classes

#### Coverage
To help you make sure you are testing all your code, there is a Pytest library called *pytest-cov*.  When properly configured, it looks to test parts of your code that othrewise would go untested.

*NOTE on Fixtures and Coverage: These are initial statemets that are in all likelihood incomplete / incorrect need to be polished.*

---

### Resources

- [Classes and Objects](https://www.learnpython.org/en/Classes_and_Objects)
- [Thinking recursively](https://realpython.com/python-thinking-recursively/)
- [Pytest Fixtures and Coverage](https://www.linuxjournal.com/content/python-testing-pytest-fixtures-and-coverage)
- [Fixtures](https://docs.pytest.org/en/latest/explanation/fixtures.html)

---

[Back to table of contents](../README.md)