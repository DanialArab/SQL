# SQL

This repo documents my solutions to Leetcode - Database questions using SQL. The Leetcode database was first needed to be regenerated in my MySQL server using the SQL Schema presented in the Leetcode questions. This is required to be able to make a query in the jupyter notebook using my MySQL credentials. The following functions need to be executed to generate the databases in the MySQL server:

    import os
    import pymysql
    import pandas as pd
    password = os.environ.get('MYSQL_PASSWORD')
    
    password = os.environ.get('MYSQL_PASSWORD')

    try:
        con = pymysql.connect(
        host='localhost',
        user='root',
        password=password,
        charset='utf8mb4'
        )
        print("Connection to the database was successful!")
    except pymysql.Error as e:
        print(f"An error occurred while connecting to the database: {e}")
        
    Connection to the database was successful!
    
    # calling this function makes life easy and just need to pass the name of the database I want to make a query on
    # It serves like USE keyword in SQL

    def connector (database, password=password, host='localhost', 
                   user='root', charset='utf8mb4',):

        conn = pymysql.connect(
                            host=host,
                            user=user,
                            password=password,
                            charset=charset, 
                            database=database)

        return conn

my course note (Complete SQL Mastery -- instructor: Mosh Hamedani)
