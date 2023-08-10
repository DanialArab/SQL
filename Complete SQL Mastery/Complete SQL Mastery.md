## Complete SQL Mastery

Here is the summary of my notes from the course <a href="https://codewithmosh.com/p/complete-sql-mastery">Complete SQL Mastery</a>. The structure of my notes is as follows:

1. [Introduction](#1)
    1. [What is a Database?](#2)
    2. [Relational DBMS](#3)
    3. [Non-relational databases](#4)
    4. [Course structure](#5)
    5. [Connecting to a MySQL Database with Python (Pandas) and Executing pure SQL Queries](#6)
2. [Retrieving Data From a Single Table](#7)
    1. [The SELECT statement](#8)
    2. [The AND, OR, and NOT operators](#9)
    3. [The IN operator in SQL](#10)
    4. [The BETWEEN operator in SQL](#11)
    5. [The LIKE operator](#12)
    6. [The REGEXP operator](#13)
    7. [The IS NULL operator](#14)
    8. [The ORDER BY clause](#15)
    9. [ The LIMIT clause](#16)
3. [Retrieving Data From Multiple Tables](#17)
    1. [Inner Joins](#18)
    2. [Joining across databases](#19)
    3. [Self Joins](#20)
    4. [Joining Multiple Tables](#21)
    5. [Compound Join Conditions](#22)
    6. [Implicit Join Syntax](#23)
    7. [Outer Joins](#24)
    8. [Outer Joins between Multiple Tables](#25)
    9. [Self Outer Joins](#26)
    10. [The Using Clause](#27)
    11. [Natural Joins](#28)
    12. [Cross Joins](#29)
    13. [Unions](#30)
4. [Inserting, Updating, and Deleting Data](#31)
    1. [Column attributes](#32)
    2. [VARCHAR vs. CHAR](#33)
    3. [Inserting a single row into a table](#34)
    4. [Multiline string](#35)
    5. [Inserting Multiple Rows](#36)
    6. [Inserting Hierarchical rows](#37)
    7. [Creating a Copy of a Table](#38)
    8. [Updating a Single Row](#39)
    9. [Updating Multiple Rows](#40)
    10. [Using Subqueries in Updates](#41)
    11. [Deleting rows](#42)
5. [Summarizing Data](#43)
    1. [Aggregate functions](#44)
    2. [The GROUP BY Clause](#45)
    3. [The HAVING Clause](#46)
    4. [The ROLLUP Operator](#47)
6. [Writing a complex query](#48)
    1. [Subqueries](#49)
    2. [Subqueries vs. JOINs](#50)
    3. [ALL](#51)
    4. [ANY or SOME (they are equivalent)](#52)
    5. [Correlated Subqueries](#53)
    6. [EXISTS](#54)
    7. [Subqueries in the SELECT clause](#55)
    8. [Subqueries in the FROM clause](#56)
7. [Essential MySQL Functions](#57)
    1. [NUMERIC Function](#58)
    2. [STRING Functions](#59)
    3. [DATE Functions](#60)
    4. [FORMATTING Date and Times](#61)
    5. [CALCULATING Dates and Times](#62)
    6. [IFNULL and COALESCE Functions](#63)
    7. [IF Function](#64)
    8. [CASE Operator](#65)
8. [VIEWS](#66)
    1. [Creating Views](#67)
    2. [Altering or Dropping VIEWS](#68)
    3. [Updating VIEWS](#69)
    4. [The WITH CHECK OPTION clause](#70)
    5. [ Other benefits of VIEWS](#71)
9. [Stored Procedures and Functions](#72)
    1. [What Stored Procedures are](#73)
    2. [Creating a Stored Procedure](#74)
    3. [Dropping Stored Procedures](#75)
    4. [Parameters](#76)
    5. [Parameters with Default Value](#77)
    6. [Parameter Validation](#78)
    7. [Output Parameters](#79)
    8. [Variables](#80)
    9. [Functions](#81)
    10. [Conventions](#82)
10. [Triggers and Events](#83)
    1. [Introduction](#84)
    2. [Viewing Triggers](#85)
    3. [Dropping Triggers](#86)
    4. [Using Triggers for Auditing](#87)
    5. [ Events](#88)
    6. [Viewing, Dropping and Altering Events](#89)
11. [Transactions and Concurrency](#90)
    1. [Introduction](#91)
    2. [Creating Transactions](#92)
    3. [Concurrency and Locking](#93)
    4. [Concurrency Problems](#94)
    5. [Transaction Isolation Levels](#95)
    6. [READ UNCOMMITTED Isolation Level](#96)
    7. [READ COMMITTED Isolation Level](#97)
    8. [REPEATABLE READ Isolation Level](#98)
    9. [SERIALIZABLE Isolation Level](#99)
    10. [Deadlocks](#100)
13. [Data Types](#101)
    1. [Introduction](#102)
    2. [String Types](#103)
    3. [Integer Types](#104)
    4. [Fixed-point and Floating-point Types](#105)
    5. [Boolean Types](#106)
    6. [Enum and Set Types](#107)
    7. [Date and Time Types](#108)
    8. [Blob Types](#109)
    9. [JSON Type](#110)
15. [Designing Databases](#111)
    1. [Introduction](#112)
    2. [Data Modelling](#113)
    3. [Conceptual Models](#114)
    4. [Logical Models](#115)
    5. [Physical Models](#116)
    6. [Primary Keys](#117)
    7. [Foreign Keys](#118)
    8. [Foreign Key Constraints](#119)
    9. [Normalization](#120)
    10. [1NF- First Normal Form](#121)
    11. [Link Tables](#122)
    12. [2NF- Second Normal Form](#123)
    13. [3NF- Third Normal Form](#124)
    14. [My Pragmatic Advice](#125)
    15. [Don't Model the Universe](#126)
    16. [Forward Engineering a Model](#127)
    17. [Synchronizing a Model with a Database](#128)
    18. [Reverse Engineering a Database](#129)
    19. [Project- Flight Booking System](#130)
    20. [Project - Video Rental Application](#131)
    21. [Creating and Dropping Databases](#132)
    22. [Creating Tables](#133)
    23. [Altering Tables](#134)
    24. [Creating Relationships](#135)
    25. [Altering Primary and Foreign Key Constraints](#136)
    26. [Character Sets and Collations](#137)
    27. [Storage Engines](#138)
17. [Indexing for High Performance](#139)
    1. [Introduction](#140)
    2. [Indexes](#141)
    3. [Creating Indexes](#142)
    4. [Viewing Indexes](#143)
    5. [Prefix Indexes](#144)
    6. [Full-text Indexes](#145)
    7. [Composite Indexes](#146)
    8. [Order of Columns in Composite Indexes](#147)
    9. [When Indexes are Ignored](#148)
    10. [Using Indexes for Sorting](#149)
    11. [Covering Indexese](#150)
    12. [Index Maintenance](#151)
19. [Securing Databases](#152)
    1. [Introduction](#153)
    2. [Creating a User](#154)
    3. [Viewing Users](#155)
    4. [Dropping Users](#156)
    5. [Changing Passwords](#157)
    6. [Granting Privileges](#158)
    7. [Viewing Privileges](#159)
    8. [Revoking Privileges](#160)

   
<a name="1"></a>
### Introduction 

<a name="2"></a>
#### What is a Database? 

A database is a collection of data stored in a format that can be easily accessed. In order to manage our databases we use a software called database management system (DBMS). DBMS are categorized as two broad categories:

+ Relational
+ NoSQL

<a name="3"></a>
#### Relational DBMS

We store data in tables that are linked to each other using relationships, each table stores data about a specific type of object. We use Structured Query Language (SQL) to work with these relational DBMSs. We use SQL to query or modify our data. There are various RDBMS:

+ MySQL
+ SQL Server
+ Oracle
+ ...

All of these flavors are based on the standard specifications of SQL. So what I learn in this course mostly can be applied to any of these RDBMS. In this course, we use MySQL, which is the most popular open-source database in the world.

<a name="4"></a>
#### Non-relational databases

In Non-relational databases, we don’t have tables or relationships, these databases are very different from relational databases and NoSQL systems don’t understand SQL and they have their own query language.

<a name="5"></a>
#### Course structure

Even though we use MySQL in this course, what we will be learning will be applicable at least 90% to other DBMSs. There might be a slight difference in syntax though.

Topics: 

+ Retrieving data
+ Inserting data
+ Updating data
+ Deleting data
+ Summarizing data for creating reports
+ Writing complex queries using subqueries
+ Built-in functions

As you process you see you are writing the same queries again and again and so we will learn about the followings for **storing queries and reusing them** later:

+ Views
+ Stored procedures

These are great for increasing our productivity.

Some advanced topics:

+ Triggers
+ Events
+ Transactions
+ Concurrency

Skills helping an individual stand out: 

+ Designing databases
+ Indexing for high performance, indexes are essential when your database grows in size, we can speed up our queries using indexes. If you have billions of records you want to query pretty quickly using indexes
+ Securing databases

<a name="6"></a>
#### Connecting to a MySQL Database with Python (Pandas) and Executing pure SQL Queries

In order to run pure SQL code in python, I followed the following procedure (this way allows me to push all my codes, which were run in jupyter notebook, into my GitHub repo rather than running SQL queries in my local using MySQL Workbench as a database management tool to interact with MySQL):

Create a connection to my MySQL server:

        def connector (database, password=password, host='localhost', 
                         user='root', charset='utf8mb4',):
        
              con = pymysql.connect(
                                  host=host,
                                  user=user,
                                  password=password,
                                  charset=charset, 
                                  database=database)
        
              return con
        
          con = connector (database) 

Execute the SQL query

          cursor = con.cursor()
          cursor.execute("""
        
          SELECT *
          FROM orders
        
          """)
          con.commit()
        
          cursor.close()
          con.close()

          results = cursor.fetchall()
        
          df = pd.DataFrame(results, columns=[desc[0] for desc in cursor.description])

some notes on cursor object:

In Python, we can interact with MySQL databases using the MySQL Connector/Python module, which provides a Cursor object for executing SQL queries.

A cursor is an object that allows me to execute SQL statements and retrieve data from a MySQL database. It acts as a pointer to a specific row or set of rows within a result set. The Cursor object is created by calling the cursor() method on a MySQL connection object.

Once the cursor object is created, I can execute SQL queries using the execute() method. The results of the query can be retrieved using the fetchall() method.

It's important to note that after executing a SQL query, you need to either fetch all the rows returned by the query or use one of the other fetch methods (fetchone(), fetchmany()) to retrieve specific rows. After you're done working with the cursor object, you should close it using the close() method to free up system resources.

note on pd.read_sql vs. using cursor object:

If I just need to execute a simple SELECT statement and retrieve the results as a Pandas DataFrame, then using the pd.read_sql() function is a more convenient option than using a cursor object.

But if I need to execute more complex SQL queries that involve multiple statements, transaction management, or other advanced features, then I may need to use a cursor object instead of pd.read_sql().
  
<a name="7"></a>
### Retrieving Data From a Single Table 

<a name="8"></a>
#### The SELECT statement

        USE sql_store; 
        
        SELECT * (in front of that we specify the columns that we want to retrieve, * means all columns) 
        FROM customers (here we specify the table that we want to query)
        WHERE customer_id = 1 (we use this clause to filter data)
        ORDER BY first_name (we use this clause to sort data and here we specify the columns that we want to sort the results on)

The first step to write a query to get data from a database is to select the database, the query that we write will be executed against that database. We use USE keyword to select the database.

Points:

SQL is NOT a case-sensitive language meaning we can use USE sql_store or use sql_store BUT as the best practice we should capitalize all the SQL keywords and everything else in lowercase
When you have multiple SQL statements we need to terminate each statement using a semicolon (;)
Comment in SQL is two hyphens –- and the SQL engine will not execute these comments
After executing:

USE sql_store (by double clicking on the sql_store we can achieve the same thing)
The sql_store is marked as bold in the schemas database (in the left panel)

**The order of these clauses (SELECT FROM WHERE ORDER BY) matters. And if we don’t follow the above order we get a syntax error.**

The three clauses of FROM, WHERE, ORDER BY are all optional but we mostly use them. Also we don’t need to put different clauses in different lines b/c tab, whitespaces, and line breaks are ignored when SQL code is executed. So we may have

        SELECT * FROM customers WHERE customer_id = 1 ORDER BY first_name 
        
This is fine for simple queries but as your queries get more complex it is better to put each clause on a new line.

<a name="9"></a>
#### The AND, OR, and NOT operators

AND is operated first! But we use parenthesis to make our code cleaner and easier to understand.

<a name="10"></a>
#### The IN operator in SQL

        USE sql_stores; 
        
        SELECT *
        FROM customers 
        WHERE state = ‘VA’ OR state = ‘FL’ OR state = ‘GA’ 
    
But we can use IN operator to have a cleaner code like

        SELECT *
        FROM customers 
        WHERE state IN (‘VA’, ‘GA’, ‘FL’) -- The order does NOT matter 
    We also can use NOT operator like to get the customers outside of these states:
    
        SELECT *
        FROM customers 
        WHERE state NOT IN (‘VA’, ‘GA’, ‘FL’)
    
<a name="11"></a>
#### The BETWEEN operator in SQL

Whenever we are comparing an attribute with a range of values we can use BETWEEN operator to make you code shorter and cleaner like:

        USE sql_store;
        SELECT *
        FROM customers 
        WHERE points BETWEEN 1000 AND 3000 -- The range values is inclusive. 

<a name="12"></a>
#### The LIKE operator

How to retrieve rows that match a specific string pattern? Like we want to get the customers whose last names start with “b”:

Use % to indicate any number of characters after “b”, also it doesn’t matter if it is a lower case or upper case “b”

        SELECT *
        FROM customers
        WHERE last_name LIKE “b%”
        
The percent sign doesn’t have to be at the end but it could be anywhere like we want to get customers with “b” character in their last name whether in the beginning or at the end or in the middle, for that we change our pattern to “%b%” meaning we can have any number of characters before or after “b”:

        SELECT *
        FROM customers
        WHERE last_name LIKE “%b%”

For the customers with last name ending in “y” we use this pattern “%y”. We also have underscore “_”that matches a single character like in the following we will get the customers whose last names are exactly TWO characters long and it ends in y and we don’t care what the first character is:

        SELECT *
        FROM customers 
        WHERE last_name LIKE “_y”

Another pattern is “b____y” and you know what it means!

The LIKE operator in MySQL is an older operator and we have a newer one which is more powerful which allows us to search for any string pattern. We will discuss next.

<a name="13"></a>
#### The REGEXP operator

REGEXP is short for the regular expression. REGEXP is extremely powerful when it comes to searching for strings. They allow us to search for more complex patterns. The newer and better operator compared to LIKE.

Some examples:

Let’s say if we want to have customers whose last names include field, if we want to use LIKE operator:

        SELECT *
        FROM customers
        WHERE last_name LIKE “%field%”

BUT if we use REGEXP we do NOT need % to indicate that the field word could be anywhere and the above query would be simplified to as:

        SELECT *
        FROM customers
        WHERE last_name REGEXP “field”

In REGEXP we have additional characters that we don’t have in LIKE operator. Like

+ ^ to indicate the beginning of the string like

        WHERE last_name REGEXP “^field”	means the last_name MUST start with field
  
+ $ to indicate the end of the string like

        WHERE last_name REGEXP “field$” means the last name must end with field
  
We can also search for multiple words, to do so we use pipe (|) for logical or for multiple search patterns, like to get customers who have field or mac in their last names:

        WHERE last_name REGEXP “field|mac” 
  
We can take this to the next level like finding customers who have the words field or mac or rose in their last names:

        WHERE last_name REGEXP “fiels|mac|rose”

        WHERE last_name REGEXP “^field|mac$|rose”
  
We want to get customers who have letter e in their last names and also before the letter e there is either g or i, to achieve this we use square brackets [] and inside it we can add multiple characters like “[gi]e”

        WHERE last_name REGEXP “[gi]e”
        
        WHERE last_name REGEXP “e[gi]”
  
We can also supply a range of characters like if we want to have any character from a to h before the letter e

        WHERE last_name REGEXP “[a-h]e”

There are more special characters in MySQL than listed above but honestly the ones on above are the ones you use 90 % of the times. So just learn these and you are good to go!

<a name="14"></a>
#### The IS NULL operator

How to look for records that miss an attribute? Like if we want to find all the customers that don’t have a phone number and like we want to send an email to them and say please provide phone number. To do so we use IS NULL operator:

        SELECT *
        FROM customers
        WHERE phone IS NULL 

Here we also can use NOT operator to get the customers who do have a phone like

        SELECT *
        FROM customers
        WHERE phone IS NOT NULL
        
<a name="15"></a>
#### The ORDER BY clause

How to sort data in your SQL queries?

By default the data in our query is sorted by the customer_id. Why is the customer_id column the default sort column?

Because the customer_id column is the primary key column for the table customers. You can figure it out by clicking the tools like button on the right of the table customers name and then see the customer table in the design mode. Here you see that there is a yellow key just before the customer_id meaning this is a primary key column for this table. In relational databased every table should have a primary key column and the values in that column should uniquely identify the records in that table. So that is why in our query the data is sorted by the custiomer_id which is the primary key. To sort the customers by different column:

        SELECT *
        FROM customers 
        ORDER BY first_name 

To reverse the order:

        SELECT *
        FROM customers
        ORDER BY first_name DESC

We can also sort data by multiple columns for example:

Let’s say we want to first sort customers based on their state and then within each state we want to sort them by their first name:

        SELECT *
        FROM customers
        ORDER BY state, first_name 

We can also use a descending argument anywhere like:

        SELECT *
        FROM customers
        ORDER BY state, first_name DESC 

The difference between MySQL and other DBMSs is that in MySQL we can sort by any columns whether that column is in the SELECT clause or NOT like:

        SELECT first_name, last_name
        FROM customers
        ORDER BY state

Here although I don’t have state column in SELECT clause but I can sort data based on that. But other DBMSs sometimes yell at you when you try to do sorting like this.

We also can sort data by an alias like:

        SELECT first_name, last_name, 10 AS points 
        FROM customers
        ORDER BY points, first_name 

AVOID: you can also sort data by columns position like:

        SELECT first_name, last_name
        FROM customers
        ORDER BY 1, 2 – these are the orders of the columns in the SELECT clause 

This query sorts data by first_name and then last_name.

BUT avoid this b/c if in the future you have a change in the columns in the SELECT clause like:

        SELECT birth_data, first_name, last_name 
        FROM customers
        ORDER BY 1, 2

The data would be sorted differently and generates unexpected results and so avoid sorting by column’s positions INSTEAD ALWAYS SORT BY COLUMNS’NAMES.

<a name="16"></a>
#### The LIMIT clause

How to limit the number of records from your query? Like if we only want to get the three first customers we use the LIMIT clause:

        SELECT *
        FROM customers
        LIMIT 3

We can optionally supply an offset which is useful for situations we want to paginate data. Like:

        SELECT *
        FROM customers
        LIMIT 6, 3 

Here 6 is an offset and tells MySQL to skip the first 6 records and then pick three records.

Exercise: get the top three loyal customers, like the ones with highest points

        SELECT *
        FROM customers
        ORDER BY points DESC 
        LIMIT 3 

POINT: Again the order matters! The LIMIT clause should always come at the end.

<a name="17"></a>
### Retrieving Data From Multiple Tables

<a name="18"></a>
#### Inner Joins

So far we only selected columns from a single table but in the real world we quite often select columns from multiple tables. Like:

        SELECT *
        FROM orders
        JOIN customers 
            ON orders.customer_id = customers.customer_id 

this JOIN is the same as INNER JOIN where INNER is optional, we also have OUTER JOIN, which will be discussed later

With this query we tell MySQL that hey whenever you are joining the orders table with customers table make sure that the customer_id column in the orders table equals customer_id column in the customers table.

The output would be all the columns from the two tables, first all the columns from orders table, b/c we have listed this table first, and then all the columns from the customers table. Let’s simplify the results:

        SELECT order_id, first_name, last_name
        FROM orders
        JOIN customers 
            ON orders.customer_id = customers.customer_id 

What if we want to display the customer_id as well?

        SELECT order_id, customer_id, first_name, last_name
        FROM orders
        JOIN customers 
            ON orders.customer_id = customers.customer_id 

This query throws an error b/c I have the column customer_id in two tables! The error says that customer_id column in the field list is ambiguous! So I need to specify from which table like:

        SELECT order_id, orders.customer_id, first_name, last_name
        FROM orders
        JOIN customers 
            ON orders.customer_id = customers.customer_id         

Now it works!

Points:

In situations where we have same column in multiple tables we need to prefix the name of the column with the name of the table like above

ON phrase specifies the basis based on which we want to join the tables, after ON we need to specify the condition

We can use an alias to make our code cleaner, NOTE: if you give an alias to a table you have to use that alias everywhere else otherwise you get an error.

          SELECT order_id, o.customer_id, first_name, last_name
          FROM orders o
          JOIN customers c 
              ON o.customer_id = c.customer_id

<a name="19"></a>
#### Joining across databases

How to combine columns from tables across multiple databases?

What we did so far was to combine columns from multiple tables within a database, sql_store, but now we want to combine columns from tables across multiple databases. We need to prefix the table in JOIN with its database name:

        USE sql_store;
        SELECT *
        FROM order_items oi
        JOIN sql_inventory.products p 
            ON oi.product_id = p.product_id 

So we successfully joined tables across multiple databases.

We need this prefix, sql_inventory.products, b/c the database we write this query against is the sql_store database. Also

        USE sql_inventory;
        SELECT *
        FROM sql_store.order_items oi 
        JOIN products p 
            ON oi.product_id = p.product_id 
    
LESSON ----> I only have to prefix the tables that are NOT part of the current database. And so my query would be different depending on the current database.

<a name="20"></a>
#### Self Joins

In SQL we can also join a table with itself. Let’s write a query to get each employee and their manager

        USE sql_hr;
        SELECT 
            e.employee_id, 
            e.first_name, 
            m.first_name AS Manager
        FROM employees e
        JOIN employees m 
            ON e.reports_to = m.employee_id
    
Joining a table with itself is pretty similar to joining a table with another table the only difference is that we have to use different aliases and we have to prefix each column with an alias, this is called self-join.

<a name="21"></a>
#### Joining Multiple Tables

How to join more than TWO tables when writing a query?

We want to write a query to join the orders table with two tables: the customers table and the order_statuses table.

        USE sql_store;
        SELECT 
            o.order_id, 
            o.order_date, 
            c.first_name, 
            c.last_name, 
            os.name AS status 
        FROM orders o
        JOIN customers c
            ON o.customer_id = c.customer_id 
        JOIN order_statuses os 
            ON o.status = os.order_status_id 
    
Exercise: write a query to join the payment table with the payment methods table as well as the client table and produce a report that shows the payment with more details such as the client’s name and the payment method:

        USE sql_invoicing;
        SELECT 
            p.date,
            p.invoice_id,
            p.amount,
            c.name,
            pm.name AS payment 
        FROM payments p
        JOIN clients c 
            ON p.client_id = c.client_id 
        JOIN payment_methods pm
            ON p.payment_method = pm.payment_method_id 

<a name="22"></a>
#### Compound Join Conditions

In all examples so far, we used a single column to uniquely identify the rows in a given table. There are times when we cannot use a single column to uniquely identify records in a given table. In these cases we use a combination of values in multiple columns to uniquely identify each record.

Here, we need multiple conditions to join two tables.

In some tables we have a composite primary key. A composite primary key contains more than one column. When you have a table with a composite primary key you need to learn how to join that table with other tables:

        USE sql_store;
        SELECT *
        FROM order_items oi
        JOIN order_item_notes oin
            ON oi.order_id = oin.order_id
            AND oi.product_id = oin.product_id
    
<a name="23"></a>
#### Implicit Join Syntax

We have the following basic JOIN (explicit join):

        SELECT *
        FROM orders o
        JOIN customers c
            ON o.customer_id = c.customer_id 
            
There is another way to write this query using implicit join syntax:

        SELECT *
        FROM orders o, customers c
        WHERE o.customer_id = c.customer_id 

Same as explicit join, we will get 10 records (we have 10 in each orders and customers tables).

Although MySQL supports this syntax I suggest you not to use this implicit join syntax b/c if you accidentally forget to type the WHERE clause you will get a cross join:

        SELECT *
        FROM orders o, customers c

In this case every record in the orders table is joined with every record in the customers table and we end up having 100 records! Later in the section we talk in more details about cross join.

Lesson ----> avoid using implicit join syntax and instead use the explicit join syntax!

<a name="24"></a>
#### Outer Joins

With the (INNER) JOIN we only get the records meeting the condition we specified in JOIN (after ON) but what if we want to get other records, not meeting the condition, as well? Use OUTER JOIN

We have two types of (OUTER) JOIN:

+ LEFT, all the records in the LEFT table (the one comes first in front of FROM is returned whether or not the JOIN condition is True)

+ RIGHT, all the records in the RIGHT table (the one comes in front of JOIN is returned whether or not the JOIN condition is True)

        USE sql_store; 
        SELECT p.product_id, 
                p.name, 
                oi.quantity 
        FROM products p 
        LEFT JOIN order_items oi 
            ON p.product_id = oi.product_id

So whenever you see JOIN it is inner join and LEFT/RIGHT JOIN it is outer join. As a best practice avoid RIGHT JOIN and always use LEFT JOIN instead!

<a name="25"></a>
#### Outer Joins between Multiple Tables

As a best practice avoid RIGHT JOIN and always use LEFT JOIN instead! It is easier to visualize your query.

        USE sql_store;
        SELECT 
            o.order_id,
            o.order_date,
            c.first_name AS customer, 
            sh.name AS shipper,
            os.name AS status 
        FROM orders o
        JOIN customers c 
            ON o.customer_id = c.customer_id 
        LEFT JOIN shippers sh
            ON o.shipper_id = sh.shipper_id 
        JOIN order_statuses os
            ON o.status = os.order_status_id 
    
<a name="26"></a>
#### Self Outer Joins

        USE sql_hr;
        SELECT 
            e.employee_id,
            e.first_name AS employee
            m.first_name AS manager 
        FROM employees e
        LEFT JOIN employees m
            ON e.reports_to = m.employee_id
    
<a name="27"></a>
#### The Using Clause

We can use USING clause with both INNER and OUTER JOIN.

We use USING clause to make our query shorter and cleaner, we use it whenever the column name in both tables are EXACTLY the same, like

        USE sql_store;
        SELECT 
            o.order_id,
            c.first_name,
            sh.name AS shipper
        FROM orders o
        JOIN customers c
            ON o.customer_id = c.customer_id 
    
The simpler query using USING keyword is:

        USE sql_store;
        SELECT 
            o.order_id,
            c.first_name,
            sh.name AS shipper
        FROM orders o
        JOIN customers c
            USING (customer_id)  
        LEFT JOIN shippers sh
            USING (shipper_id) 
            
Again remember, USING clause works ONLY if the columns are of exactly the same name across multiple tables.

What if we have multiple columns in our JOIN condition? If you remember we had the following before:

        SELECT *
        FROM order_items oi
        JOIN order_item_notes oin
            ON oi.order_id = oin.order_id
            AND oi.product_id = oin.product_id
    
The above JOIN condition is messy we can simplify it using USING keyword:

        SELECT *
        FROM order_items oi
        JOIN order_item_notes oin
            USINT (order_id, product_id) 
    
Exercise:

Write a query to select payments from the payments table and produce a report including date, client, amount, and name of the payment method:

        USE sql_invoicing;
        SELECT 
            p.date,
            c.name AS client,
            p.amount,
            pm.name AS payment_method 
        FROM clients c
        JOIN payments p USING (client_id)
        JOIN payment_methods pm
            ON p.payment_method = pm.payment_method_id -- here I cannot use USING clause b/c the name of the column in the p and pm tables are NOT the same! 
    
<a name="28"></a>
#### Natural Joins

In MySQL we also have another simpler way to join two tables, which is easier to code BUT NOT RECOMMENDED! Because it sometimes produces unexpected results. You will be presented here to make sure you understand it if you see it somewhere but don’t use it yourself.

        USE sql_store;
        SELECT
            o.order_id,
            c.first_name
        FROM orders o
        NATURAL JOIN customers c

With natural JOIN we don’t explicitly specify the column names. The database engine looks at these two tables and join them based on the common columns i.e., columns that have the same names that is the reason this query is shorter to write.

<a name="29"></a>
#### Cross Joins

We use cross JOIN to join every record in the first table with every record in the second table. So that is why we don’t have a condition using ON keyword in the cross JOIN.

        USE sql_store;
        SELECT 
            c.first_name AS customer,
            p.name AS product
        FROM customers c
        CROSS JOIN products p
        ORDER BY c.first_name 

What we have above is called the explicit syntax for CROSS JOIN. We also have implicit syntax which looks like the following: Instead of typing CROSS JOIN products p we type multiple tables in FROM clause like:

        USE sql_store;
        SELECT
            c.first_name AS customer,
            p.name AS product
        FROM customers c, products p
        ORDER BY c.first_name

MOSH advice: he prefers the explicit syntax b/c it is more clear.

<a name="30"></a>
#### Unions

So far we learned that how to join columns from multiple tables. But in SQL we can also JOIN rows from multiple tables, which is extremely powerful.

Using UNION operator we can combine records from multiple queries.

        USE sql_store;
        SELECT 
            Order_id,
            Order_date,
            ‘Active’ AS status
        FROM orders o
        WHERE o.order_date >= “2019-01-01” -- here I hard coded the current year date, which does not deliver the desired results next year and so we will learn how to not hard code this later in the course. 
        UNION
        SELECT 
            ordare_id,
            order_date,
            ‘Archived’ AS status 
        FROM orders o
        WHERE o.order_date < “2019-01-01”

In the above both the queries are from the same table, you also can query from different tables and then using UNION operator you can combine the results into one result set.

Like:

        SELECT first_name
        FROM customers
        UNION
        SELECT name
        FROM shippers 

The name of the column in the returned results is based on the first query like in the above the name of the column in the returned result is first_name. we can also have an alias like SELECT first_name AS full_name.

Just remember the number of columns each query returns should be equal otherwise you will get an error. We get an error running the following b/c the first query returns 2 columns and the second one returns only one column!

        SELECT first_name, last_name 
        FROM customers
        UNION
        SELECT name
        FROM shippers 

Exercise:

Points < 2000 >>> type would be Bronze 
2000 <Points < 3000 >>> type would be Silver  
Points > 3000 >>> type would be Gold 
And also sort the results by the first name of the customers. 
My solution:

        USE sql_store;
        SELECT 
            customer_id,
            first_name,
            points,
            ‘Gold’ AS type
        FROM customers 
        WHERE points > 3000
        UNION
        SELECT 
            customer_id,
            first_name,
            points,
            ‘Silver’ AS type
        FROM customers
        WHERE points BETWEEN 2000 AND 3000
        UNION
        SELECT 
            customer_id,
            first_name,
            points,
            ‘Bronze’ AS type
        FROM customers
        WHERE points < 2000
        ORDER BY first_name 

<a name="31"></a>
### Inserting, Updating, and Deleting Data

<a name="32"></a>
#### Column attributes

In MySQL workbench, I can open a table in a design mode through clicking on the tool sign beside table name and learn about column attributes. But in Pandas, I can get the column attributes using the following function:

        def column_attribute (database, table_name):
        
            con = connector(database)
        
            query = """
                SELECT column_name, data_type
                FROM information_schema.columns
                WHERE table_name = '{}'
            """.format(table_name)
        
            # read the query result into a DataFrame
            df = pd.read_sql(query, con)
            return df

<a name="33"></a>
#### VARCHAR vs. CHAR

VARCHAR and CHAR are both SQL data types used to store character strings, but they have some differences in terms of their storage and usage.

CHAR is a fixed-length string data type, which means that it always allocates a fixed amount of space for each value, regardless of whether the value needs it or not. For example, if you define a column as CHAR(10), each value in that column will take up exactly 10 bytes of storage, regardless of whether the actual value is shorter or longer than 10 characters. This makes CHAR more efficient for fixed-length data, such as postal codes or phone numbers.

VARCHAR, on the other hand, is a variable-length string data type. It allocates only as much space as the value needs, plus a small amount of overhead to store the length of the value. For example, if you define a column as VARCHAR(10), a value that is 5 characters long will take up only 5 bytes of storage, plus an additional byte to store the length of the value. This makes VARCHAR more efficient for variable-length data, such as names or addresses.

In general, it is recommended to use VARCHAR for most string data types, unless you know that the data will always be fixed-length. The reason is that VARCHAR is more flexible and efficient in terms of storage space. However, if you know that your data will always be fixed-length, CHAR can be more efficient in terms of processing time, as it eliminates the need to calculate the length of each value during queries.

Here is an example of how you can create a table with CHAR and VARCHAR columns in SQL:

SQL code:

        CREATE TABLE users (
            id INT PRIMARY KEY,
            postal CHAR(50),
            email VARCHAR(100)
        );
        
In this example, the postal column is defined as a CHAR column with a fixed length of 50 characters, while the email column is defined as a VARCHAR column with a maximum length of 100 characters.

<a name="34"></a>
#### Inserting a single row into a table

        USE sql_store;
        INSERT INTO customers
        VALUES (
            DEFAULT,
            ‘John’,
            ‘Smith’,
            ‘1990-01-01’,
            NULL, 
            ’address’,
            ‘city’,
            ‘CA,
            DEFAULT)
    
This way we can add a row to our table called customers. However, since we only provide values for some of the columns there is another way to write this statement:

In this way we can optionally supply the name of columns we want to supply values for, this way we don’t need to provide the default or null values as above:

        INSERT INTO customers (
                        first_name,
                        last_name,
                        birth_date,
                        address,
                        city,
                        state)
        VALUES(
                        ‘John’,
                        ‘Smith’,
                        ‘1990-01-01’,
                        ’address’,
                        ‘city’,
                        ‘CA)
                
This way we can also change the order of columns in the statement and so we don’t need to follow the columns order as in the table like:

        INSERT INTO customers (
                            last_name,
                            first_name,
                            birth_date,
                            address,
                            city,
                            state)
        VALUES(
                            ‘Smith,
                            ‘John,
                            ‘1990-01-01’,
                            ’address’,
                            ‘city’,
                            ‘CA)
                    
Be aware of opening a table in a design mode through clicking on the tool sign beside table name and learn about column attributes. Notice for the customer_id column the AI (Auto increment) is checked. Pay attention that here MySQL automatically generates the value of 11 for the customer_id value for the new row; it gets the value of the customer_id column for the last row and increments it by one and assigns it to the customer_id value for the new added row.

To achieve the same using Pandas, I need:

        con = connector('sql_store')
        cursor = con.cursor()
        
        cursor.execute("""
            INSERT INTO shippers (name) 
            VALUES  ('shipper1')
        
        """)
        
        con.commit()

<a name="35"></a>
#### Multiline string

The """ at the beginning and end of the query is called a multiline string, or a triple-quoted string. It is a Python syntax feature that allows you to define a string that spans multiple lines of code.

In this case, the triple-quoted string is used to define a multiline SQL query that spans multiple lines of code in the Python script. It makes the code more readable and easier to maintain, especially for longer SQL queries that might be harder to read if they were defined as a single line of code.

Note that triple-quoted strings are not required to execute SQL queries in Python, and you can define SQL queries as regular strings using single or double quotes. However, when defining long SQL queries, it can be useful to use triple-quoted strings to make the code more readable.

example:

        pd.read_sql("""
                    SELECT *
                    FROM customers
        
                    """, con)
            
<a name="36"></a>
#### Inserting Multiple Rows

We just need to supply different rows’ values in separate parenthesis in front of VALUES like

        USE sql_store;
        INSERT INTO shippers (name)
        VALUES (‘shipper1’),
            (‘shipper2’),
            (‘shipper3’) 
    
<a name="37"></a>
#### Inserting Hierarchical rows

So far we learned how to enter data into a single table. Here we will learn how to insert data into multiple tables.

We have a parent table and a child table like in our sql_store database we have orders table as parent table and order_items table as child table. So one row in orders table can have one or more children inside the order_items table. We want to insert an order and all its items, which requires us to insert data into multiple tables:

        USE sql_store;
        INSERT INTO orders (customer_id, order_date, status) -- order_id is auto increment of orders table and so it will be generated, I need to get it through executing LAST_INSERT_ID () function to use it to insert the child record into the child table i.e., order_items
        VALUES (1, ‘2019-01-02’, 1);
        INSERT INTO order_items 
        VALUES 
            (LAST_INSERT_ID(), 1, 1, 2.95),
            (LAST_INSERT_ID(), 2, 1, 3.95)
Some points:

In MySQL there are bunch of built-in functions. We can call/execute the function LAST_INSERT_ID () to access the ID that MySQL generates when we insert a new row. We use LAST_INSERT_ID () to get the ID of the newly inserted record. So we can use that ID to insert the child record.

note on running sql code in Pandas:

I needed to separate the two INSERT queries like in the following otherwise I got programmingerror:

        cursor = con.cursor()
        
        cursor.execute("""
        
        INSERT INTO orders (customer_id, order_date, status)
        VALUES (1, '2019-01-02', 1); 
        
        """)
        
        cursor.execute("""
        
        INSERT INTO order_items
        VALUES 
            (LAST_INSERT_ID(), 1, 1, 2)
        """)
        
        con.commit()

<a name="38"></a>
#### Creating a Copy of a Table

We will learn how to copy data from one table to another.

Let’s say we want to make an exact copy of table orders, we can use the following:

CREATE TABLE name_of_the_new_table AS then we use SELECT statement to get everything from orders table:

        USE sql_store;
        CREATE TABLE orders_archived AS
        SELECT *
        FROM orders 

This way we can create an exact copy of orders table, but if we open the orders_archived table in design mode we see in this table we don’t have a primary key and auto increment for this table. So when creating a table using this technique MySQL ignores these attributes and that means if we want explicitly insert a record into the orders_archived we have to supply a value for order_id as well (order_id is the primary key and also marked as auto increment in the orders table).

In the above query we refer to the SELECT statement as a subquery. A subquery is a SELECT statement that is part of another SQL statement. We can also use a subquery in an INSERT statement and that is a very powerful technique like:

Side note: To delete all the data in a table we can right click on the table name in the schemas and then click Truncate Table, this deletes all the data in the table.

I can achieve this using Python as follows:

        con = connector('sql_store')
        
        cursor = con.cursor()
        
        cursor.execute("""
        
        TRUNCATE TABLE orders_archived
        
        """)
        
        con.commit()
        
        con.close()

How to copy a subset of a table into a new table? using a subquery in an INSERT statement, like in the following:

Here we want to copy all the orders before 2019 into the table orders_archived: We can use the SELECT statement as a subquery to the INSERT statement:

        USE sql_store;
        INSERT INTO orders_archived 
        SELECT *
        FROM orders
        WHERE order_date <  ‘2019-01-01’
        Exercise:
        
        USE sql_invoicing;
        CREATE TABLE invoice_archived AS 
        SELECT 
            i.invoice_id,
            i.number,
            c.name AS client,
            i.invoice_total, 
            i.payment_total,
            i.invoice_date,
            i.payment_date,
            i.due_date
        FROM clients c
        JOIN invoices i USING (client_id) 
        WHERE payment_date IS NOT NULL 
Note:

Because the columns invoice_date, payment_date and due_date only exist in invoices table we don’t need to prefix their names in the SELECT statement but MOSH prefers to do so to make his query more clear.

<a name="39"></a>
#### Updating a Single Row

We use UPDATE statement to update one or more records in a table, which table? the one in front of it! In the SET clause we specify the new value for one or more columns (we use a comma to add more columns) then we use WHERE to identify the condition to get the record we would like to update:

        USE sql_invoicing;
        UPDATE invoices 
        SET
            payment_total = 0.5 * total_invoice,
            payment_date = due_date 
        WHERE invoice_id = 3 
        
<a name="40"></a>
#### Updating Multiple Rows

This is exactly the same as updating a single row, as above, but we need a more general condition in the WHERE clause:

        USE sql_invoicing;
        UPDATE invoices
        SET
            payment_total = 0.5 * total_invoice,
            payment_date = due_date 
        WHERE client_id = 3 -- all the operators you learned to use in WHERE clause also apply here like WHERE client_id IN (3, 4) 

The WHERE clause above is optional and if you want to update all the records in a table you can simply leave the WHERE clause out.

But if we run the above query we get an error, this is the case because MySQL Workbench yells at us because Workbench allows us to update only a single record (this is specific to Workbench and if I use other clients for MySQL I may not get this error, also I connected to a MySQL Database with Python (Pandas) and executing pure SQL Queries I did not get this issue) to fix this we go to

Edit > preferences > SQL editor > uncheck safe updates …

Now we close and reconnect to the database and now it works.

Exercise:

        USE sql_store,
        UPDATE customers
        SET
            Points = points + 50
        WHERE birth_date < ‘1990-01-01’ -- anyone born before 1990 
                
<a name="41"></a>
#### Using Subqueries in Updates

Running the following query, what if we don’t have the client_id and we only have the name of the client?

        USE sql_invoicing;
        UPDATE invoices
        SET
            payment_total = 0.5 * total_invoice,
            payment_date = due_date 
        WHERE client_id = 3

For example, imagine you have an application and the user types in the client name in that application so first we should find the client_id and then use that ID to update all their invoices.

To do so we use a subquery to get the client_id based on the name rather than hard coding the client_id like:

        USE sql_invoicing;
        UPDATE invoices
        SET
            payment_total = 0.5 * total_invoice,
            payment_date = due_date 
        WHERE client_id = 
            (SELECT client_id
            FROM clients
            WHERE name = ‘Myworks’)
    
This will update all the invoices for this client.

Pay attention we need to put the subquery in the parenthesis.

What if our subquery in the parenthesis above returns multiple clients? When this is the case we need to use IN instead of the equal sign in the WHERE clause:

        USE sql_invoicing;
        UPDATE invoices
        SET
            payment_total = 0.5 * total_invoice,
            payment_date = due_date 
        WHERE client_id IN
            (SELECT client_id
            FROM clients
            WHERE state IN (‘CA’, ‘NY’))
    
As a best practice before executing your update statement run your subquery, to see what records you are going to update so you don’t accidentally update the records that shouldn't be updated. In the above, we have a subquery but even if we did not have a subquery we could still query the records that we want to update like:

UPDATE invoices SET payment_total = 0.5 * total_invoice, payment_date = due_date WHERE payment_date IS NULL

before running the above query, I would run the following:

        SELECT *
        From INVOICES 
        WHERE payment_date IS NULL 

Then when we are confident that we will be updating the right records as we run our query to update them.

Exercise:

        USE sql_store;
        UPDATE orders
        SET comments = ‘Golden customer’
        WHERE customer_id IN 
                        (SELECT customer_id
                        FROM customers
                        WHERE points > 3000)
                        
<a name="42"></a>
#### Deleting rows

If we don’t provide the optional WHERE clause here all the data in the table will be deleted, which is obviously very dangerous so be very careful:

        DELETE FROM invoices
        WHERE invoice_id = 1 

Also, we can use subqueries in the WHERE clause:
        
        DELETE FROM invoices
        WHERE client_id = (
                SELECT client_id
                FROM clients
                WHERE name = ‘Myworks’)
        
<a name="43"></a>
### Summarizing Data

We will learn how to write queries that summarize data. This section is extremely important specially if you work with lots of data.

<a name="44"></a>
#### Aggregate functions

These functions take a series of values and aggregate them to produce a single value for example MAX () returns the maximum in a series of values. Like

        USE sql_invoicing;
        SELECT MAX(invoice_total)
        FROM invoices

The name of the returned column is set to the expression we used, in this case it is MAX(invoice_total) let’s be more meaningful:

        USE sql_invoicing;
        SELECT MAX(invoice_total) AS highest 
        FROM invoices

In the same query we can also calculate the minimum, average, sum, and count:

        USE sql_invoicing;
        SELECT
        MAX(invoice_total) AS highest, 
        MIN(invoice_total) AS lowest,
        AVG(invoice_total) AS average,
        SUM(invoice_total) AS total,
        COUNT(invoice_total) AS number_of_invoices 
        FROM invoices

Above we apply these functions on columns with numeric values but also we can apply them to the columns with dates and strings:

        USE sql_invoicing;
        SELECT
        MAX(payment_date) AS highest, 
        FROM invoices

The above query returns the latest date that we received the payment.

POINT: the aggregate functions ONLY operate on NON NULL values. And if you have a NULL value in your columns it is not going to be included in these functions’ calculations.

If you want to get the total number in your tables irrespective of the NULL values you have to use COUNT(*) meaning it counts all the rows, including those with NULL values, and returns a single value representing the count.

Most of the times we use a column name inside the parenthesis in front of the aggregate functions but we also can write an expression like:

        SELECT
            MAX(invoice_total) AS highest, 
            MIN(invoice_total) AS lowest,
            AVG(invoice_total) AS average,
            SUM(invoice_total * 1.1) AS total,
            COUNT(invoice_total) AS number_of_invoices 
        FROM invoices

Also if you have a filter, the calculations would be based on the filtered results that match the certain criteria:

        SELECT
            MAX(invoice_total) AS highest, 
            MIN(invoice_total) AS lowest,
            AVG(invoice_total) AS average,
            SUM(invoice_total * 1.1) AS total,
            COUNT(invoice_total) AS number_of_invoices 
        FROM invoices
        WHERE invoice_date > ‘2019-07-01’

Point: by default, all these aggregate functions mentioned above take duplicate values and if you want to exclude duplicates you have to use the DISTINCT keyword like:

        SELECT
            MAX(invoice_total) AS highest, 
            MIN(invoice_total) AS lowest,
            AVG(invoice_total) AS average,
            SUM(invoice_total * 1.1) AS total,
            COUNT(DISTINCT client_id) AS total_records 
        FROM invoices
        WHERE invoice_date > ‘2019-07-01’

<a name="45"></a>
#### The GROUP BY Clause

        USE sql_invoicing;
        SELECT
            Client_id,
            SUM(invoice_total) AS total_sales
        FROM invoices
        GROUP BY client_id
        ORDER BY total_sales DESC 

By default, our data would be sorted by the column in the GROUP BY clause but we can change it by the ORDER BY clause, as above.

We can also apply a filter before grouping our data:

        USE sql_invoicing;
        SELECT 
            client_id,
            SUM(invoice_total) AS total_sales 
        FROM invoices 
        WHERE invoice_date >= ‘2019-07-01’
        GROUP BY client_id 
        ORDER BY total_sales DESC 

So here we can group data based on a single column.

Pay attention to the order of the above clauses FIRST SELECT, then FROM, then optionally WHERE, then GROUP BY, then ORDER BY. The GROUP BY clause always comes after the FROM and WHERE clauses and BEFORE ORDER BY.

How to group data based on multiple columns:

        SELECT 
            state,
            city,
            SUM(invoice_total) AS total_sales
        FROM invoices
        JOIN clients USING (client_id)
        GROUP BY state, city

We get one record for each state-city combination.

Exercise:

        USE sql_invoicing;
        SELECT
            data,
            pm.name AS payment_method, 
            SUM(amount) AS total_payments 
        FROM payments p
        JOIN payment_methods pm -- so I cannot use USING clause! 
            ON p.payment_method = pm.payment_method_id 
        GROUP BY date, payment_method
        ORDER BY date 

<a name="46"></a>
#### The HAVING Clause

If we want to filter the results after grouping our rows we have to use HAVING clause and NOT WHERE clause. Like:

        SELECT 
            client_id,
            SUM(invoice_total) AS total_sales 
        FROM invoices 
        GROUP BY client_id 
        HAVING total_sales > 500 

So with WHERE clause we can filter data before our rows are grouped, while with HAVING clause we can filter data after our rows are grouped. That is the difference between WHERE and HAVING clauses.

POINT: In a HAVING clause we can have a compound search condition (just like the WHERE clause) BUT the columns that we use in HAVING clause should be part of our SELECT clause. In contrast, when writing a WHERE clause we can reference any columns whether or not they are included in the SELECT clause.

like:

        SELECT 
            client_id,
            SUM(invoice_total) AS total_sales,
            COUNT (*) AS number_of_invoices 
        FROM invoices 
        GROUP BY client_id 
        HAVING total_sales > 500 AND number_of_invoices > 5

Exercise:

Get the customers who are located in ‘VA’ and have spent more than $100:

Solution:

        USE sql_store;
        SELECT 
            c.customer_id,
            c.first_name,
            c.last_name,
            SUM (oi.quantity * oi.unit_price) AS total_sales 
        FROM customers c 
        JOIN orders o USING (customer_id)
        JOIN order_items oi USING (order_id)
        WHERE state = ‘VA’
        GROUP BY 
            c.customer_id,
            c.first_name,
            c.last_name
        HAVING toal_Sales > 100

As a rule of thumb when we have an aggregate function in the SELECT statement and we want to group our data we should group by all the columns in the SELECT clause.

<a name="47"></a>
#### The ROLLUP Operator

Only available in MySQL (and not part of standard SQL language, so I won't be able to execute it in SQL server or oracle), which summarizes our entire results set with one extra row. The ROLLUP operator only applies to the columns that aggregate values.

        con = connector('sql_invoicing')
        pd.read_sql("""
        SELECT 
            client_id,
            SUM(invoice_total) AS total_sales
        FROM invoices
        GROUP BY client_id WITH ROLLUP
        """, con)
        
        client_id	total_sales
        0	1.0	802.89
        1	2.0	101.79
        2	3.0	705.90
        3	5.0	980.02
        4	NaN	2590.60

What if we GROUP BY multiple columns:

        pd.read_sql("""
        SELECT 
            state, 
            city, 
            SUM(invoice_total) AS total_sales
        FROM invoices
        JOIN clients c USING (client_id)
        GROUP BY state, city WITH ROLLUP
        """, con)
        
        state	city	total_sales
        0	CA	San Francisco	705.90
        1	CA	None	705.90
        2	NY	Syracuse	802.89
        3	NY	None	802.89
        4	OR	Portland	980.02
        5	OR	None	980.02
        6	WV	Huntington	101.79
        7	WV	None	101.79
        8	None	None	2590.60

So when GROUP BY multiple columns, we get an extra row for each grouop and also one extra row at the end for the entire results set, as above.

Exercise:

        pd.read_sql("""
        SELECT 
            pm.name AS payment_method,
            SUM(amount) AS total
        FROM payments p
        JOIN payment_methods pm
            ON p.payment_method = pm.payment_method_id
        GROUP BY pm.name WITH ROLLUP 
        """, con)

        payment_method	total
        0	Cash	10.00
        1	Credit Card	351.38
        2	None	361.38

When we use a ROLLUP operator we cannot use a column alias in the GROUP BY clause so the following won't work:

        GROUP BY payment_method WITH ROLLUP

<a name="48"></a>
### Writing a complex query

<a name="49"></a>
#### Subqueries

        con = connector('sql_store')
        pd.read_sql("""
        SELECT *
        FROM products
        WHERE unit_price > (
                    SELECT unit_price
                    FROM products
                    WHERE product_id=3)
        """, con)
        
        product_id	name	quantity_in_stock	unit_price
        0	2	Pork - Bacon,back Peameal	49	4.65
        1	4	Brocolinni - Gaylan, Chinese	90	4.53

<a name="50"></a>
#### Subqueries vs. JOINs

We can achieve the same results using either subquery or JOIN:

The readability and performance determine which way to go! Later, we talk about execution plans where we learn how to write a query that executes faster. But here, let's assume both queries (i.e., the one using subqueries and the one using JOIN execute similarly in terms of speed) then we pay attention to the readability.

Using subquery:

        pd.read_sql("""
        SELECT *
        FROM clients
        WHERE client_id NOT IN(
                SELECT DISTINCT client_id
                FROM invoices
        )
        """, con)
        
        client_id	name	address	city	state	phone
        0	4	Kwideo	81674 Westerfield Circle	Waco	TX	254-750-0784
        And using JOIN:
        
        pd.read_sql("""
        SELECT *
        FROM clients
        LEFT JOIN invoices USING (client_id)
        WHERE invoice_id IS NULL
        """, con)

        client_id	name	address	city	state	phone	invoice_id	number	invoice_total	payment_total	invoice_date	due_date	payment_date
        0	4	Kwideo	81674 Westerfield Circle	Waco	TX	254-750-0784	None	None	None	None	None	None	None

In this particular example using subqueries makes our query more readable, which is not always true, and sometimes using subqueries makes queries complicated and it is better to go with JOIN! So always pay great attention to the readability of your code.

<a name="51"></a>
#### ALL

solution using ALL:

Here the subquery returns a list:

        pd.read_sql("""
        SELECT *
        FROM invoices
        WHERE invoice_total > ALL (
                    SELECT invoice_total
                    FROM invoices
                    WHERE client_id = 3
        
                    )
        """, con)
        
        invoice_id	number	client_id	invoice_total	payment_total	invoice_date	due_date	payment_date
        0	2	03-898-6735	5	175.32	8.18	2019-06-11	2019-07-01	2019-02-12
        1	5	87-052-3121	5	169.36	0.00	2019-07-18	2019-08-07	None
        2	8	78-145-1093	1	189.12	0.00	2019-05-20	2019-06-09	None
        3	9	77-593-0081	5	172.17	0.00	2019-07-09	2019-07-29	None
        4	18	52-269-9803	5	180.17	42.77	2019-05-23	2019-06-12	2019-01-08
        solution using MAX():

Here my subquery returns a single value:

        pd.read_sql("""
        SELECT *
        FROM invoices
        WHERE invoice_total > (
                    SELECT MAX(invoice_total)
                    FROM invoices
                    WHERE client_id = 3
                    )
        """, con)
        
        invoice_id	number	client_id	invoice_total	payment_total	invoice_date	due_date	payment_date
        0	2	03-898-6735	5	175.32	8.18	2019-06-11	2019-07-01	2019-02-12
        1	5	87-052-3121	5	169.36	0.00	2019-07-18	2019-08-07	None
        2	8	78-145-1093	1	189.12	0.00	2019-05-20	2019-06-09	None
        3	9	77-593-0081	5	172.17	0.00	2019-07-09	2019-07-29	None
        4	18	52-269-9803	5	180.17	42.77	2019-05-23	2019-06-12	2019-01-08

Both queries above (the one using MAX() and the one using ALL) are readable, so go with the one you like more!

Sometimes our subquery returns a single value, sometimes it returns a list, sometimes returns a table.

<a name="52"></a>
#### ANY or SOME (they are equivalent

        pd.read_sql("""
        SELECT *
        FROM clients
        WHERE client_id IN (
                SELECT client_id
                FROM invoices
                GROUP BY client_id
                HAVING COUNT(*) >=2
        )
        
        """, con)
        
        client_id	name	address	city	state	phone
        0	1	Vinte	3 Nevada Parkway	Syracuse	NY	315-252-7305
        1	3	Yadel	096 Pawling Parkway	San Francisco	CA	415-144-6037
        2	5	Topiclounge	0863 Farmco Road	Portland	OR	971-888-9129

another way to write the above query:

        pd.read_sql("""
        SELECT *
        FROM clients
        WHERE client_id = ANY (
                SELECT client_id
                FROM invoices
                GROUP BY client_id
                HAVING COUNT(*) >=2
        )
        
        """, con)
        
        client_id	name	address	city	state	phone
        0	1	Vinte	3 Nevada Parkway	Syracuse	NY	315-252-7305
        1	3	Yadel	096 Pawling Parkway	San Francisco	CA	415-144-6037
        2	5	Topiclounge	0863 Farmco Road	Portland	OR	971-888-9129

(= ANY) is equivalent to (IN) (choose what you prefer, it is up to you)

<a name="53"></a>
#### Correlated Subqueries

In correlated subqueries, we have a correlation with the outer query, like we are referencing the alias from the outer query.

        pd.read_sql("""
        SELECT *
        FROM employees e
        WHERE salary > (
                    SELECT AVG(salary)
                    FROM employees
                    WHERE office_id = e.office_id
                    )
        """, con)
        
        employee_id	first_name	last_name	job_title	salary	reports_to	office_id
        0	37851	Sayer	Matterson	Statistician III	98926	37270	1
        1	40448	Mindy	Crissil	Staff Scientist	94860	37270	1
        2	56274	Keriann	Alloisi	VP Marketing	110150	37270	1
        3	67009	North	de Clerc	VP Product Management	114257	37270	2
        4	67370	Elladine	Rising	Social Worker	96767	37270	2
        5	72540	Guthrey	Iacopetti	Office Assistant I	117690	37270	3
        6	76196	Mirilla	Janowski	Cost Accountant	119241	37270	3
        7	84791	Hazel	Tarbert	General Manager	93760	37270	4
        8	95213	Cole	Kesterton	Pharmacist	86119	37270	4
        9	98374	Estrellita	Daleman	Staff Accountant IV	70187	37270	5
        10	115357	Ivy	Fearey	Structural Engineer	92710	37270	5

<a name="54"></a>
#### EXISTS

Takeaway:

When we use IN operator MySQL executes the subquery and returns the results to the WHERE clause, which in our case is a list of 4 client_id. What if I have millions of elements in this list? negative effect on the performance and in these situations I need to use EXISTS operator, where the subquery does not return a result to the outer query and instead it returns an indication of whether any rows in the subquery match the serach condition! This enhances performance.

So if the subquery we write after the IN operator produces a large result set, it is more efficient to use EXISTS operator.

        pd.read_sql("""
        SELECT *
        FROM products p
        WHERE NOT EXISTS (
                SELECT DISTINCT product_id
                FROM order_items
                WHERE product_id = p.product_id
                )
        """, con)
        
        product_id	name	quantity_in_stock	unit_price
        0	7	Sweet Pea Sprouts	98	3.29

<a name="55"></a>
#### Subqueries in the SELECT clause

So far we only used subqueries in the WHERE clause of a SELECT clause, we can also use subqueries in the SELECT clase and also FROM clause.

        pd.read_sql("""
        SELECT 
            invoice_id,
            invoice_total,
            (
                SELECT AVG(invoice_total)
                FROM invoices 
            ) AS invoice_average,
            invoice_total - (
                SELECT AVG(invoice_total)
                FROM invoices 
            ) AS invoice_dif
        FROM invoices
        """, con)

        invoice_id	invoice_total	invoice_average	invoice_dif
        0	1	101.79	152.388235	-50.598235
        1	2	175.32	152.388235	22.931765
        2	3	147.99	152.388235	-4.398235
        3	4	152.21	152.388235	-0.178235
        4	5	169.36	152.388235	16.971765
        5	6	157.78	152.388235	5.391765
        6	7	133.87	152.388235	-18.518235
        7	8	189.12	152.388235	36.731765
        8	9	172.17	152.388235	19.781765
        9	10	159.50	152.388235	7.111765
        10	11	126.15	152.388235	-26.238235
        11	13	135.01	152.388235	-17.378235
        12	15	167.29	152.388235	14.901765
        13	16	162.02	152.388235	9.631765
        14	17	126.38	152.388235	-26.008235
        15	18	180.17	152.388235	27.781765
        16	19	134.47	152.388235	-17.918235

above query is repetitive and better idea is as follows

        pd.read_sql("""
        SELECT 
            invoice_id,
            invoice_total,
            (
                SELECT AVG(invoice_total)
                FROM invoices 
            ) AS invoice_average,
            invoice_total - (SELECT invoice_average) AS invoice_dif
        FROM invoices
        """, con)
        
        invoice_id	invoice_total	invoice_average	invoice_dif
        0	1	101.79	152.388235	-50.598235
        1	2	175.32	152.388235	22.931765
        2	3	147.99	152.388235	-4.398235
        3	4	152.21	152.388235	-0.178235
        4	5	169.36	152.388235	16.971765
        5	6	157.78	152.388235	5.391765
        6	7	133.87	152.388235	-18.518235
        7	8	189.12	152.388235	36.731765
        8	9	172.17	152.388235	19.781765
        9	10	159.50	152.388235	7.111765
        10	11	126.15	152.388235	-26.238235
        11	13	135.01	152.388235	-17.378235
        12	15	167.29	152.388235	14.901765
        13	16	162.02	152.388235	9.631765
        14	17	126.38	152.388235	-26.008235
        15	18	180.17	152.388235	27.781765
        16	19	134.47	152.388235	-17.918235

<a name="56"></a>
#### Subqueries in the FROM clause

Whenever we use a subquery in a FROM clause we HAVE to give the subquery an alias whether ot not we use that alias. This is required.

Writing subqueries in the FROM clause of a SELECT statement may make our main query more complex, there is a better way to solve this problem using views, we can take this subquery and store it in our database as a view then we can call that view, we look at it later.

Takeaway: You can write a subquery in the FROM clause of the SELECT statement, but reserve it ONLY for simple queries.

        pd.read_sql("""
        SELECT *
        FROM(
            SELECT 
                client_id,
                name,
                (SELECT SUM(invoice_total)
                FROM invoices
                WHERE client_id = c.client_id) AS total_sales,
                (SELECT AVG(invoice_total) FROM invoices) AS average,
                (SELECT total_sales - average) AS difference
            FROM clients c
        ) AS sales_summary
        WHERE total_sales IS NOT NULL
        """, con)
        
        client_id	name	total_sales	average	difference
        0	1	Vinte	802.89	152.388235	650.501765
        1	2	Myworks	101.79	152.388235	-50.598235
        2	3	Yadel	705.90	152.388235	553.511765
        3	5	Topiclounge	980.02	152.388235	827.631765
   
<a name="57"></a>
### Essential MySQL Functions 

<a name="58"></a>
#### NUMERIC Function

        ROUND
        TRUNCATE
        CEILING
        FLOOR
        ABS
        RAND
        
https://dev.mysql.com/doc/refman/8.0/en/numeric-functions.html

<a name="59"></a>
#### STRING Functions

        LENGTH
        LOWER
        UPPER
        LTRIM
        RTRIM
        TRIM
        LEFT
        RIGHT
        SUBSTRING
        LOCATE
        REPLACE
        CONCAT

https://dev.mysql.com/doc/refman/8.0/en/string-functions.html

<a name="60"></a>
#### DATE Functions

        NOW
        CURDATE
        CURTIME
        YEAR
        MONTH
        DAY
        HOUR
        MINUTE
        SECOND
        DAYNAME
        MONTHNAME
        EXTRACT
        DATEDIFF

https://dev.mysql.com/doc/refman/8.0/en/date-and-time-functions.html

<a name="61"></a>
#### FORMATTING Date and Times

        DATE_FORMAT
    
        https://dev.mysql.com/doc/refman/8.0/en/date-and-time-functions.html

        TIME_FORMAT

<a name="62"></a>
#### CALCULATING Dates and Times

        DATE_ADD
        DATE_SUB
        DATEDIFF
        TIME_TO_SEC

<a name="63"></a>
#### IFNULL and COALESCE Functions

        pd.read_sql("""
        SELECT 
            order_id,
            IFNULL(shipper_id, 'Not assigned') AS shipper
        FROM orders""", con)
        order_id	shipper
        0	1	Not assigned
        1	3	Not assigned
        2	4	Not assigned
        3	6	Not assigned
        4	8	Not assigned
        5	9	1
        6	10	2
        7	5	3
        8	2	4
        9	7	4

        pd.read_sql("""
        SELECT 
            order_id,
            COALESCE(shipper_id, comments, 'Not assigned') AS shipper
        FROM orders""", con)
        order_id	shipper
        0	1	Not assigned
        1	2	4
        2	3	Not assigned
        3	4	Not assigned
        4	5	3
        5	6	Aliquam erat volutpat. In congue.
        6	7	4
        7	8	Mauris enim leo, rhoncus sed, vestibulum sit a...
        8	9	1
        9	10	2

<a name="64"></a>
#### IF Function

        pd.read_sql("""
        SELECT 
            order_id,
            customer_id,
            'Active' AS status
        FROM orders
        WHERE order_date >= '2019-01-01'
        
        UNION
        SELECT 
             order_id,
            customer_id,
            'Archived' AS status
        FROM orders
        WHERE order_date < '2019-01-01'
        
        """, con)
        order_id	customer_id	status
        0	1	6	Active
        1	2	7	Archived
        2	3	8	Archived
        3	4	2	Archived
        4	5	5	Archived
        5	6	10	Archived
        6	7	2	Archived
        7	8	5	Archived
        8	9	10	Archived
        9	10	6	Archived
        
Using IF function I achieved the same results as above but with much shorted query:

        pd.read_sql("""
        SELECT 
            order_id,
            customer_id, 
            IF (order_date >= '2019-01-01', 'Active', 'Archived') AS status
        FROM orders
        """, con)
        order_id	customer_id	status
        0	1	6	Active
        1	2	7	Archived
        2	3	8	Archived
        3	4	2	Archived
        4	5	5	Archived
        5	6	10	Archived
        6	7	2	Archived
        7	8	5	Archived
        8	9	10	Archived
        9	10	6	Archived
        
<a name="65"></a>
#### CASE Operator
        pd.read_sql("""
        SELECT 
            CONCAT(first_name, ' ', last_name) AS customer,
            points,
            CASE
                WHEN points < 2000 THEN 'Bronze'
                WHEN points BETWEEN 2000 AND 3000 THEN 'Silver'
                WHEN points > 3000 THEN 'Gold'
            END AS category
        FROM customers
        """, con)
        
        customer	points	category
        0	Babara MacCaffrey	2273	Silver
        1	Ines Brushfield	947	Bronze
        2	Freddi Boagey	2967	Silver
        3	Ambur Roseburgh	457	Bronze
        4	Clemmie Betchley	3675	Gold
        5	Elka Twiddell	3073	Gold
        6	Ilene Dowson	1672	Bronze
        7	Thacher Naseby	205	Bronze
        8	Romola Rumgay	1486	Bronze
        9	Levy Mynett	796	Bronze

<a name="66"></a>
### VIEWS

<a name="67"></a>
#### Creating Views

Sometimes our queries get complex specially when we have multiple JOINs and subqueries, this is where VIEWS come to rescuse, we can save these queries or subqueries in a view, then we can reuse those views later with no need to rewrite those queries or subqueries again. We can create view using:

        cursor = con.cursor()
        
        cursor.execute("""
        CREATE VIEW sales_by_client AS
        SELECT 
            c.client_id,
            c.name,
            SUM(invoice_total) AS total_sales
        FROM clients c
        JOIN invoices USING (client_id)
        GROUP BY client_id, name
        
        """)
        
        con.commit()
        cursor.close()
        
I can reuse this view and select data from it just like a table like:

        pd.read_sql("""
        SELECT *
        FROM sales_by_client
        """, con)
        client_id	name	total_sales
        0	2	Myworks	101.79
        1	5	Topiclounge	980.02
        2	3	Yadel	705.90
        3	1	Vinte	802.89

we can use it just like a table like doing ORDER BY:

        pd.read_sql("""
        SELECT *
        FROM sales_by_client
        ORDER BY total_sales DESC
        """, con)
        client_id	name	total_sales
        0	5	Topiclounge	980.02
        1	1	Vinte	802.89
        2	3	Yadel	705.90
        3	2	Myworks	101.79

or filtering:

        pd.read_sql("""
        SELECT *
        FROM sales_by_client
        WHERE total_sales > 500
        """, con)
        client_id	name	total_sales
        0	5	Topiclounge	980.02
        1	3	Yadel	705.90
        2	1	Vinte	802.89

or JOIN it with any other tables we have:

        pd.read_sql("""
        SELECT *
        FROM sales_by_client
        JOIN clients USING (client_id)
        """, con)
        client_id	name	total_sales	name	address	city	state	phone
        0	1	Vinte	802.89	Vinte	3 Nevada Parkway	Syracuse	NY	315-252-7305
        1	2	Myworks	101.79	Myworks	34267 Glendale Parkway	Huntington	WV	304-659-1170
        2	3	Yadel	705.90	Yadel	096 Pawling Parkway	San Francisco	CA	415-144-6037
        3	5	Topiclounge	980.02	Topiclounge	0863 Farmco Road	Portland	OR	971-888-9129

So VIEWS are extremely powerful and can greatly simplify our future queries.

VIEWS behaves like virtual tables BUT remember VIEWS don't store data, our data is actually stored in tables, a view just provides a view to the underlying tables, that is why we call it view.

<a name="68"></a>
#### Altering or Dropping VIEWS

If we want to modify our VIEW after we already created it, we have 2 options:

1- Drop it then recreate it like:

        def delete_view (database, view_name):
        
            con = connector(database)
            cursor = con.cursor()
        
            cursor.execute(f"DROP VIEW {view_name}")
        
            # Commit the transaction
            con.commit()
        
            # Close the connection
            con.close()
            
2- using CREATE OR REPLACE keyword (this method is a preferred way)

        cursor = con.cursor()
        
        cursor.execute("""
        
        CREATE OR REPLACE VIEW clients_balance AS
        SELECT 
            c.client_id,
            c.name,
            SUM(invoice_total - payment_total) AS balance 
        FROM clients c
        JOIN invoices i
            USING (client_id)
        GROUP BY client_id, name 
        ORDER BY balance DESC
        """)

        con.commit()
        cursor.close()

What if the query in the view is gone and you don't have access to it anymore?

The ideal way is to save your view as a sql file and then put it under the source control, very common and great practice is to check these files into your Git repository and then share that repository with other people allowing others to recreate the database on their own machines.

<a name="69"></a>
#### Updating VIEWS

So far we used our views in SELECT statements, but also we can use them in INSERT, UPDATE, and DELETE statements, BUT ONLY IF the view is updatable meaning not having any of the followings in it:

        DISTINCT
        Aggregare Functions (MIN, MAX, SUM ...)
        GROUP BY/HAVING
        UNION

Here are the examples for DELETING and UPDATING an updatable view:

        cursor = con.cursor()
        
        cursor.execute("""
        CREATE OR REPLACE VIEW invoices_with_balance AS
        SELECT 
            invoice_id,
            number,
            client_id,
            invoice_total,
            payment_total,
            invoice_total - payment_total AS balance, 
            invoice_date,
            due_date,
            payment_date
        FROM invoices
        WHERE (invoice_total - payment_total) > 0
        """)
        
        con.commit()
        cursor.close()

Since in my view above i don't have DISTINCT keyword, or using any aggregate functions or groupby or union so my view is UPDATABLE!

        cursor = con.cursor()
        
        cursor.execute("""
        DELETE FROM invoices_with_balance
        WHERE invoice_id = 1
        
        """)
        
        con.commit()
        cursor.close()

or i can UPDATE it:

        cursor = con.cursor()
        
        cursor.execute("""
        UPDATE invoices_with_balance
        SET due_date = DATE_ADD(due_date, INTERVAL 2 DAY)
        WHERE invoice_id = 2
        """)
        
        con.commit()
        cursor.close()

The INSERT is a bit tricky because it only works if the view has all the required columns in the underlying table.

Most of the time we update data through our tables but in some cases we may not have direct permission to the table for securing reasons so our only option is to modify data through a view, in these cases we use views to delete, update, or insert data assuming our view is updatable.

<a name="70"></a>
#### The WITH CHECK OPTION clause

The default behavior of view is that when you UPDATE data through a view some of the rows may disappear. There are times that you want to prevent this: you don't want the UPDATE statement to exclude a row from the VIEW, you can do this with WITH CHECK OPTION at the end of your VIEW, like:

        cursor = con.cursor()
        
        cursor.execute("""
        CREATE OR REPLACE VIEW invoices_with_balance AS
        SELECT 
            invoice_id,
            number,
            client_id,
            invoice_total,
            payment_total,
            invoice_total - payment_total AS balance, 
            invoice_date,
            due_date,
            payment_date
        FROM invoices
        WHERE (invoice_total - payment_total) > 0
        WITH CHECK OPTION
        
        """)

        con.commit()
        cursor.close()

So now if I try to update a view which results in exclusion of any row I get an error like:

        cursor = con.cursor()
        
        cursor.execute("""
        UPDATE invoices_with_balance
        SET payment_total = invoice_total
        WHERE invoice_id = 3
        
        """)
        
        con.commit()
        cursor.close()
        OperationalError: (1369, "CHECK OPTION failed 'sql_invoicing.invoices_with_balance'")

<a name="71"></a>
#### Other benefits of VIEWS

VIEWS's benefits:

+ Simply our queries
+ Reduce the impact of changes in the database design
+ Restrict access to the data in the underlying tables

<a name="72"></a>
### Stored Procedures and Functions

<a name="73"></a>
#### What Stored Procedures are

Where you are building an application that has a database, whare you are going to write these SQL statements?

In your application code? NO, because it makes your application code messy and hard to maintain. So we keep our SQL code inside the Stored procedures or function.

A stored procedures is a database object that contains a block of SQL code. In our application code we simply call these procedures to get or save the data

Stored procedures benefits:

+ Store and organize SQL code
+ Faster execution
+ Data security

<a name="74"></a>
#### Creating a Stored Procedure

We can create a stored procedure like:

        cursor = con.cursor()
        
        #cursor.execute("DELIMITER $$") # I DO NOT NEED THIS WHEN USING PYTHON
        
        cursor.execute("""
        
        CREATE PROCEDURE get_clients()
        
        BEGIN 
            SELECT * FROM clients; 
        END
        
        """)
        # cursor.execute("DELIMITER ;") # I DO NOT NEED THIS WHEN USING PYTHON 

        con.commit()
        cursor.close()

Some points:

The common convention among MySQL developers: use lowercase letters and separate words using underscore when naming your stored procedure

What we have in between the BEGIN and the END is called the body of the procedure.

In MySQL we need to terminate each statement in the body of the stored procedure using a semicolon (even if we have only one single statement in the body), this is specific to MySQL.

We need to change the default DELIMITER, by convention, people use $$, we need this to indicate all the statements should be considered as one single unit, rather than individual statements using a semicolon (i mean the statements in the body of the stored procedures). W need to repeat this new DELIMITER after END, after that we need to change the default DELIMITER to the semicolon again (in other database management system like SQL server we don't have to change the default delimiter (also in my case when I am connecting to the MySQL Database with Python (Pandas) I DONOT NEED TO CHANGE THIS DEFAULT DELIMITER). Here is the code to change the default delimiter:

          DELIMITER $$
                CREATE PROCEDURE get_clients()
                BEGIN
                    SELECT * FROM clients
                END $$

          DELIMITER ; 

I also can use one of my views to create the stored procedure, this is better because I also can see the balance column

        cursor = con.cursor()
        
        cursor.execute("""
        
        CREATE PROCEDURE get_invoices_with_balance_from_view ()
        
        BEGIN
          SELECT *
          FROM invoices_with_balance 
          WHERE balance > 0; 
        END
        """)

        con.commit()
        cursor.close()
We can call the stored procedure using CALL statement. We mostly call the stored procedures in our application code in python for example, but if we want to call it in SQL code we do it like

        CALL get_clients()

In my case in Python:

        pd.read_sql("""
        CALL get_invoices_with_balance_from_view ()
        """, con)

    
<a name="75"></a>
#### Dropping Stored Procedures

Here is my function to drop the stored procedure:

        def delete_stored_procedure(database, stored_procedure_name):
        
            con = connector(database)
            cursor = con.cursor()
        
            cursor.execute(f"DROP PROCEDURE IF EXISTS {stored_procedure_name}")
        
            # Commit the transaction
            con.commit()
        
            # Close the connection
            con.close()

Note: I added IF EXISTS to prevent raising errors in case there is no stored procedure with the name we specified to be dropped.

<a name="76"></a>
#### Parameters

We typically use a parameter to pass a value to the stored procedure.

        cursor = con.cursor()
        
        cursor.execute("DROP PROCEDURE IF EXISTS get_clients_by_state")
        
        cursor.execute("""
        
        CREATE PROCEDURE get_clients_by_state 
        (
        state CHAR(2)
        )
        BEGIN
            SELECT *
            FROM clients c
            WHERE c.state = state; 
        END
        """)
        
        con.commit()
        cursor.close()

        pd.read_sql("""
        CALL get_clients_by_state('CA')
        """, con)
        
        client_id	name	address	city	state	phone
        0	3	Yadel	096 Pawling Parkway	San Francisco	CA	415-144-6037
        

<a name="77"></a>
#### Parameters with Default Value
        
        Here is the code:
        
        cursor = con.cursor()
        
        cursor.execute("DROP PROCEDURE IF EXISTS get_clients_by_state")

        cursor.execute("""
        CREATE PROCEDURE get_clients_by_state
        (
        state CHAR(2)
        )
        BEGIN
            IF state IS NULL THEN
                SET state = 'CA';
            END IF;   **Whenever we use **IF statement** we should terminate it with **END IF;**.**
        
            SELECT *
            FROM clients c
            WHERE c.state = state; 
        END
        """)

        con.commit()
        cursor.close()
        
        pd.read_sql("""
        CALL get_clients_by_state ('CA')
        """, con)
        
        client_id	name	address	city	state	phone
        0	3	Yadel	096 Pawling Parkway	San Francisco	CA	415-144-6037

another example:

        cursor = con.cursor()
        
        cursor.execute("DROP PROCEDURE IF EXISTS get_clients_by_state")
        
        cursor.execute("""
        
        CREATE PROCEDURE get_clients_by_state
        (
        state CHAR(2)
        )
        BEGIN
            IF state IS NULL THEN
                SELECT * FROM clients;
            ELSE 
                SELECT * FROM clients c 
                WHERE c.state = state; 
            END IF; 
        END
        
        """)
        
        con.commit()
        cursor.close()
        
        pd.read_sql("""
        CALL get_clients_by_state(NULL)
        """, con)
        
            client_id	name	address	city	state	phone
        0	1	Vinte	3 Nevada Parkway	Syracuse	NY	315-252-7305
        1	2	Myworks	34267 Glendale Parkway	Huntington	WV	304-659-1170
        2	3	Yadel	096 Pawling Parkway	San Francisco	CA	415-144-6037
        3	4	Kwideo	81674 Westerfield Circle	Waco	TX	254-750-0784
        4	5	Topiclounge	0863 Farmco Road	Portland	OR	971-888-9129
        
        pd.read_sql("""
        CALL get_clients_by_state('CA')
        """, con)
        
        client_id	name	address	city	state	phone
        0	3	Yadel	096 Pawling Parkway	San Francisco	CA	415-144-6037
        BUT the above approach is a bit verbose and amateurous the better way is as follows:
        
        cursor = con.cursor()
        
        cursor.execute("DROP PROCEDURE IF EXISTS get_clients_by_state")
        
        cursor.execute("""
        
        CREATE PROCEDURE get_clients_by_state
        (
        state CHAR(2)
        )
        BEGIN
            SELECT * FROM clients c 
            WHERE c.state = IFNULL(state, c.state); 
        END
        
        """)
        
        con.commit()
        cursor.close()
        pd.read_sql("""
        CALL get_clients_by_state(NULL)
        """, con)
        
            client_id	name	address	city	state	phone
        0	1	Vinte	3 Nevada Parkway	Syracuse	NY	315-252-7305
        1	2	Myworks	34267 Glendale Parkway	Huntington	WV	304-659-1170
        2	3	Yadel	096 Pawling Parkway	San Francisco	CA	415-144-6037
        3	4	Kwideo	81674 Westerfield Circle	Waco	TX	254-750-0784
        4	5	Topiclounge	0863 Farmco Road	Portland	OR	971-888-9129


<a name="78"></a>
#### Parameter Validation

So far we saw the procedures to SELECT data but we also may use procedures to INSERT, UPDATE, or DELETE data.

        cursor = con.cursor()
        
        cursor.execute("DROP PROCEDURE IF EXISTS make_payment")
        cursor.execute("""
        
        CREATE PROCEDURE make_payment
        (
            invoice_id INT,
            payment_amount DECIMAL(9, 2),
            payment_date DATE
            )
        
        
        BEGIN
            UPDATE invoices i
            SET 
                i.payment_total = payment_amount, 
                i.payment_date = payment_date 
            WHERE i.invoice_id = invoice_id;     
        
        END
        """)

        con.commit()
        cursor.close()
        cursor = con.cursor()

Since the make_payment stored procedure I created only performs an UPDATE operation, it does not produce any results that can be returned by the pd.read_sql() function, so I need to use cursor object to call it:

        cursor.execute("""
        CALL make_payment (2, 100, '2019-01-01')
        """)
        
        con.commit()
        cursor.close()
        
        pd.read_sql("""
        SELECT *
        FROM invoices
        """, con)
        

        invoice_id	number	client_id	invoice_total	payment_total	invoice_date	due_date	payment_date
        0	2	03-898-6735	5	175.32	100.00	2019-06-11	2019-07-03	2019-01-01
        1	3	20-228-0335	5	147.99	0.00	2019-07-31	2019-08-20	None
        2	4	56-934-0748	3	152.21	0.00	2019-03-08	2019-03-28	None
        3	5	87-052-3121	5	169.36	0.00	2019-07-18	2019-08-07	None
        4	6	75-587-6626	1	157.78	74.55	2019-01-29	2019-02-18	2019-01-03
        5	7	68-093-9863	3	133.87	0.00	2019-09-04	2019-09-24	None
        6	8	78-145-1093	1	189.12	0.00	2019-05-20	2019-06-09	None
        7	9	77-593-0081	5	172.17	0.00	2019-07-09	2019-07-29	None
        8	10	48-266-1517	1	159.50	0.00	2019-06-30	2019-07-20	None
        9	11	20-848-0181	3	126.15	0.03	2019-01-07	2019-01-27	2019-01-11
        10	13	41-666-1035	5	135.01	87.44	2019-06-25	2019-07-15	2019-01-26
        11	15	55-105-9605	3	167.29	80.31	2019-11-25	2019-12-15	2019-01-15
        12	16	10-451-8824	1	162.02	0.00	2019-03-30	2019-04-19	None
        13	17	33-615-4694	3	126.38	68.10	2019-07-30	2019-08-19	2019-01-15
        14	18	52-269-9803	5	180.17	42.77	2019-05-23	2019-06-12	2019-01-08
        15	19	83-559-4105	1	134.47	0.00	2019-11-23	2019-12-13	None
        
        cursor = con.cursor()
        
        cursor.execute("""
        CALL make_payment (2, -100, '2019-01-01')
        """)

        con.commit()
        cursor.close()

        pd.read_sql("""
        SELECT *
        FROM invoices
        """, con)
        invoice_id	number	client_id	invoice_total	payment_total	invoice_date	due_date	payment_date
        0	2	03-898-6735	5	175.32	-100.00	2019-06-11	2019-07-03	2019-01-01
        1	3	20-228-0335	5	147.99	0.00	2019-07-31	2019-08-20	None
        2	4	56-934-0748	3	152.21	0.00	2019-03-08	2019-03-28	None
        3	5	87-052-3121	5	169.36	0.00	2019-07-18	2019-08-07	None
        4	6	75-587-6626	1	157.78	74.55	2019-01-29	2019-02-18	2019-01-03
        5	7	68-093-9863	3	133.87	0.00	2019-09-04	2019-09-24	None
        6	8	78-145-1093	1	189.12	0.00	2019-05-20	2019-06-09	None
        7	9	77-593-0081	5	172.17	0.00	2019-07-09	2019-07-29	None
        8	10	48-266-1517	1	159.50	0.00	2019-06-30	2019-07-20	None
        9	11	20-848-0181	3	126.15	0.03	2019-01-07	2019-01-27	2019-01-11
        10	13	41-666-1035	5	135.01	87.44	2019-06-25	2019-07-15	2019-01-26
        11	15	55-105-9605	3	167.29	80.31	2019-11-25	2019-12-15	2019-01-15
        12	16	10-451-8824	1	162.02	0.00	2019-03-30	2019-04-19	None
        13	17	33-615-4694	3	126.38	68.10	2019-07-30	2019-08-19	2019-01-15
        14	18	52-269-9803	5	180.17	42.77	2019-05-23	2019-06-12	2019-01-08
        15	19	83-559-4105	1	134.47	0.00	2019-11-23	2019-12-13	None
        In these terms, we need to make sure that our procedure does not accedidentaly store bad data (like -100 in the above as payment_total) in our database!

SIGNAL in SQL is like throwing an exception in other programming languages.

        cursor = con.cursor()
        
        cursor.execute("DROP PROCEDURE IF EXISTS make_payment")
        
        cursor.execute("""
        CREATE PROCEDURE make_payment
        (
            invoice_id INT,
            payment_amount DECIMAL(9, 2),
            payment_date DATE
        )
        BEGIN
        
            IF payment_amount <= 0 THEN 
                SIGNAL SQLSTATE '22003' 
                    SET MESSAGE_TEXT = 'Invalid payment amount'; 
            END IF; 
        
            UPDATE invoices i
                SET i.payment_total = payment_amount,
                    i.payment_date = payment_date
            WHERE i.invoice_id = invoice_id; 
        END
        """)
        
        con.commit()
        cursor.close()
        Now
        
        cursor = con.cursor()
        
        cursor.execute("""
        CALL make_payment (2, -100, '2019-01-01')
        """)
        
        con.commit()
        cursor.close()


        ~/.local/lib/python3.6/site-packages/pymysql/err.py in raise_mysql_exception(data)
            141     if errorclass is None:
            142         errorclass = InternalError if errno < 1000 else OperationalError
        --> 143     raise errorclass(errno, errval)
        
        OperationalError: (1644, 'Invalid payment amount')
        SQLSTATE errors: https://www.ibm.com/docs/en/db2-for-zos/11?topic=codes-sqlstate-values-common-error

SET MESSAGE_TEXT is optional but a good practice

So it is a good practice to check the parameters of a stored procedure before before making any changes to the data, but too much of a good thing is a bad thing so don't write too much validation logics, keep it to what is absolutely essential.

<a name="79"></a>
#### Output Parameters

We can also use parameters to return values to the calling programs.

By default, all the parameters in the stored procedure are input parameters meaning we can only use them to pass values to the stored procedure. If we prefix them with keyword OUT we mark them as output parameters meaning we can use them to get values from these procedure. We also need to define user defined variables, the ones prefixed with @ in the code below. like:

        con = connector('sql_invoicing')
        cursor = con.cursor()
        
        
        cursor.execute("SET @invoices_count = 0")
        cursor.execute("SET @invoices_total = 0")
        
        cursor.execute("DROP PROCEDURE IF EXISTS get_unpaid_invoices_for_client")
        cursor.execute("""
        CREATE PROCEDURE get_unpaid_invoices_for_client
        (
            client_id INT,
            OUT invoices_count INT,
            OUT invoices_total DECIMAL(9, 2)
        )
        
        BEGIN
        
            SELECT 
                COUNT(*),
                SUM(invoice_total)
            INTO invoices_count, invoices_total
            FROM invoices i
            WHERE i.client_id = client_id AND payment_total = 0; 
        END
        """)
        
        con.commit()
        cursor.close()

When calling the stored procedure, I also need to pass these output variables as well, like in the following:

        cursor = con.cursor()
        
        cursor.execute("CALL get_unpaid_invoices_for_client(3, @invoices_count, @invoices_total)")
        cursor.execute("SELECT @invoices_count, @invoices_total")
        output = cursor.fetchone()
        print(output)
        con.commit()
        cursor.close()
        
        (2, Decimal('286.08'))

Using output parameters requires a bit more effort to read data and I would suggest avoid them unless you have a valid reason to use them.

<a name="80"></a>
#### Variables

User or session variables: We quite often use them when defining a stored procedure that has output parameters like in the previous point. They are the variables that will be in memory during the entire client session, when the client disconnects from MySQL these are freed up. We define them using SET statement and we prefix them using an @ like

        SET @invoice_count = 0

Local variables; they are defined inside the stored procedure or function. These variables do not stay in memory during the entire session and as soon as our stored procedure finishes execution these variables are freed up. We quite often use these variables to perform calculations in our stored procedures. We use declare statement to declare a local variable on the top right after the BEGIN statement.

        cursor = con.cursor()
        cursor.execute("DROP PROCEDURE IF EXISTS get_risk_factor")
        cursor.execute("""
        CREATE PROCEDURE get_risk_factor()
        BEGIN
          DECLARE risk_factor DECIMAL(9, 2) DEFAULT 0;
          DECLARE invoices_total DECIMAL(9, 2);
          DECLARE invoices_count INT; 
        
          SELECT COUNT(*), SUM(invoice_total)
          INTO invoices_count, invoices_total
          FROM invoices;
        
          SET risk_factor = invoices_total / invoices_count * 5;
        
          SELECT risk_factor; 
        END 
        
        """)
        con.commit()
        cursor.close()
        
        pd.read_sql("""
        CALL get_risk_factor
        """, con)
        
        risk_factor
        0	777.75

<a name="81"></a>
#### Functions

+ Let's see how to create our own functions 
+ Functions are pretty similar to the stored procedures BUT they can only return a **single value**. So functions unlike stored procedures cannot return results set with multiple rows and columns.
+ The syntax for creating a function is very similar to the syntax to create a stored procedure 
+ One of the main differences between functions and stored procedures is the RETURNS statement where we specify the type of value the functions returns which could be any data type in MySQL.
+ Right after the RETURNS statement, we need to set the **function's attributes**, which could be one of the following (every MySQL function should have at least one attribute):

    + DETERMINISTIC meaning if we give the function the same set of values it always returns the same results every time (in short it means the same output for the same input)
    + READS SQL DATA, meaning we are going to have a SELECT statement in our function to read some data 
    + MODIFIES SQL DATA, meaning we are going to have an INSERT, UPDATE or DELETE statement in our function 

We can have multiple attributes in a function for example if our function both reads and modifies the SQL data we may have both READS SQL DATA and MODIFIES SQL DATA as our function's attributes. 

            cursor = con.cursor()
            
            cursor.execute("DROP FUNCTION IF EXISTS get_risk_factor_for_client")
            cursor.execute("""
            CREATE FUNCTION get_risk_factor_for_client
            (
                client_id INT
            )
            RETURNS INTEGER
            READS SQL DATA
            BEGIN 
                DECLARE risk_factor DECIMAL(9, 2) DEFAULT 0;
                DECLARE invoices_total DECIMAL(9, 2);
                DECLARE invoices_count INT; 
            
                SELECT COUNT(*), SUM(invoice_total)
                INTO invoices_count, invoices_total
                FROM invoices i
                WHERE i.client_id = client_id; 
            
                SET risk_factor = invoices_total / invoices_count * 5;
            
                RETURN IFNULL(risk_factor, 0); 
                END 
                """)
                
                con.commit()
                cursor.close()
      
We can use this function just like the built-in functions in the SELECT statements:

        pd.read_sql("""
        SELECT 
            client_id,
            name,
            get_risk_factor_for_client(client_id) AS risk_factor
        FROM clients
        """, con)
        
        client_id	name	risk_factor
        0	1	Vinte	803
        1	2	Myworks	0
        2	3	Yadel	706
        3	4	Kwideo	0
        4	5	Topiclounge	817

Similar to views and stored procedures it is a good practice to save your functions in SQL files and put them under the source control.

We can use the DROP FUNCTION statement to drop a function:

        DROP FUNCTION IF EXISTS function_name
        
<a name="82"></a>
#### Conventions

Try to stick with the conventions, like naming conventions or the default delimiter, that are already adopted in your organization, and don't try to reinvent the wheel! 

<a name="83"></a>
### Triggers and Events

<a name="84"></a>
#### Introduction

A trigger is a block of SQL code that automatically gets executed before or after an INSERT, UPDATE, or DELETE statement. We use triggers to enforce **data consistency.**



[Triggers and Events](#83)
    1. [Introduction](#84)
    2. [Viewing Triggers](#85)
    3. [Dropping Triggers](#86)
    4. [Using Triggers for Auditing](#87)
    5. [ Events](#88)
    6. [Viewing, Dropping and Altering Events](#89)
