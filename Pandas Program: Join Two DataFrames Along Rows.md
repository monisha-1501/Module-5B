# 🧪 Pandas Program: Join Two DataFrames Along Rows

## 🎯 AIM

To write a Python program using Pandas to **join two DataFrames along rows** (row-wise concatenation) and assign all data to a new DataFrame.

---

## 🧠 ALGORITHM

1. **Import Libraries**: Import the `pandas` library.
2. **Create First DataFrame**: Use a dictionary to create `student_data1`.
3. **Create Second DataFrame**: Use another dictionary to create `student_data2`.
4. **Concatenate DataFrames**: Use `pd.concat()` with `axis=0` to concatenate both DataFrames row-wise.
5. **Display Result**: Print the new combined DataFrame.

---

## 💻 Program
```
import pandas as pd

student_data1 = {
    'Name': ['Anu', 'Bala'],
    'Marks': [85, 90]
}

student_data2 = {
    'Name': ['Charan', 'Divya'],
    'Marks': [78, 88]
}

df1 = pd.DataFrame(student_data1)
df2 = pd.DataFrame(student_data2)

result = pd.concat([df1, df2], axis=0)

print(result)
```

## Output
<img width="1271" height="572" alt="{AA0EDF0E-BBB8-4BEE-82D6-3935F20CBC65}" src="https://github.com/user-attachments/assets/35c97c9a-3cff-467a-a2ba-fbf391107815" />

## Result
The program successfully concatenates the two DataFrames row-wise using pd.concat() and displays the combined DataFrame.
