# List Comprehensions

List Comprehension is one of Python's most distinctive features.  It allows you to create powerful functionality within a single line of code!

> List comprehensions make it easy to create lists while performing sophisticated filtering, mapping, and conditional logic on their members.

> List comprehensions are also more declarative than loops.  Loops require you to focus on how the list is created. You have to create an empty list, loop over the elements, and add each of them to the end of the list. With a list comprehension in Python, you can instead focus on what you want to go in the list

### Replace a `for` loop with a single line
Replacing a `for` loop with, is perhaps the most common case of list comprehension.  Instead of:

`my_list = []`
`For i in iterable:`
  `my_list.append(i)`

You may use:

`my_list = [i for i in iterable]`

### List Comprehensions for mapping and filtering

Add conditional logic to create and filter a list using list comprehension, e.g.:

`my_filtered_list = [i for i in iterable if i > 10]`

For mapping, perform the operation on each element you want to add to the list, e.g.:

`my_mapped_list = [i**3 for i in iterable]`

Create, map and filter!

`my_filtered_list = [i/3 for i in iterable if i > 10]`

### Set and Dictionary Comprehensions
While list comprehension is most common, you can also use comprehensions to creat sets and dictionaries.

To create a set, which avoids duplicates, use curly braces; e.g.:

`sentence = 'some text with repreated letters`
`unique_letters = {l for l in sentence}`

To create a dictionary, you need to provide for a key, e.g.:

`squares_dictionary = {i: i**2 for i in range(7)}`

### Comprehensions are not always the best option

*Warning:  some developers overuse list comprehensions; leading to less efficient and harder to read code.*

- Watch out for nested comprehensions
- Use generators for large datasets
- For pure computations, for loops might be faster

### Summary
In summary, comprehensions are:
- Simple
- Powerful
- Clean

---

### Resources

- [List Comprehensions](https://realpython.com/list-comprehension-python/)
- [Comprehensions examples](https://www.pythonforbeginners.com/basics/list-comprehensions-in-python)
-[pythonpodcast](https://www.pythonpodcast.com/pysnooper-python-debugging-episode-241/)
- [Decorators primer](https://realpython.com/primer-on-python-decorators/)

---

[Back to table of contents](../README.md)