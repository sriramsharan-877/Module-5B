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

# Step 3: Sort column-wise
sorted_arr = np.sort(arr, axis=0)

# Step 4 & 5: Display results
print("Original Array:\n", arr)
print("Column-wise Sorted Array:\n", sorted_arr)
```

## Output
```
Enter number of rows: 3
Enter number of columns: 3
Enter elements row-wise:
3 2 1
6 5 4
9 8 7

Original Array:
 [[3 2 1]
  [6 5 4]
  [9 8 7]]

Column-wise Sorted Array:
 [[3 2 1]
  [6 5 4]
  [9 8 7]]
```

## Result
a **NumPy** program that sorts the elements in each column of a given 2D array in ascending order is verified.
