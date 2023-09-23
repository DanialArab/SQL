
## Workflow to generate the Leetcode databases in the MySQL server

The following steps detail the functions that need to be executed to generate the databases in the MySQL server using SQL Schema of the Leetcode questions (more details can be found in the Jupyter Notebook **<a href="https://github.com/DanialArab/SQL/blob/master/Leetcode%20Database%20Questions/Leetcode_Database_Questions_Pandas_API.ipynb">Leetcode_Database_Questions_Pandas_API</a>**.):


### 1. Connecting to the MySQL server  


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
    
### 2. Connecting to a database 

The following function provides a handy connection to the desired database, and the user just needs to pass the name of the database he/she wants to make a query on. It serves like USE keyword in SQL.
    
    def connector (database, password=password, host='localhost', user='root', charset='utf8mb4',):
    
        conn = pymysql.connect(
                            host=host,
                            user=user,
                            password=password,
                            charset=charset, 
                            database=database)

        return conn
  
### 3. Creating a database in the MySQL server and populating it with the data based on the SQL Schema of the Leetcode question

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
    in each tuple like data = [('Math'), ('Physics'), ('Programming')] like in Q 1280

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

### 4. Getting the name of databases in the MySQL server

    def database_names():

        # Create a cursor object
        cursor = con.cursor()

        # Execute the SHOW DATABASES command
        cursor.execute('SHOW DATABASES')

        # Fetch all the results as a list of tuples
        results = cursor.fetchall()

        # Print the names of all databases in the MySQL server
        for row in results:
            print(row[0])

        # Close the cursor and connection
        cursor.close()
        con.close()

### 5. Getting the name of the tables in the database

    def table_names (database):

        con = connector(database)

        query = "SELECT table_name FROM information_schema.tables WHERE table_schema='{}';".format(database)

        # Execute the query and store the results in a Pandas DataFrame
        tables = pd.read_sql_query(query, con)

        # Print the list of tables
        return tables

### 6. Deleting a database

    def delete_database(database):
        conn = connector(database=None)
        cursor = conn.cursor()

        # Replace <database_name> with the name of the database you want to delete
        database_name = database

        # Execute the DROP DATABASE SQL command
        cursor.execute(f"DROP DATABASE {database_name}")

        # Commit the transaction
        conn.commit()

        # Close the connection
        conn.close()
    
