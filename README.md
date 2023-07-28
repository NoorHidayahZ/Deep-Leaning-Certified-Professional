# Deep-Leaning-Certified-Professional

# 1.0 NumPy, along with their answers and justifications:

What is NumPy primarily used for in the PyData ecosystem?
a. Image processing
b. Data visualization
c. Linear algebra and numerical operations
d. Text analysis

Answer: c
Justification: NumPy is a powerful library for linear algebra, and many other libraries in the PyData ecosystem rely on it for numerical computations.

Which of the following is a 2D array in NumPy?
a. [1, 2, 3]
b. [[1, 2, 3]]
c. [1, 2], [3, 4]
d. [[1], [2], [3]]

Answer: b
Justification: A 2D array in NumPy is represented as a list of lists.

How can you create an array with values ranging from 0 to 9?
a. np.linspace(0, 9, 10)
b. np.arange(0, 9)
c. np.zeros(10)
d. np.array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9])

Answer: b
Justification: np.arange() generates an array of evenly spaced values within a given interval.

Which method is used to create an identity matrix in NumPy?
a. np.eye()
b. np.ones()
c. np.identity()
d. np.zeros()

Answer: a
Justification: np.eye() is used to create an identity matrix with ones on the diagonal and zeros elsewhere.

What is the output of np.random.rand(3)?
a. [0.33, 0.66, 0.99]
b. [0.234, 0.456, 0.789]
c. [0.045, 0.871, 0.238]
d. [0.224, 0.325, 0.623]

Answer: b
Justification: np.random.rand() generates random samples from a uniform distribution over [0, 1).

How can you find the maximum value in the array arr?
a. arr.max()
b. np.max(arr)
c. max(arr)
d. arr.maximum()

Answer: a
Justification: arr.max() is a method in NumPy to find the maximum value in an array.

What is the shape of the array arr with 25 elements?
a. (5, 5)
b. (25,)
c. (1, 25)
d. (25, 1)

Answer: b
Justification: The shape of a 1D array with 25 elements is (25,).

What is the data type of the array arr2 with values [1.2, 3.4, 5.6]?
a. int32
b. int64
c. float32
d. float64

Answer: d
Justification: The values in the array arr2 are floating-point numbers, and NumPy infers the data type as float64.

Which of the following methods creates an array of zeros?
a. np.zeros(3)
b. np.ones(3)
c. np.arange(3)
d. np.eye(3)

Answer: a
Justification: np.zeros() generates an array of zeros with the specified shape.

What is the output of np.linspace(0, 10, 3)?
a. [0, 5, 10]
b. [0, 2.5, 5, 7.5, 10]
c. [0, 10]
d. [0, 1, 2]

Answer: b
Justification: np.linspace() returns evenly spaced numbers over a specified interval, and the third argument specifies the number of items.

Which method is used to find the index location of the minimum value in an array?
a. arr.min()
b. np.min(arr)
c. min(arr)
d. arr.argmin()

Answer: d
Justification: arr.argmin() returns the index of the minimum value in the array.

How can you set the random seed for reproducibility?
a. np.random.seed(42)
b. np.random.seed()
c. np.seed(42)
d. seed(42)

Answer: a
Justification: np.random.seed() sets the random seed to a specific value, allowing reproducibility of random number generation.

What is the shape of the array arr.reshape(1, 25)?
a. (1, 25)
b. (25, 1)
c. (1, 5)
d. (5, 1)

Answer: a
Justification: The shape of the array after reshaping to (1, 25) will be (1, 25).

How can you create an array with random integers from 1 to 100?
a. np.random.randint(1, 100)
b. np.random.randint(1, 100, 10)
c. np.random.randn(1, 100)
d. np.random.rand(1, 100)

Answer: b
Justification: np.random.randint() generates random integers within a specified range.


How can you set a seed to produce the same random results in NumPy?
a) np.random.seed(42)
b) np.seed(42)
c) np.random.random_state(42)
d) np.random.set_seed(42)
Answer: a
Justification: The np.random.seed() function sets the random state, allowing you to reproduce the same random results.

Which function is used to create an array with a given shape and populate it with random integers?
a) random()
b) rand()
c) randint()
d) randn()
Answer: c
Justification: The randint() function is used to create an array with a given shape and populate it with random integers.

