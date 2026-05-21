`GROUP BY` is used when you want to combine rows with the same value into groups.

> [!NOTE] ## **Main rule**
> When using `GROUP BY`, `SELECT` can contain only:
> 1. Columns listed in GROUP BY
> 2. Aggregate functions

 WHERE **vs** HAVING
`WHERE` filters rows before grouping.
`HAVING` filters groups after grouping.


==GROUP BY = create groups==
==COUNT/SUM/AVG/MIN/MAX = calculate inside each group==
==HAVING = filter groups==