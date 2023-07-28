# Deep-Learning-Certified-Professional

# 1.0 NumPy, along with their answers and justifications:

### NumPy MCQ Questions

1. What makes NumPy important in the PyData ecosystem?

   a) Provides web development capabilities  
   b) Enables data visualization  
   c) Serves as a foundation for other PyData libraries  
   d) Offers natural language data analysis capabilities  

   **Answer: c**  
   **Justification:** NumPy is an essential building block for other PyData libraries like pandas, scipy, and scikit-learn, providing powerful linear algebra capabilities.

2. How do you import NumPy in Python?

   a) `import pandas as np`  
   b) `import npy as np`  
   c) `import numpy as np`  
   d) `import np`  

   **Answer: c**  
   **Justification:** The standard convention to import NumPy is by using the alias `np`.

3. What is the result of the code snippet?

   ```python
   my_list = [1, 2, 3]
   my_matrix = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
   np.array(my_list)
   ```

   a) `[1, 2, 3]`  
   b) `[[1, 2, 3], [4, 5, 6], [7, 8, 9]]`  
   c) `array([1, 2, 3])`  
   d) `array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])`

   **Answer: c**  
   **Justification:** The `np.array()` function converts `my_list` to a NumPy array, resulting in `array([1, 2, 3])`.

4. Which NumPy function generates evenly spaced values within a given interval?

   a) `np.arange(0, 10)`  
   b) `np.linspace(0, 10, num=10)`  
   c) `np.random.rand(10)`  
   d) `np.zeros(10)`

   **Answer: a**  
   **Justification:** The function `np.arange(0, 10)` generates an array with values from 0 to 9 (inclusive).

5. How do you create an identity matrix using NumPy?

   a) `np.eye(3)`  
   b) `np.identity(3)`  
   c) `np.ones((3, 3))`  
   d) `np.zeros((3, 3))`

   **Answer: a**  
   **Justification:** `np.eye(3)` creates a 3x3 identity matrix with ones on the main diagonal.

6. What does the attribute `arr.shape` represent for a NumPy array `arr`?

   a) The number of dimensions of the array  
   b) The size of the array  
   c) The shape of the array (number of rows and columns)  
   d) The data type of the array  

   **Answer: a**  
   **Justification:** `arr.shape` represents the number of dimensions of the NumPy array `arr`.

7. Which method is used to find the maximum value in the NumPy array `arr`?

   a) `arr.max()`  
   b) `np.max(arr)`  
   c) `np.argmax(arr)`  
   d) `max(arr)`

   **Answer: a**  
   **Justification:** The `max()` method returns the maximum value from the array `arr`.

8. What is the output of the following code snippet?

   ```python
   arr = np.arange(1, 11)
   bool_arr = arr > 4
   arr[bool_arr]
   ```

   a) `[1, 2, 3, 4]`  
   b) `[5, 6, 7, 8, 9, 10]`  
   c) `array([1, 2, 3, 4])`  
   d) `array([5, 6, 7, 8, 9, 10])`

   **Answer: b**  
   **Justification:** The code uses boolean indexing to select elements greater than 4 from the array `arr`.

9. Which NumPy function generates an array of zeros with a specified shape?

   a) `np.zeros(3)`  
   b) `np.zeros((3, 3))`  
   c) `np.ones(3)`  
   d) `np.random.rand(3)`

   **Answer: b**  
   **Justification:** `np.zeros((3, 3))` creates a 3x3 array filled with zeros.

10. What is the purpose of NumPy's `np.random.seed(42)` function?

    a) Generates random integers with a given seed  
    b) Sets the random state for reproducible results  
    c) Seeds the random number generator for improved performance  
    d) Creates random samples from a normal distribution

    **Answer: b**  
    **Justification:** The function `np.random.seed(42)` sets the random seed to produce reproducible random numbers.

11. How can you reshape a NumPy array `arr` to have dimensions (5, 5)?

    a) `arr.reshape(25, 1)`  
    b) `arr.reshape(5, 5)`  
    c) `arr.reshape(1, 25)`  
    d) `arr.reshape(5, -1)`

    **Answer: b**  
    **Justification:** Reshaping `arr` with `arr.reshape(5, 5)` creates a 5x5 array.

