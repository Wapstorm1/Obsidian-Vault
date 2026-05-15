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
  
  For example if we have a table users and the users can add phones. If we say SELECT COUNT (phone) FROM USERS. It will count how many users added phones and wont count NULL. It is a simple example - we do not know are there duplicates, or if user does not have a name or the number is incomplete. Just that how many rows with added numbers which are not NULLs.