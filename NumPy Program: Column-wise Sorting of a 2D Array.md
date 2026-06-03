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
rows = int(input("Enter number of rows: "))
cols = int(input("Enter number of columns: "))
print("Enter array elements:")
arr = np.array([[int(input()) for j in range(cols)] for i in range(rows)])

sorted_arr = np.sort(arr, axis=0)
print("Original Array:")
print(arr)
print("Column-wise Sorted Array:")
print(sorted_arr)
```

## Output
<img width="1361" height="605" alt="{0FAB7C05-1C89-4AFF-AC2D-47A2E8F034A1}" src="https://github.com/user-attachments/assets/ebd137ba-5dd8-4dda-9f35-66e9c073d346" />

## Result
The program successfully sorts each column of the NumPy array in ascending order and displays both the original and sorted arrays. 
