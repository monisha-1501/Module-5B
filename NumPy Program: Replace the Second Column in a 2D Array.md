# NumPy Program: Replace the Second Column in a 2D Array

## 🎯 Aim
To write a **NumPy** program that deletes the second column from a given 2D array and inserts a new column at the same position.

## 🧠 Algorithm
1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Get a 2D NumPy array and a new column (as another array) from the user.
3. **Delete Column**: Use `np.delete()` to remove the second column (index 1) from the original array.
4. **Insert Column**: Use `np.insert()` to insert the new column at the second column's original position.
5. **Display Result**: Print the updated array with the replaced column.

## 🧾 Program
```
import numpy as np

rows = int(input("Enter number of rows: "))
cols = int(input("Enter number of columns: "))

print("Enter array elements:")
arr = np.array([[int(input()) for j in range(cols)] for i in range(rows)])

print("Enter new column elements:")
new_col = np.array([int(input()) for i in range(rows)])

arr = np.delete(arr, 1, axis=1)
arr = np.insert(arr, 1, new_col, axis=1)

print("Updated Array:")
print(arr)
```

## Output
<img width="1265" height="563" alt="{01A61968-326C-431D-9CB2-1EFFF0A050F9}" src="https://github.com/user-attachments/assets/d15ab811-3cc6-48ee-a611-79bc55286382" />

## Result
The program successfully replaces the second column of the NumPy array with a new column provided by the user and displays the updated array.
