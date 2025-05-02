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

# Create first DataFrame
student_data1 = {
    'student_id': ['S1', 'S2', 'S3', 'S4'],
    'name': ['Alice', 'Bob', 'Charlie', 'David'],
    'marks': [85, 90, 78, 92]
}
df1 = pd.DataFrame(student_data1)

# Create second DataFrame
student_data2 = {
    'student_id': ['S5', 'S6'],
    'name': ['Eve', 'Frank'],
    'marks': [88, 80]
}
df2 = pd.DataFrame(student_data2)

# Join the two DataFrames row-wise
combined_df = pd.concat([df1, df2], axis=0)

# Display the combined DataFrame
print(combined_df)
```

## Output
```
  student_id     name  marks
0         S1    Alice     85
1         S2      Bob     90
2         S3  Charlie     78
3         S4    David     92
0         S5      Eve     88
1         S6    Frank     80
```


## Result
The program successfully concatenates two DataFrames along rows using pd.concat() and displays the combined result in a new DataFrame.
