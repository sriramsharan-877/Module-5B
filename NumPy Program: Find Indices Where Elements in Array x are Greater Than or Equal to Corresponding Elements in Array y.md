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
# Step 1: Import NumPy
import numpy as np

# Step 2: Define arrays
x = np.array([1, 5, 3, 7, 9])
y = np.array([2, 5, 1, 8, 6])

# Step 3: Boolean indexing
greater = x > y
equal = x == y

print("x > y :", greater)
print("x == y:", equal)

# Step 4: Find indices where x >= y
indices = np.where(x >= y)

# Step 5: Print indices
print("Indices where x >= y:", indices)
```

## Output
```
x > y : [False False  True False  True]
x == y: [False  True False False False]
Indices where x >= y: (array([1, 2, 4]),)
```

## Result
Python program using **NumPy** that finds the indices where elements in array `x` are greater than or equal to their corresponding elements in array `y` is verified.
