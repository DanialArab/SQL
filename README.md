# SQL

This repo documents my solutions to Leetcode - Database questions using SQL. The Leetcode database was first needed to be regenerated in my MySQL server using the SQL Schema presented in the Leetcode questions. This is required to be able to make a query in the jupyter notebook using my MySQL credentials. The following functions need to be executed to generate the databases in the MySQL server:

    import os
    import pymysql
    import pandas as pd
    password = os.environ.get('MYSQL_PASSWORD')

my course note (Complete SQL Mastery -- instructor: Mosh Hamedani)
