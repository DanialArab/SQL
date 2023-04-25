# Structured Query Language 

This repo documents my solutions to Leetcode - Database questions using SQL. The Leetcode database was first needed to be regenerated in my MySQL server using the SQL Schema presented in the Leetcode questions. This is required to be able to make a query in the jupyter notebook using my MySQL credentials. 

Also included in this repo is my notes from a course Complete SQL Mastery by Mosh Hamedani. 

Note on the jupyter notebook files attached to this repo:

- SQL_Coding.ipynb file contains my solution to all of the class exercises.
- SQL_Theoretical_Points.ipynb contains all of the notes I took from the course videos. 
- Leetcode_Database_Questions.ipynb contains my solutions to the Leetcode - database questions using SQL.

The following steps detail the functions that need to be executed to generate the databases in the MySQL server using SQL Schema of the Leetcode questions (more details in the Leetcode_Database_Questions.ipynb file):


## 1. Connecting to the MySQL server  


    import os
    import pymysql
    import pandas as pd
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
    
## 2. Connecting to a database 

The following function provides a handy connection to the desired database, and the user just needs to pass the name of the database he/she wants to make a query on. It serves like USE keyword in SQL.
    
    def connector (database, password=password, host='localhost', user='root', charset='utf8mb4',):
    
        conn = pymysql.connect(
                            host=host,
                            user=user,
                            password=password,
                            charset=charset, 
                            database=database)

        return conn
  
## 3. Creating a database in the MySQL server based on the SQL Schema of the Leetcode question

In terms of Leetcode database questions, the database first need to be regenerated. The function **database_creator** is executed to create a database and then the function **insert_data_to_table** is executed to populate the created database with the data provided by the SQL Schema, found in the Leetcode.com for each SQL questions:
    
    def database_creator(database_name):

        conn = connector(database=None)

        # Create a cursor object
        cursor = conn.cursor()

        # Execute the CREATE DATABASE SQL command
        cursor.execute(f"CREATE DATABASE {database_name}")

        # Commit the transaction
        conn.commit()

        # Close the connection
        conn.close()  
    
    # Populating the created database using the data
    
    def insert_data_to_table(database_name, table_name, schema, data):
        # Connect to the database
        conn = connector(database_name)

        # Create a cursor object
        cursor = conn.cursor()

        # Create the table with the given schema if it does not exist
        cursor.execute(f"CREATE TABLE IF NOT EXISTS {table_name} ({schema})")

        # Truncate the table to remove any existing data
        cursor.execute(f"TRUNCATE TABLE {table_name}")

        # Insert data into the table
        for row in data:
            placeholders = ",".join(["%s" for _ in range(len(row))])
            query = f"INSERT INTO {table_name} VALUES ({placeholders})"
            cursor.execute(query, row)

        # Commit the transaction to save the changes
        conn.commit()

        # Close the connection
        conn.close()

        # This is a modified version of the insert_data_to_table to take care of when we have one item 
        in each tuple like data = [('Math'), ('Physics'), ('Programming')] in Q 1280

    def insert_data_to_table_modified(database_name, table_name, schema, data):
        # Connect to the database
        conn = connector(database_name)

        # Create a cursor object
        cursor = conn.cursor()

        # Create the table with the given schema if it does not exist
        cursor.execute(f"CREATE TABLE IF NOT EXISTS {table_name} ({schema})")

        # Truncate the table to remove any existing data
        cursor.execute(f"TRUNCATE TABLE {table_name}")

         # Insert data into the table
        for row in data:
            if type (row) == tuple:
                placeholders = ",".join(["%s" for _ in range(len(row))])
                query = f"INSERT INTO {table_name} VALUES ({placeholders})"
                cursor.execute(query, row)
            else:
                query = f"INSERT INTO {table_name} VALUES (%s)"
                cursor.execute(query, row)

        # Commit the transaction to save the changes
        conn.commit()

        # Close the connection
        conn.close()
