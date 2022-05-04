# Linear Regression
A Linear Regression is finding a straight line that best approximates a set of data points.  This is commonly done by minimizing the distance between the points and the proposed line.

> One of linear regression's main advantages is the ease of interpreting results.

### How to Run Linear Regression in Python (Scikit-Learn)
> Scikit-learn is a powerful Python module that contains functions for regression, classification, clustering, model selection and dimensionality reduction.

1. `from sklearn.linear_model import LinearRegression`
2. assign to a variable data points from which the line will be calculated
3. create an istance of 'LinearRegression'
4. apply the `fit(x, y)` method to the instance to conduct the regression
5. apply the `predict(x)` method to the instance to make predictions
6. compare / plot predicted vs actual values to see if the linear regression is useful for the dataset (for a quantitative measure use the `score(x, y)` method)

#### Splitting data into train and test sets
To test the validity of our model, in this case a linear regression, we need a set of data points that is separate from the data points used to train the model.  This is called the test set.

When working with a data set that is not already divided into a train set and a test set, we split the original set into these two.  (Although some times we split it in three to include a validation set.)

As a rule of thumb, the split is 80/20 (or 70/30) train set and test set.  (60/20/20 train, validation and test.)

Sklearn, and other libraries, have modules that help us split the data.  In many cases, you can just use a bracket notation to create the splits.

##### Cross Validation

If the dataset is not large enough to allow us a validation set, we can use cross validation.  For cross validation, with divide the train set into k subsets.  We train the model on k-1 subsets and validate it with the kth subset.

### Keep in mind

> Adding independent variables to a linear regression model will always increase the explained variance of the model (typically expressed as R²).  However, overfitting can occur, which reduces model generalizability.  A simple model is preferable to a complex model.  Statistically, if a model includes a large number of variables, some of the variables will be statistically significant due to chance alone.

---

### Resources

- [How to Run Linear Regression in Python](https://bigdata-madesimple.com/how-to-run-linear-regression-in-python-scikit-learn/)
- [Linear regression in python](https://realpython.com/linear-regression-in-python/)
- [Video: Simple Linear Regressions](https://www.youtube.com/watch?v=KsVBBJRb9TE)
- [Train and test sets](https://towardsdatascience.com/train-test-split-and-cross-validation-in-python-80b61beca4b6)
- [What is linear regression](https://www.statisticssolutions.com/free-resources/directory-of-statistical-analyses/what-is-linear-regression/)

---

[Back to table of contents](../README.md)