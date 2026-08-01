# Pandas Commands and Their Task
| Command |  Task  |
|---------|--------|
| pd.read_csv() | Load a CSV |
| df.head() | Preview first rows |
| df.tail() | Preview last rows |
| df.shape | Check rows and columns |
| df.columns | View column names |
| df.info() | View dataset summary |
| df.describe() | View numerical statistics | 

---
# Pandas Filtering Notes
## Selecting One Column
To select one column from a DataFrame:

---python---

df["Name"]

This returns only the Name column.

---
## Selecting Multiple Columns
To select multiple columns from a DataFrame:

---python---
  
df[["Name", "Salary"]]

Notice that two square brackets are used because the second pair creates a list of column names.

---
## Filtering Rows
Example:

---python---
  
df[df["Age"] > 25]

This returns only the row where Age is greater than 25.

---
## Multiple Conditions
AND

---python---
  
df[(df["Age"] > 20) & (df["Department"] == "Sales")]

OR

---python---
  
df[(df["Age"] > 20) | (df["Department"] == "Sales")]


---
## What I Learned
Today I learned that filtering in Pandas works like asking questions about data.
I also learned the difference between AND (&) and OR (|).
AND requires both conditions to br true.
OR requires atleast one condition to be true.
I now understand why each condition is placed inside parentheses.