# 2.0 NumPy Indexing and Selection, along with their answers and justifications:

1. What is the output of the following code snippet?
   ```python
   arr = np.arange(0, 11)
   arr[3]
   ```
   a) 0
   b) 1
   c) 2
   d) 3
   Answer: d
   Justification: The code snippet accesses the element at index 3, which is 3.

2. What is the output of the following code snippet?
   ```python
   arr = np.arange(0, 11)
   arr[2:6]
   ```
   a) array([0, 1, 2, 3])
   b) array([2, 3, 4, 5])
   c) array([1, 2, 3, 4])
   d) array([0, 1, 2, 3, 4, 5])
   Answer: b
   Justification: The code snippet selects elements from index 2 to index 5 (excluding index 6).

3. What is the output of the following code snippet?
   ```python
   arr = np.arange(0, 11)
   arr[4:] = 100
   arr
   ```
   a) array([100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100])
   b) array([0, 1, 2, 3, 100, 100, 100, 100, 100, 100, 100])
   c) array([0, 1, 2, 3, 4, 5, 100, 100, 100, 100, 100])
   d) array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
   Answer: b
   Justification: The code snippet sets the elements from index 4 to the end of the array to the value 100.

4. What is the purpose of using `arr.copy()` in NumPy?
   a) It creates a deep copy of the original array.
   b) It creates a shallow copy of the original array.
   c) It creates a view of the original array.
   d) It creates a reference to the original array.
   Answer: a
   Justification: `arr.copy()` creates a deep copy of the original array, ensuring that any changes to the new array do not affect the original array.

5. How do you access the element at row 1 and column 0 in a 2D NumPy array?
   a) arr_2d[1][0]
   b) arr_2d[0][1]
   c) arr_2d[1, 0]
   d) arr_2d[0, 1]
   Answer: c
   Justification: The correct format to access a 2D array element is `arr_2d[row, col]`.

6. What does the following code snippet do?
   ```python
   arr_2d = np.array(([5, 10, 15], [20, 25, 30], [35, 40, 45]))
   arr_2d[:2, 1:]
   ```
   a) It selects the top right corner of the 2D array.
   b) It selects the bottom row of the 2D array.
   c) It selects the elements from the second row onward and from the second column onward.
   d) It selects the elements from the first two rows and from the second column onward.
   Answer: d
   Justification: The code snippet selects the elements from the first two rows and from the second column onward.

7. What is the output of the following code snippet?
   ```python
   arr = np.arange(1, 11)
   arr[arr > 5]
   ```
   a) array([5, 6, 7, 8, 9, 10])
   b) array([6, 7, 8, 9, 10])
   c) array([1, 2, 3, 4, 5, 6])
   d) array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
   Answer: a
   Justification: The code snippet selects elements greater than 5 from the array `arr`.

8. What is the output of the following code snippet?
   ```python
   arr = np.arange(1, 11)
   bool_arr = arr > 2
   arr[bool_arr]
   ```
   a) array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
   b) array([2, 3, 4, 5, 6, 7, 8, 9, 10])
   c) array([3, 4, 5, 6, 7, 8, 9, 10])
   d) array([1, 2])
   Answer: c
   Justification: The code snippet selects elements greater than 2 from the array `arr`.

9. What is the output of the following code snippet?
   ```python
   arr = np.arange(1, 11)
   bool_arr = arr % 2 == 0
   arr[bool_arr]
   ```
   a) array([2, 4, 6, 8, 10])
   b) array([1, 3, 5, 7, 9])
   c) array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
   d) array([1, 3, 5, 7, 9, 10])
   Answer: a
   Justification: The code snippet selects elements that are even from the array `arr`.

10. What does the `bool_arr` variable contain after the execution of the following code snippet?
    ```python
    arr = np.arange(1, 11)
    bool_arr = arr < 5
    ```
    a) array([False, False, False, False,  True,  True,  True,  True,  True,  True])
    b) array([ True,  True,  True,  True, False, False, False, False, False, False])
    c) array([False, False, False, False, False, False, False, False, False, False])
    d) array([ True,  True,  True,  True,  True, False, False, False, False, False])
    Answer: b
    Justification: The `bool_arr` variable contains `True` for elements less than 5 and `False` for elements greater than or equal to 5 in the array `arr`.



# 3.0 NumPy, along with their answers and justifications:
