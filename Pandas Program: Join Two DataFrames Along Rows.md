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
# Step 1: Import pandas
import pandas as pd

# Step 2: Create first DataFrame
student_data1 = {
    'name': ['Ankit', 'Riya'],
    'marks': [85, 90]
}
df1 = pd.DataFrame(student_data1)

# Step 3: Create second DataFrame
student_data2 = {
    'name': ['Karan', 'Meena'],
    'marks': [78, 88]
}
df2 = pd.DataFrame(student_data2)

# Step 4: Concatenate DataFrames
combined_df = pd.concat([df1, df2], axis=0)

# Step 5: Display result
print(combined_df)
```

## Output
```
    name  marks
0  Ankit     85
1   Riya     90
0  Karan     78
1  Meena     88
```

## Result
 Python program using Pandas to **join two DataFrames along rows** (row-wise concatenation) and assign all data to a new DataFrame is verified.
