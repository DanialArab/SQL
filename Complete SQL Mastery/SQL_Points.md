
# Here are some good points I encountered during Leetcoding, not found them in the Complete SQL Mastery:

1. When I need to make a query to return some kind of consecutive records, it is good to think of either self join or lag and lead functions.

LAG and LEAD::

They are analytical functions in SQL that allow you to access data from a previous or subsequent row within a result set. These functions are commonly used for time series analysis, finding the difference between consecutive rows, or comparing values with the previous or next row.