12. Which NumPy function returns an array of evenly spaced numbers over a specified interval?

    a) `np.arange()`  
    b) `np.random.randn()`  
    c) `np.zeros()`  
    d) `np.linspace()`

    **Answer: d**  
    **Justification:** The function `np.linspace()` returns an array with evenly spaced values over a specified interval.

13. What is the data type of the NumPy array `arr2 = np.array([1.2, 3.4, 5.6])`?

    a) `int32`  
    b) `int64`  
    c) `float32`  
    d) `float64`

    **Answer: d**  
    **Justification:** The array `arr2` contains floating-point numbers, so its data type is `float64`.



# 2.0 NumPy Indexing and Selection, along with their answers and justifications:


| Question                                                                                                                          | Answer | Justification                                                                                                                              |
|-----------------------------------------------------------------------------------------------------------------------------------|--------|--------------------------------------------------------------------------------------------------------------------------------------------|
| What is the output of `arr[8]` when `arr = np.arange(0,11)`?                                                                      | a) 8  | **Answer: a**<br>**Justification:** The expression `arr[8]` retrieves the element at index 8 in the array `arr`, which is 8.               |
| What is the output of `arr[0:5]` when `arr = np.arange(0,11)`?                                                                    | b) `array([0, 1, 2, 3, 4])` | **Answer: b**<br>**Justification:** The expression `arr[0:5]` selects elements from index 0 to 4 (exclusive) in the array `arr`, resulting in the given output. |
| After executing `arr[0:5]=100`, what will `arr` be when `arr = np.arange(0,11)`?                                                  | d) `array([100, 100, 100, 100, 100, 5, 6, 7, 8, 9, 10])` | **Answer: d**<br>**Justification:** The code sets the values of elements from index 0 to 4 in the array `arr` to 100, while keeping the rest of the elements unchanged. |
| How would you get a copy of the original array `arr` without modifying the original?                                             | a) `arr_copy = arr.copy()` | **Answer: a**<br>**Justification:** The code creates a copy of the array `arr` using the `copy()` method, ensuring that changes made to `arr_copy` will not affect the original `arr`. |
| What is the output of `arr_2d[:2,1:]` when `arr_2d = np.array(([5,10,15],[20,25,30],[35,40,45]))`?                                | c) `array([[10, 15], [25, 30]])` | **Answer: c**<br>**Justification:** The slicing expression selects the top right 2x2 submatrix of `arr_2d`, excluding the first row and all columns except the last two. |
| How do you access the element at row 1, column 0 in the 2D array `arr_2d`?                                                         | b) `arr_2d[1,0]` | **Answer: b**<br>**Justification:** The expression `arr_2d[1,0]` retrieves the element in the first row and first column of the 2D array `arr_2d`, which is 20. |
| What is the output of `arr[arr>4]` when `arr = np.arange(1,11)`?                                                                   | b) `array([5, 6, 7, 8, 9, 10])` | **Answer: b**<br>**Justification:** The expression `arr[arr>4]` selects elements from `arr` that satisfy the condition `arr > 4`, resulting in the given output. |
| What will be the output of `arr[arr>2]` when `arr = np.arange(1,11)`?                                                              | d) `array([3, 4, 5, 6, 7, 8, 9, 10])` | **Answer: d**<br>**Justification:** The expression `arr[arr>2]` selects elements from `arr` that are greater than 2, resulting in the given output. |
| After executing `bool_arr = arr>4`, what is the value of `bool_arr` when `arr = np.arange(1,11)`?                                   | a) `array([False, False, False, False, True, True, True, True, True, True])` | **Answer: a**<br>**Justification:** The code creates a boolean array `bool_arr` by checking which elements in `arr` are greater than 4, resulting in the given output. |
| How would you access elements in `arr` that are greater than 2 and store them in a new array `x`?                                  | c) `x = arr[arr > 2]` | **Answer: c**<br>**Justification:** The expression `arr[arr > 2]` selects elements from `arr` that satisfy the condition `arr > 2` and stores them in the array `x`. |

---

# 3.0 NumPy Operations, along with their answers and justifications:

