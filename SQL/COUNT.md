It counts rows or values.

```
SELECT COUNT(*) AS total_users 
FROM users;
```


> [!NOTE] NOTE
> `COUNT(*)` counts every row, including rows with `NULL` values.

The behavior of `COUNT()` depends on the argument used within the parentheses:

- `COUNT(*)` - Counts the total number of rows in a table (including NULL values).
- `COUNT(columnname)` - Counts all non-null values in the column.
- `COUNT(DISTINCT columnname)` - Counts only the unique, non-null values in the column.