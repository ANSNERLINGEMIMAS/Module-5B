# NumPy Program: Column-wise Sorting of a 2D Array

## 🎯 Aim
To write a **NumPy** program that sorts the elements in each column of a given 2D array in ascending order.

## 🧠 Algorithm

1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Accept a 2D NumPy array from the user.
3. **Sort Column-wise**: Use the `np.sort()` function with `axis=0` to sort each column in ascending order.
4. **Store Result**: Store the sorted result in a new array.
5. **Display Output**: Print the original array and the column-wise sorted array.

## 🧾 Program
```
import numpy as np
arr = np.array([[12, 5, 3],
                [4, 8, 6],
                [7, 1, 9]])

sorted_arr = np.sort(arr, axis=0)

print("Original Array:\n", arr)
print("Column-wise Sorted Array:\n", sorted_arr)
```


## Output
```
Original Array:
 [[12  5  3]
  [ 4  8  6]
  [ 7  1  9]]
Column-wise Sorted Array:
 [[ 4  1  3]
  [ 7  5  6]
  [12  8  9]]
```


## Result
The program successfully sorts the elements in each column of the 2D array in ascending order using NumPy’s np.sort() function with axis=0.