| Question                                                                                                                                  | Answer | Justification                                                                                                                                                                                                                         |
|-------------------------------------------------------------------------------------------------------------------------------------------|--------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| What will be the output of `arr * arr` when `arr = np.arange(0,10)`?                                                                       | c) `array([ 0,  1,  4,  9, 16, 25, 36, 49, 64, 81])` | **Answer: c**<br>**Justification:** The expression `arr * arr` performs element-wise multiplication of the array `arr` with itself. This results in a new array where each element is the square of the corresponding element in `arr`.        |
| What does the warning message "RuntimeWarning: divide by zero encountered in true_divide" indicate in the expression `arr/arr`?            | b) Division by zero in the array | **Answer: b**<br>**Justification:** The warning message indicates that there is a division by zero in the array `arr`. This results in the array having `nan` (Not a Number) values wherever the division by zero occurs.     |
| What will be the output of `np.exp(arr)` when `arr = np.arange(0,10)`?                                                                     | c) `array([1.00000000e+00, 2.71828183e+00, 7.38905610e+00, 2.00855369e+01, 5.45981500e+01, 1.48413159e+02, 4.03428793e+02, 1.09663316e+03, 2.98095799e+03, 8.10308393e+03])` | **Answer: c**<br>**Justification:** The expression `np.exp(arr)` calculates the exponential (e^) of each element in the array `arr`. This results in a new array where each element is the exponential value of the corresponding element in `arr`. |
| Which NumPy function can be used to calculate the square root of each element in the array `arr` when `arr = np.arange(0,10)`?              | a) `np.sqrt(arr)` | **Answer: a**<br>**Justification:** The function `np.sqrt()` calculates the square root of each element in the array `arr`, as demonstrated in the given example.                                                                          |
| What is the output of `np.sin(arr)` when `arr = np.arange(0,10)`?                                                                          | d) `array([ 0.        ,  0.84147098,  0.90929743,  0.14112001, -0.7568025 , -0.95892427, -0.2794155 ,  0.6569866 ,  0.98935825,  0.41211849])` | **Answer: d**<br>**Justification:** The expression `np.sin(arr)` calculates the sine of each element in the array `arr`. This results in a new array where each element is the sine value of the corresponding element in `arr`.                  |
| What will be the output of `arr_2d.sum(axis=0)` when `arr_2d = np.array([[1,2,3,4],[5,6,7,8],[9,10,11,12]])`?                             | b) `array([15, 18, 21, 24])` | **Answer: b**<br>**Justification:** The expression `arr_2d.sum(axis=0)` calculates the sum of elements along the vertical axis (axis=0) in the 2D array `arr_2d`. This results in a new 1D array with the sum of elements in each column.     |
| What does the expression `arr.min()` return when `arr = np.arange(0,10)`?                                                                  | d) 0                | **Answer: d**<br>**Justification:** The expression `arr.min()` returns the minimum value in the array `arr`, which is 0 in this case, as `arr` starts from 0.                                                                            |
| What will be the output of `arr.mean()` when `arr = np.arange(0,10)`?                                                                      | b) 4.5              | **Answer: b**<br>**Justification:** The expression `arr.mean()` calculates the mean (average) value of the elements in the array `arr`. In this case, the mean of `[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]` is 4.5.                                          |
| What does the expression `arr.var()` return when `arr = np.arange(0,10)`?                                                                   | c) 8.25             | **Answer: c**<br>**Justification:** The expression `arr.var()` returns the variance of the elements in the array `arr`. In this case, the variance of `[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]` is 8.25.                                          |
| What will be the output of `arr_2d.shape` when `arr_2d = np.array([[1,2,3,4],[5,6,7,8],[9,10,11,12]])`?                                   | a) `(3, 4)`         | **Answer: a**<br>**Justification:** The expression `arr_2d.shape` returns the shape of the 2D array `arr_2d`, which is `(3, 4)` as it has 3 rows and 4 columns.                                                                    |

---

# 1.0 Pandas Series, along with their answers and justifications:


