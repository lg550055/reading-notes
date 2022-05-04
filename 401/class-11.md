# Numpy

> NumPy, developed in the mid 2000s, arose from an older package called Numeric. Thus, almost every data analysis or machine learning package for Python leverages NumPy in some way.

Numpy makes is simple and efficient to work with datasets.  Things that would need other libraries and several lines of code can be done with a single Numpy function.  Furthrermore, Numpy array are highly optimized to be fast.

> In a NumPy array, the number of dimensions is called the rank, and each dimension is called an axis.

In a matrix, the rows are the first axis, and the columns are the second axis.  The shape method returns a tuple with the number of rows and columns.

*Note: For much faster runtime performance, use Numpy instead of plain Python for numerical array calculations.  See link to Numpy array programming at the bottom.*

#### np.random.rand(x,y)
> Creating arrays full of random numbers can be useful when you want to quickly test your code with sample arrays.

For example, `np.random.rand(3,4)` returns an numpy array with 3 rows and 4 columns of random numbers in the range (0,1)

#### np.genfromtxt(x,y)
The 'genfromtxt' function generates a numpy array from a file.  The function can take a number of arguments to help us clean the data.

#### Slicing numpy arrays
Just like with regular lists, use square bracket notation to access parts of the numpy array to read, assign or overwritte array values.

#### NumPy Data Types
A numpy array can only have one data type.  The most common types are: 'int', 'float', 'string' and 'object'.

Use the `astype(dtype)` method to convert the array to the desired data type.

#### NumPy Array Operations
> NumPy makes it simple to perform mathematical operations on arrays.

> ***Single Array Math***
If you do any of the basic mathematical operations (/, *, -, +, ^) with an array and a value, it will apply the operation to each of the elements in the array.

***Multiple Array Math***
Similarly, you can (/, *, -, +, ^) each element of array1 by each element of array2 for arrays of the same size.

For arrays of different size, Numpy performs 'broadcasting' to try to match up elements.  Generally, Numpy is able to do this when the length of one dimension in array A matches the length of one dimension in array B (or one array has a dimiension with lenght one).

#### NumPy Array Methods
Use the '.sum(slice)' method to add all selected elements
Similarly, use the 'mean', 'std', 'min' and 'max' methods.
Find all array methods [here](https://numpy.org/doc/stable/reference/arrays.ndarray.html)


#### NumPy Array Comparisons
Similar to Single Array Math, Numpy can perform comparison operations (<, >, >=, <=, and ==) on each element.  This allows us to create subsets of our data, among other things.

#### Combine NumPy Arrays
Combine (compatible) arrays vertically or horizontally with the 'vstack' or 'hstack' function.

---

## Bonus: Jupyter shortcuts

'Esc' takes you to command mode.

Command mode shortcuts:
 - H -help
 - A or B -insert cell above or below
 - M or Y -change cell to Markdown or code
 - D D -(d twice) delete current cell
 - ctrl + shift + - -split cell from cursor location

---

### Resources

- [NumPy Tutorial](https://www.dataquest.io/blog/numpy-tutorial-python/)
- [NumPy Quickstart](https://numpy.org/doc/stable/user/quickstart.html)
- [Python NumPy Tutorial](https://cs231n.github.io/python-numpy-tutorial/#numpy)
- [Visual NumPy Introduction](https://github.com/rougier/numpy-tutorial)
- [NumPy Tutorials](https://www.tutorialspoint.com/numpy/index.htm)
- [Numpy array programming](https://realpython.com/numpy-array-programming/)

---

[Back to table of contents](../README.md)