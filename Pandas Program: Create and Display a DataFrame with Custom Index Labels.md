# Pandas Program: Create and Display a DataFrame with Custom Index Labels

## 🎯 Aim

To create and display a **DataFrame** using the **Pandas** library in Python from a given dictionary, and apply specific index labels to the rows.

---

## 🧠 Algorithm

1. **Import Libraries**: Import the required libraries – `pandas` and `numpy`.
2. **Create Dictionary**: Define a dictionary `exam_data` with keys: `'name'`, `'score'`, `'attempts'`, and `'qualify'`.
3. **Index Labels**: Create a list of custom index labels called `labels`.
4. **Create DataFrame**: Use `pd.DataFrame()` to create the DataFrame by passing the dictionary and index labels.
5. **Display Output**: Display the DataFrame using `print()` or by simply calling the DataFrame variable.

---

## 💻 Program
```
# Step 1: Import libraries
import pandas as pd
import numpy as np

# Step 2: Create dictionary
exam_data = {
    'name': ['Ankit', 'Riya', 'Karan', 'Meena', 'John'],
    'score': [90, 75, 88, np.nan, 95],
    'attempts': [1, 2, 1, 3, 1],
    'qualify': ['Yes', 'No', 'Yes', 'No', 'Yes']
}

# Step 3: Define index labels
labels = ['a', 'b', 'c', 'd', 'e']

# Step 4: Create DataFrame
df = pd.DataFrame(exam_data, index=labels)

# Step 5: Display output
print(df)
```

## Output
```
    name  score  attempts qualify
a  Ankit   90.0         1     Yes
b   Riya   75.0         2      No
c  Karan   88.0         1     Yes
d  Meena    NaN         3      No
e   John   95.0         1     Yes
```

## Result
a **DataFrame** using the **Pandas** library in Python from a given dictionary, and apply specific index labels to the rows is verified.