| Question                                                                                                                                                    | Answer | Justification                                                                                                                                                                                                                                                                                                                                                         |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------|--------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| What is the primary feature that differentiates a pandas Series from a NumPy array?                                                                        | b) Axis labels for indexing                   | **Answer: b**<br>**Justification:** The primary feature that differentiates a pandas Series from a NumPy array is that a Series can have axis labels for indexing. This allows for indexing by labels, in addition to numerical locations, making it more flexible and versatile for data manipulation.                                                               |
| How would you create a pandas Series from the given data and labels?<br>`data = [10, 20, 30]`<br>`labels = ['a', 'b', 'c']`                               | c) `pd.Series(data=data, index=labels)`      | **Answer: c**<br>**Justification:** To create a pandas Series from the given data and labels, you would use the `pd.Series()` function with the `data` and `index` arguments. The correct syntax would be `pd.Series(data=data, index=labels)`.                                                                                                                          |
| What data type does a pandas Series hold if the data contains different Python objects like strings?                                                       | a) `object`                                   | **Answer: a**<br>**Justification:** A pandas Series can hold a variety of object types, including strings and other Python objects. If the data in a Series contains different Python objects, the data type of the Series will be `object`.                                                                                                                          |
| How can you access the element with the label 'China' from the Series `sales_Q1`?                                                                          | a) `sales_Q1['China']`                       | **Answer: a**<br>**Justification:** To access the element with the label 'China' from the Series `sales_Q1`, you can use the square bracket notation with the label as the index, like `sales_Q1['China']`. This will return the value associated with the label 'China' in the Series.                                                                    |
| What will be the result of `sales_Q1 + sales_Q2`?                                                                                                          | d) Some elements with NaN (Not a Number)     | **Answer: d**<br>**Justification:** When performing operations between two Series, pandas aligns the data based on the index. If there are elements in one Series that do not have a corresponding match in the other Series, the result will be `NaN`. In this case, the result will have some elements with `NaN`.                                                  |
| Which of the following statements is true about indexing in a pandas Series?                                                                              | c) Indexing allows for fast lookups          | **Answer: c**<br>**Justification:** In pandas Series, indexing plays a crucial role. It allows for fast lookups of information, similar to how a hash table or dictionary works. This is because pandas uses the index names or numbers to quickly retrieve data, making data manipulation and access efficient.                                                |
| What will be the output of `pd.Series([sum, print, len])`?                                                                                                 | b) Series holding references to functions    | **Answer: b**<br>**Justification:** A pandas Series can hold various object types, including functions. The expression `pd.Series([sum, print, len])` creates a Series where each element is a reference to a built-in function (`sum`, `print`, `len`). These functions can be accessed and used later in the code. |
| Suppose you have two Series, `ser1` and `ser2`. Which line of code will correctly add the elements of both Series and handle elements with missing matches?    | a) `ser1.add(ser2, fill_value=0)`            | **Answer: a**<br>**Justification:** The `add()` method with `fill_value` parameter can be used to add the elements of both Series while handling missing matches. It will align the Series based on the index and fill any missing values with 0, then perform the addition.                                                                                           |
| What happens if you try to access the element with the label 'Russia' from the Series `sales_Q1` using `sales_Q1['Russia']`?                                | c) KeyError: 'Russia'                        | **Answer: c**<br>**Justification:** If you try to access an element using a label that does not exist in the Series, it will raise a `KeyError`. In this case, trying to access `sales_Q1['Russia']` will raise a `KeyError` because 'Russia' is not a valid label in the given Series.                                              |
| Which of the following data types can a pandas Series hold?                                                                                                | d) All of the above                          | **Answer: d**<br>**Justification:** A pandas Series can hold a wide variety of data types, including numeric data (integers, floats), strings, objects, functions, etc. It can virtually hold any arbitrary Python object, making it a versatile data structure for various types of data.                   |

---
# 2.0 Pandas DataFrame, along with their answers and justifications:

Sure! Here are 10 multiple-choice questions related to pandas DataFrames, along with their answer options and answers with reasons, in Markdown format:

---

### Pandas DataFrames MCQ Questions

1. What are DataFrames in pandas?

   a) DataFrames are inspired by the R programming language.

   b) DataFrames consist of a single column of data.

   c) DataFrames are two-dimensional data structures that share the same index.

   d) DataFrames are one-dimensional arrays.

   **Answer: c**

   **Reason:** DataFrames in pandas are two-dimensional data structures that can be thought of as a bunch of Series objects put together to share the same index.

