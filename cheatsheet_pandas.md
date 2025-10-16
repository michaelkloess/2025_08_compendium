## Data Cleaning & Transformation with pandas

| Command                                           | Description                               |
| ------------------------------------------------- | ----------------------------------------- |
| `df = pd.read_csv('data.csv')`                    | Read CSV file                             |
| `df.head()`                                       | Preview top rows                          |
| `df.info()`                                       | DataFrame overview                        |
| `df.describe()`                                   | Statistical summary                       |
| `df.isnull().sum()`                               | Count missing values per column           |
| `df.fillna(0, inplace=True)`                      | Replace missing values with 0             |
| `df.dropna(inplace=True)`                         | Remove rows with missing values           |
| `df.rename(columns={'old': 'new'}, inplace=True)` | Rename column                             |
| `df[df['col'] > 10]`                              | Filter by condition                       |
| `df.groupby('col').mean()`                        | Group by and calculate mean               |
| `df.sort_values(by='col', ascending=False)`       | Sort by column descending                 |
| `df['new_col'] = df['col1'] + df['col2']`         | Create new calculated column              |
| `df.drop('col_name', axis=1, inplace=True)`       | Drop column                               |
| `df['col'].unique()`                              | Get unique values                         |
| `df['col'].value_counts()`                        | Count frequency of entries                |
| `df['col'] = df['col'].astype(str)`               | Convert data type to string               |
| `df['col'] = df['col'].apply(lambda x: x * 2)`    | Apply custom function                     |
| `df['col'].str.lower()`                           | Convert to lowercase                      |
| `pd.merge(df1, df2, on='id')`                     | Merge DataFrames on common key            |
| `pd.concat([df1, df2])`                           | Concatenate DataFrames                    |
| `df.reset_index(drop=True, inplace=True)`         | Reset index                               |
| `df.set_index('id', inplace=True)`                | Set column as index                       |
| `df.duplicated().sum()`                           | Count duplicate rows                      |
| `df.drop_duplicates(inplace=True)`                | Remove duplicate rows                     |
| `df.to_csv('cleaned.csv', index=False)`           | Save to CSV file                          |
