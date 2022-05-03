# Pandas

> A DataFrame is a 2-dimensional data structure that can store data of different types
 Note: NumPy arrays have one dtype for the entire array, while pandas DataFrames have one dtype per column.

 DataFrame.to_numpy() gives a NumPy representation of the underlying data, but is an **expensive operation** when your DataFrame has columns with different data types.

Each column in a DataFrame is a Series.

#### Object creation
- `pd.Series(list of values)` creates a Series with the list of values, with a default integer index
- `pd.DataFrame()` creates a DataFrame from:
  - an array, head labels and row labels
  - a dictionary 

#### Viewing data
- `df.head(n)` displays the table head plus the first 'n' rows
- `df.tail(n)` displays the table head plus the last 'n' rows
- `df.info()` displays a summary of the data
- `df.index` displays the index labels
- `df.columns` displays the columns labels
- `df.describe()` shows a quick statistic summary of the data
- `df.T` transposes the data
- `df.sort_index(axis=1, ascending=False)` sorts the data

#### Getting
- `df['label']` is equivalent to `df.Label` -selects a single column
- `df[ : ]` selects rows by index or label
- `df.loc[ ]` select rows or columns by label
- `df.at[ ]` fast access to a scalar
- `df.iloc[ ]` selects by position

#### Boolean indexing
- `df[ df['A'] > 0 ]` selects possitive values in column A
- `df[df>0]` selects possitive values in data
- `df[slice].isin(filter)` filters data

#### Missing data
> Pandas primarily uses the value np.nan to represent missing data.
- `df.dropna()` drops any rows that have missing data
- `df.fillna(value=?)` fills missing data

### Operations
> Operations in general exclude missing data.

- `df.mean()` returns the mean for each column
- `df.mean(1)` returns the mean for each row

- `df.apply(function)` applies a function to the data

### Getting data in/out
- `df.to_csv(file name)` writtes to csv file
- `pd.read_csv(file name)` reads from csv file

---

### Resources

- [Pandas in 10](https://pandas.pydata.org/pandas-docs/stable/user_guide/10min.html)
- [Pandas getting started](https://pandas.pydata.org/pandas-docs/stable/getting_started/intro_tutorials/index.html)
- [Pandas video](https://www.youtube.com/watch?v=dcqPhpY7tWk&t=391s)
- [Master Pandas](https://towardsdatascience.com/be-a-more-efficient-data-scientist-today-master-pandas-with-this-guide-ea362d27386)

---

[Back to table of contents](../README.md)