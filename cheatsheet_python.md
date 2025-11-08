## Data Cleaning in Python

| Command                                  | Description                            |
| ---------------------------------------- | -------------------------------------- |
| `df.isnull().sum()`                      | Count nulls per column                 | - Handle Missing Data & Duplicate Data - 
| `df.dropna()`                            | Drop rows with missing values          |
| `df.fillna(method='ffill')`              | Fill missing values                    |
| `df.drop_duplicates()`                   | Remove duplicate rows                  |
| `df.replace({'old': 'new'})`             | Replace values in dataframe            |
| `df.head()`                              | Shows first rows of data frame         | - Inspect & Understand the Data - 
| `df.info()`                              | Displays dataframe info and data types |
| `df.describe()`                          | Shows summary statistics               |
| `df.rename(columns={'old': 'new'})`      | Rename columns                         | - Rename, Convert & Clean Columns - 
| `df.astype({'col': 'type'})`             | Change data type of column             |
| `df.drop(['col'], axis=1)`               | Drop one or more columns               |
| `df.reset_index(drop=True)`              | Reset index, drop old index            |
| `df.columns.str.strip()`                 | Strip whitespace from column names     |
| `df.loc[df['col'] > value]`              | Filter using condition                 | - Filter, Slice & Select Rows - 
| `df.iloc[:5]`                            | Select rows by index                   |
| `df['col'].isin(['val1', 'val2'])`       | Filter using multiple values           |
| `df.query('col1 > 10 & col2 == "yes"')`  | Query with expressions                 |
| `pd.concat([df1, df2], axis=0)`          | Concatenate rows                       | - Merge & Group Data - 
| `pd.merge(df1, df2, on='key')`           | Merge on key                           |
| `df.groupby('col').agg({'val': 'mean'})` | Group & aggregate                      |
| `df['col'].value_counts()`               | Frequency of unique values             |
| `df.pivot_table(values, index, columns)` | Pivot table                            |
