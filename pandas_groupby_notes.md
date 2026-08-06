# Pandas: groupby()
## What is groupby()?
groupby() groups rows that shares the same value in a column.
It does not perform calculations by itself. It simply creates groups that can later be summarized.
## Syntax
df.groupby("Department")
## Example 
Departments:
- Sales
- HR
Pandas groups all Sales rows together and all HR rows together.

## Note:
I've learned that the number of groups created by groupby() depends on the number of unique values in the column being group.
## Selecting a Column After Grouping
df.groupby("Department")["Salary"].mean()
### Explanation
- df.groupby("Department") groups rows by department.
- ["Salary"] selects the Salary column.
- .mean() calculates the average salary.
## Note:
The column selected after the groupby()'s column is the column that the calculation will be performed on.
