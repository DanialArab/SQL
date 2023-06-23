# Structured Query Language 

This repo documents my solutions to **Leetcode - Database questions using SQL**. The Leetcode database was first needed to be regenerated in my MySQL server using the SQL Schema, presented along with each Leetcode question. This is required to be able to make a query in the Jupyter Notebook. All of my solutions are presented in Jupyter Notebook **<a href="https://github.com/DanialArab/SQL/blob/master/Leetcode_Database_Questions.ipynb">Leetcode_Database_Questions</a>**. The structure of this repo is as follows: 


1. [Leetcode - Database Questions](#1)
    1. [Leetcode Questions](#2)
    2. [Workflow to generate the Leetcode databases in the MySQL server](#3)
2. [Complete SQL Mastery](#4)


<a name="1"></a>
## Leetcode - Database Questions

<a name="2"></a>
### Leetcode Questions

The following table details the Leetcode database question I solved so far:

|**Index**|**Question ID** | **Question title**|  **Difficulty level**|
| -- | --|  -- | -- |
|1 | 1757| Recyclable and Low Fat Products | Easy |
|2 |1378| Replace Employee ID With The Unique Identifier| Easy | 
|3 |1683| Invalid Tweets | Easy | 
| 4|1741| Find Total Time Spent by Each Employee | Easy |
|5 | 2356| Number of Unique Subjects Taught by Each Teacher| Easy |
| 6| 1693| Daily Leads and Partners| Easy |
|7 | 1795| Rearrange Products Table| Easy |
| 8| 1587| Bank Account Summary II| Easy |
|9 |1581| Customer Who Visited but Did Not Make Any Transactions | Easy |
| 10| 627| Swap Salary| Easy |
|11 |1251| Average Selling Price | Easy |
|12 | 1068| Product Sales Analysis I| Easy |
|13 | 1179| Reformat Department Table| Easy |
|14 | 1484| Group Sold Products By The Date| Easy |
|15 | 1890| The Latest Login in 2020| Easy |
|16 | 1789| Primary Department for Each Employee| Easy |
|17 |1661| Average Time of Process per Machine | Easy |
|18 |1148| Article Views I | Easy |
|19 | 511| Game Play Analysis I| Easy |
|20 | 1327| List the Products Ordered in a Period| Easy |
|21 | 577| Employee Bonus| Easy |
|22 |1965| Employees With Missing Information | Easy |
|23 | 620| Not Boring Movies| Easy |
|24 |1729| Find Followers Count | Easy |
|25 |182| Duplicate Emails | Easy |
|26 | 610| Triangle Judgement| Easy |
|27 | 1211| Queries Quality and Percentage| Easy |
|28 | 1050| Actors and Directors Who Cooperated At Least Three Times| Easy |
|29 | 1280| Students and Examinations| Easy |
|30 | 595| Big Countries| Easy |
|31 | 584| Find Customer Referee| Easy |
|32 | 181| Employees Earning More Than Their Managers| Easy |
|33 |607| Sales Person | Easy |
|34 |183|Customers Who Never Order | Easy |
|35 | 586| Customer Placing the Largest Number of Orders| Easy |
|36 | 1075| Project Employees I| Easy |
|37 | 1633| Percentage of Users Attended a Contest| Easy |
|38 | 1667| Fix Names in a Table| Easy |
|39 | 1407| Top Travellers| Easy |
|40 | 196| Delete Duplicate Emails| Easy |
|41 | 1873| Calculate Special Bonus| Easy |
|42 | 1517| Find Users With Valid E-Mails| Easy |
|43 |619| Biggest Single Number | Easy |
|44 |1978| Employees Whose Manager Left the Company | Easy |
|45 | 1731| The Number of Employees Which Report to Each Employee| Easy |
|46 | 1084| Sales Analysis III| Easy |
|47 | 1141| User Activity for the Past 30 Days I| Easy |
|48 | 596| Classes More Than 5 Students| Easy |
|49 |197| Rising Temperature | Easy |
|50 |1527| Patients With a Condition | Easy |


<a name="3"></a>
### Workflow to generate the Leetcode databases in the MySQL server

The following steps detail the functions that need to be executed to generate the databases in the MySQL server using SQL Schema of the Leetcode questions (more details can be found in the Jupyter Notebook **<a href="https://github.com/DanialArab/SQL/blob/master/Leetcode_Database_Questions.ipynb">Leetcode_Database_Questions</a>**.):


#### 1. Connecting to the MySQL server  


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
    
#### 2. Connecting to a database 

The following function provides a handy connection to the desired database, and the user just needs to pass the name of the database he/she wants to make a query on. It serves like USE keyword in SQL.
    
    def connector (database, password=password, host='localhost', user='root', charset='utf8mb4',):
    
        conn = pymysql.connect(
                            host=host,
                            user=user,
                            password=password,
                            charset=charset, 
                            database=database)

        return conn
  
#### 3. Creating a database in the MySQL server and populating it with the data based on the SQL Schema of the Leetcode question

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

#### 4. Getting the name of databases in the MySQL server

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

#### 5. Getting the name of the tables in the database

    def table_names (database):

        con = connector(database)

        query = "SELECT table_name FROM information_schema.tables WHERE table_schema='{}';".format(database)

        # Execute the query and store the results in a Pandas DataFrame
        tables = pd.read_sql_query(query, con)

        # Print the list of tables
        return tables

#### 6. Deleting a database

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
        
<a name="4"></a>
## Complete SQL Mastery

Also included in this repo are <a href="https://github.com/DanialArab/SQL/tree/master/Complete%20SQL%20Mastery">my notes/a> from the course Complete SQL Mastery. My solutions to all of the class exercises are also detailed in the Jupyter Notebook <a href="linmk)
