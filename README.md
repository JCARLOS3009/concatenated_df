# concatenated_df
Intuition
Approach
Complexity
Time complexity:
Space complexity:
Code
```bash
import pandas as pd

def concatenateTables(df1: pd.DataFrame, df2: pd.DataFrame) -> pd.DataFrame:
    # Concatenate df1 and df2 along rows (axis=0) with ignore_index=True
    concatenated_df = pd.concat([df1, df2], axis=0, ignore_index=True)
    return concatenated_df

# Example DataFrames (moved outside the function for clarity)
df1 = pd.DataFrame({
    'student_id': [1, 2, 3, 4],
    'name': ['Mason', 'Ava', 'Taylor', 'Georgia'],
    'age': [8, 6, 15, 17]
})

df2 = pd.DataFrame({
    'student_id': [5, 6],
    'name': ['Leo', 'Alex'],
    'age': [7, 7]
})
```
# Call the function to concatenate the DataFrames
result = concatenateTables(df1, df2)

# Print the concatenated DataFrame
print("Concatenated DataFrame:")
print(result)
