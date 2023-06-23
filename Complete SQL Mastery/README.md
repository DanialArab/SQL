## Complete SQL Mastery

Here is the summary of my notes from the course <a href="https://codewithmosh.com/p/complete-sql-mastery">Complete SQL Mastery</a>. The structure of my notes is as follows:

1. [Introduction](#1)
    1. [What is a Database?](#2)
    2. [Relational DBMS](#3)
    3. [Non-relational databases](#4)
    4. [Course structure](#5)
2. [Retrieving Data From a Single Table](#6)
    1. [The SELECT statement](#7)
    2. [The AND, OR, and NOT operators](8#)
    3. [The IN operator in SQL](#9)
    4. [The BETWEEN operator in SQL](#10)
    5. [The LIKE operator](#11)
    6. [The REGEXP operator](#12)
    7. [The IS NULL operator](#13)
    8. [The ORDER BY clause](#14)
    9. [ The LIMIT clause](#15)
3. [Retrieving Data From Multiple Tables](#16)
    1. [Inner Joins](#17)
    2. [Joining across databases](#18)
    3. [Self Joins](#19)
    4. [Joining Multiple Tables](#20)
    5. [Compound Join Conditions](#21)
    6. [Implicit Join Syntax](#22)
    7. [Outer Joins](#23)
    8. [Outer Joins between Multiple Tables](#24)
    9. [Self Outer Joins](#25)
    10. [The Using Clause](#26)
    11. [Natural Joins](#27)
    12. [Cross Joins](#28)
    13. [Unions](#29)
4. [Inserting, Updating, and Deleting Data](#30)

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
### Retrieving Data From a Single Table 

<a name="7"></a>
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

<a name="8"></a>
#### The AND, OR, and NOT operators

AND is operated first! But we use parenthesis to make our code cleaner and easier to understand.

<a name="9"></a>
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
    
<a name="10"></a>
#### The BETWEEN operator in SQL

Whenever we are comparing an attribute with a range of values we can use BETWEEN operator to make you code shorter and cleaner like:

        USE sql_store;
        SELECT *
        FROM customers 
        WHERE points BETWEEN 1000 AND 3000 -- The range values is inclusive. 

<a name="11"></a>
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

<a name="12"></a>
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

<a name="13"></a>
#### The IS NULL operator

How to look for records that miss an attribute? Like if we want to find all the customers that don’t have a phone number and like we want to send an email to them and say please provide phone number. To do so we use IS NULL operator:

        SELECT *
        FROM customers
        WHERE phone IS NULL 

Here we also can use NOT operator to get the customers who do have a phone like

        SELECT *
        FROM customers
        WHERE phone IS NOT NULL
        
<a name="14"></a>
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

<a name="15"></a>
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

<a name="16"></a>
### Retrieving Data From Multiple Tables

<a name="17"></a>
#### Inner Joins



<a name="18"></a>
#### Joining across databases

<a name="19"></a>
#### Self Joins

<a name="20"></a>
#### Joining Multiple Tables

<a name="21"></a>
#### Compound Join Conditions

<a name="22"></a>
#### Implicit Join Syntax

<a name="23"></a>
#### Outer Joins

<a name="24"></a>
#### Outer Joins between Multiple Tables

<a name="25"></a>
#### Self Outer Joins

<a name="26"></a>
#### The Using Clause

<a name="27"></a>
#### Natural Joins

<a name="28"></a>
#### Cross Joins

<a name="29"></a>
#### Unions
