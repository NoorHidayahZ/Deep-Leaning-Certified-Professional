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

Sure! Here are 10 multiple-choice questions related to NumPy indexing and selection along with their answers and justifications in Markdown format:

---

### NumPy Indexing and Selection MCQ Questions

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


