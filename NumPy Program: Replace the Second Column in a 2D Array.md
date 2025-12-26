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
arr_str = input()
arr = np.array(eval(arr_str))
print("Printing Original array")
print(arr)
arr_deleted = np.delete(arr, 1, axis=1)
print("Array after deleting column 2 on axis 1")
print(arr_deleted)
new_col_str = input()
new_col = np.array(eval(new_col_str))
arr_final = np.insert(arr_deleted, 1, new_col, axis=1)
print("Array after inserting column 2 on axis 1")
print(arr_final)


```

## Output
<img width="891" height="508" alt="530170447-13f97578-5704-4916-b90a-85778c17fe8e" src="https://github.com/user-attachments/assets/074c3d3e-7e21-46b7-bc3e-4c9581e31735" />

## Result
We got the successful output
