
## Here are some good points I encountered during my Leetcoding, but not found them in the Complete SQL Mastery:

1. When I need to make a query to return some kind of consecutive records, it is good to think of either self join or lag and lead functions.

LAG and LEAD::

They are analytical functions in SQL that allow you to access data from a previous or subsequent row within a result set. These functions are commonly used for time series analysis, finding the difference between consecutive rows, or comparing values with the previous or next row.

Both LAG and LEAD are window functions in SQL. Window functions perform calculations across a set of rows that are related to the current row. They allow you to perform operations on a "window" of rows defined by a specific criteria.

In the case of LAG and LEAD, the window is determined by the ORDER BY clause within the OVER() clause. The ORDER BY clause specifies the column(s) by which the rows are sorted, defining the order of the window. The PARTITION BY clause, if used, divides the result set into partitions, and the window function is applied separately within each partition.

Window functions like LAG and LEAD operate on a subset of rows within the window, considering the current row and its adjacent rows based on the specified offset. They provide access to the values in the previous or next row, allowing you to perform calculations or comparisons across consecutive rows.

By using window functions, you can avoid self-joins or subqueries that would be necessary to retrieve data from previous or subsequent rows, resulting in more concise and efficient queries.

https://dev.mysql.com/doc/refman/8.0/en/window-function-descriptions.html#function_lag

https://dev.mysql.com/doc/refman/8.0/en/window-function-descriptions.html#function_lead