2. How would you select the 'W' column from the DataFrame `df`?

   a) `df['W']`

   b) `df['column':'W']`

   c) `df['column']['W']`

   d) `df['W']['column']`

   **Answer: a**

   **Reason:** To select the 'W' column from the DataFrame `df`, you can use square bracket notation with the column name, like `df['W']`.

3. What is the result of the code `df.iloc[0:2]`?

   a) Rows with labels 0 and 2

   b) Rows with integer index location 0 and 2

   c) Rows from the 0th row up to (but not including) the 2nd row

   d) Rows with integer index location 0 and 1

   **Answer: d**

   **Reason:** The code `df.iloc[0:2]` will output rows with integer index location 0 and 1 in the DataFrame `df`.

4. What is the data type of the column 'X' in the DataFrame `df`?

   a) int

   b) str

   c) float

   d) bool

   **Answer: a**

   **Reason:** The data type of the column 'X' in the DataFrame `df` is `int32`, which is used to store 32-bit integer values.

5. How would you create a new column 'Total' in the DataFrame `df` that sums the values of columns 'W' and 'Y'?

   a) `df['Total'] = df['W'] + df['Y']`

   b) `df['Total'] = df['W'].sum() + df['Y'].sum()`

   c) `df['Total'] = df['W'].sum(axis=1) + df['Y'].sum(axis=1)`

   d) `df['Total'] = df['W'] + df['Y']`

   **Answer: a**

   **Reason:** To create a new column 'Total' in the DataFrame `df` that sums the values of columns 'W' and 'Y', you can use the expression `df['Total'] = df['W'] + df['Y']`.

6. What is the result of the code `df[df['Z'] > 0]`?

   a) Rows where the value in column 'Z' is greater than 0

   b) Values of column 'Z' where column 'Z' is greater than 0

   c) Rows where the value in column 'Z' is True

   d) Columns where the value in column 'Z' is greater than 0

   **Answer: a**

   **Reason:** The code `df[df['Z'] > 0]` performs conditional selection on the DataFrame `df`. It selects rows where the value in column 'Z' is greater than 0.

7. Suppose you want to remove the row with the label 'E' from the DataFrame `df`. Which code will achieve this without modifying the original DataFrame?

   a) `df.drop('E', inplace=False)`

   b) `df.drop(index='E', inplace=True)`

   c) `df.drop(index='E', inplace=False)`

   d) `df.drop('E', axis=0, inplace=False)`

   **Answer: a**

   **Reason:** The code `df.drop('E', inplace=False)` will remove the row with the label 'E' from the DataFrame `df`. The `inplace=False` argument ensures that the original DataFrame remains unchanged, and the row with the label 'E' is dropped temporarily.

8. How would you select the first three rows and the last two columns of the DataFrame `df` using integer index location?

   a) `df.iloc[:3, -2:]`

   b) `df.iloc[3:, -2:]`

   c) `df.iloc[:2, -3:]`

   d) `df.iloc[3:, :-2`

   **Answer: a**

   **Reason:** To select the first three rows and the last two columns of the DataFrame `df` using integer index location, you can use `df.iloc[:3, -2:]`.

9. What does the `df.describe()` method provide?

   a) Summary statistics on all numerical columns

   b) Number of non-null values in each column

   c) Data types of all columns

   d) Mean and median values of each column

   **Answer: a**

   **Reason:** The `df.describe()` method provides summary statistics on all numerical columns of the DataFrame, including count, mean, standard deviation, minimum, 25th percentile, median (50th percentile), 75th percentile, and maximum values.

10. Which method displays the data type of all columns in the DataFrame?

    a) `df.info()`

    b) `df.dtypes`

    c) `df.describe()`

    d) `df.head()`

    **Answer: b**

    **Reason:** The `df.dtypes` attribute displays the data type of each column in the DataFrame.

# 3.0 Pandas Missing Data, along with their answers and justifications:
Sure! Here are 10 multiple-choice questions related to handling missing data in pandas, along with their answer options and answers with reasons, in Markdown format:

1. What is the purpose of the `dropna()` method in pandas?

   a) It drops rows containing NaN values from the DataFrame.

   b) It drops columns containing NaN values from the DataFrame.

   c) It fills in missing data with a specified value.

   d) It replaces NaN values with the mean of the column.

   **Answer: a**

   **Reason:** The `dropna()` method in pandas is used to drop rows containing NaN (missing) values from the DataFrame.

