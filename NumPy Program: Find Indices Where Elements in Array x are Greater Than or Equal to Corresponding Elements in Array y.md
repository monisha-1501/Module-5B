# # NumPy Program: Find Indices Where Elements in Array x are Greater Than or Equal to Corresponding Elements in Array y

## 🎯 Aim
To write a Python program using **NumPy** that finds the indices where elements in array `x` are greater than or equal to their corresponding elements in array `y`.

## 🧠 Algorithm
1. **Import NumPy**: Import the NumPy library.
2. **Define Arrays**: Define two NumPy arrays, `x` and `y`, with the same shape (i.e., same number of elements).
3. **Use Boolean Indexing**: 
   - `x > y` gives a boolean array where elements of `x` are greater than `y`.
   - `x == y` gives a boolean array where elements of `x` are equal to `y`.
4. **Find Indices**: Use `np.where()` to get the indices where the conditions `x >= y` are satisfied.
5. **Print Indices**: Print the indices where the condition holds true.

## 🧾 Program
```
import numpy as np

x = np.array([10, 20, 30, 40, 50])
y = np.array([15, 20, 25, 45, 40])

print("x > y :", x > y)
print("x == y :", x == y)

indices = np.where(x >= y)

print("Indices where x >= y:", indices)
```


## Output
<img width="1382" height="446" alt="{A617700A-1E42-4779-B19E-00AB7B0DEDF4}" src="https://github.com/user-attachments/assets/40debe37-77b6-45cb-b25e-03d8b1471f01" />

## Result
The program successfully identifies and prints the indices where the elements of array x are greater than or equal to the corresponding elements of array y using np.where().
