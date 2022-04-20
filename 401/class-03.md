# FileIO & Exceptions
Reading and writing file data is an essential programming skill because often the program's input or output is data stored in a file.
Similarly, handling exceptions is also a foundational programming skill.  Anticipating and handling potential deviations in a program makes for much better code.

## Reading and writing file data
> At its core, a file is a contiguous set of bytes used to store data.  Modern files have three main parts: header (metadata about the contents), data, and end of file (EOF) marker.

#### Opening and closing files in Python
- Open a file:  `file = open('text_file.txt')`
- The open function takes an optional 2nd argument string to use the file in different ways:
  - Default is 'r' for read only: `open('file.txt', 'r')`
  - Use 'w' for writing: `open('file.txt', 'w')`
  - For binary mode use 'rb' or 'wb' respectively
- Files must be closed after use:  `file.close()`
- To ensure a file is closed even if there is an error:
  - Use a `try` `finally: file.close()` block
  - Use the 'with' context manager - `with open('text_file.txt') as file:` - using 'with' is recommended because it allows for cleaner code

#### Types of files: text, buffered binary or raw binary

- Text files are the most common
- Buffered binary used for reading or writing binary files
- Raw binary are the least common

#### Reading and writing opened files
For reading, here are some methods we can use:
- `.read(size=-1)` -reads based on the *size*; if none or -1, the reads the entire file
- `.readline(size=-1)` -reads *size* chars from the line.  Continues to the end of line and wraps around.  If no argrument or -1, reads entire line (or rest of line)
- `.readlines()` -returns remaining lines as a list

***However, directly iterating over the file object can be quicker and more efficient***

For writing, here are some methods we can use:
- `.write(str)` -writes str to file
- `.writelines(seq)` -writes seq to file withour appending line endings (you must add as appropriate)

To **append** to a file use `open('file.txt', 'a')`

#### Important details when working with files and data

- Representation of line ending, which are often different depending on the operating system used to produce the file
- Paths: absolute or relative
- Character encoding - parsing with the incorrect encoder can lead to failures or misrepresentation of the character.

To **work with two files at the same time**, say one for reading and the other for writing use:
`with open('file1.txt') as reader, open('file2.txt', 'w') as writer`

*Note on Encoding: ASCII (which can store 128 characters) is a subset of Unicode (UTF-8), which can contain up to 1e6 characters.*

##### Remember: there are built-in libaries to help with other formats and situations
For example:
- **wave** for WAV files (audio)
- **zipfile** for ZIP files
- **PyPDF2** toolkit for PDF

---

## Exceptions
> A Python program terminates as soon as it encounters an error. In Python, an error can be a syntax error or an exception.

An exception error occurs when syntactically correct Python code results in an error.

The `try` and `except` block catches and handles exceptions. `Try` executes as part of the program. The code following `except` executes in response to any exceptions in the try clause.

**Try/except blocks are important because they allow our code to react appropriately exception errors.**

Keep in mind:
- The code in the try clause will stop as soon as an exception is encountered
- ***Avoid bare `except` clauses*** because they will hide all errors, which prevents our code form reacting appropriately
- Insted use specific exception classes, e.g.:
  - AssertionError
  - FileNotFoundError
  - ZeroDivisionError

#### Use the `else` clause to run code only if there are no exceptions

#### Use `finally` to always run code after the try | except | else

Use raise to throw an exception at any time.

Use assert to verify a condition is met and throw an error if it is not.

---

### Resources

- [Read & Write Files in Python](https://realpython.com/read-write-files-python/)
- [Read & Write Files video](https://realpython.com/courses/reading-and-writing-files-python/)
- [Read & Write Files in Python Quiz](https://realpython.com/quizzes/read-write-files-python/)
- [Read & Write CSV Files](https://realpython.com/python-csv/)
- [Working with JSON](https://realpython.com/python-json/)
- [Exceptions in Python](https://realpython.com/python-exceptions/)

---

[Back to table of contents](../README.md)
