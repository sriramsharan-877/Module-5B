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
# Step 1: Import NumPy
import numpy as np

# Step 2: Get input for 2D array
rows = int(input("Enter number of rows: "))
cols = int(input("Enter number of columns: "))

print("Enter elements row-wise:")
data = []
for i in range(rows):
    row = list(map(int, input().split()))
    data.append(row)

arr = np.array(data)

# Get new column input
print("Enter new column values:")
new_col = list(map(int, input().split()))
new_col = np.array(new_col)

# Step 3: Delete second column (index 1)
arr_deleted = np.delete(arr, 1, axis=1)

# Step 4: Insert new column at index 1
updated_arr = np.insert(arr_deleted, 1, new_col, axis=1)

# Step 5: Display result
print("Updated Array:\n", updated_arr)
```

## Output
```
Enter number of rows: 3
Enter number of columns: 3
Enter elements row-wise:
1 2 3
4 5 6
7 8 9
Enter new column values:
10 11 12

Updated Array:
 [[ 1 10  3]
  [ 4 11  6]
  [ 7 12  9]]
```

## Result
a **NumPy** program that deletes the second column from a given 2D array and inserts a new column at the same position is verified.