2. How would you drop columns with missing data from the DataFrame `df`?

   a) `df.dropna()`

   b) `df.dropna(axis=0)`

   c) `df.dropna(axis=1)`

   d) `df.dropna(thresh=2)`

   **Answer: c**

   **Reason:** To drop columns with missing data from the DataFrame `df`, you can use the `df.dropna(axis=1)` method with `axis=1`.

3. What does `thresh` refer to in the `dropna()` method?

   a) It sets a threshold value for the mean of the column.

   b) It determines the number of rows required to drop the column.

   c) It specifies the number of non-NA values required to keep a row.

   d) It fills in missing data with a specified value.

   **Answer: c**

   **Reason:** In the `dropna()` method, `thresh` specifies the number of non-NA values required to keep a row. Rows with fewer non-NA values than the specified threshold will be dropped.

4. How would you fill in missing data in column 'B' of the DataFrame `df` with the value 0?

   a) `df.fillna(0)`

   b) `df['B'].fillna(0)`

   c) `df.fillna(value=0)`

   d) `df['B'].fillna(value=0)`

   **Answer: d**

   **Reason:** To fill in missing data in column 'B' of the DataFrame `df` with the value 0, you can use `df['B'].fillna(value=0)`.

5. Suppose you want to fill in missing data in column 'A' of the DataFrame `df` with the mean of column 'A'. Which code will achieve this?

   a) `df['A'].fillna(df.mean())`

   b) `df['A'].fillna(value=df.mean())`

   c) `df.fillna(df['A'].mean())`

   d) `df.fillna(value=df['A'].mean())`

   **Answer: a**

   **Reason:** The code `df['A'].fillna(df.mean())` will fill in missing data in column 'A' of the DataFrame `df` with the mean of column 'A'.

6. What does the `fillna()` method do when applied to the entire DataFrame without specifying a column?

   a) It replaces NaN values with the mean of the DataFrame.

   b) It fills in missing data with the previous non-missing value.

   c) It fills in missing data with the next non-missing value.

   d) It drops rows with missing data.

   **Answer: a**

   **Reason:** When applied to the entire DataFrame without specifying a column, the `fillna()` method fills in missing data in the DataFrame with the mean of the respective columns.

7. What is the output of the following code: `df.dropna(thresh=2)`?

   a) Rows with at least 2 non-NA values

   b) Rows with less than 2 non-NA values

   c) Columns with at least 2 non-NA values

   d) Columns with less than 2 non-NA values

   **Answer: a**

   **Reason:** The code `df.dropna(thresh=2)` will output rows with at least 2 non-NA values. Rows with fewer than 2 non-NA values will be dropped.

8. Suppose the DataFrame `df` contains a significant amount of missing data in various columns. Which method would be a suitable choice to remove the rows with missing data to ensure the data quality?

   a) `df.dropna()`

   b) `df.dropna(thresh=3)`

   c) `df.fillna(value='FILL VALUE')`

   d) `df.fillna(df.mean())`

   **Answer: b**

   **Reason:** The `df.dropna(thresh=3)` method will remove rows with missing data, but it requires at least 3 non-NA values in each row to keep it. This approach helps retain rows with a sufficient amount of non-missing data, ensuring better data quality.

9. Which method is used to keep missing data in the DataFrame without making any changes?

   a) `df.dropna()`

   b) `df.fillna(value='FILL VALUE')`

   c) `df.fillna(df.mean())`

   d) `df`

   **Answer: d**

   **Reason:** Simply using the DataFrame `df` itself does not modify the original DataFrame. It keeps the missing data as is without making any changes.

10. What is the purpose of the `dropna(axis=1)` method?

    a) It drops columns containing NaN values from the DataFrame.

    b) It fills in missing data with a specified value.

    c) It removes rows containing NaN values from the DataFrame
    
**Answer: a**

**Reason:** The `dropna(axis=1)` method is used to drop columns containing NaN (missing) values from the DataFrame. By specifying `axis=1`, the method operates along columns, removing any column that contains at least one NaN value.

