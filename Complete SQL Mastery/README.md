## Complete SQL Mastery

Here is the summary of my notes from the course <a href="https://codewithmosh.com/p/complete-sql-mastery">Complete SQL Mastery<\a>. The structure of my notes is as follows:

1. [Introduction](#1)
    1. [What is a Database?](#2)
3. [Array](#2)
4. [Matrix](#3)
5. [Singly Linked List ](#4)
6. [Hash Table](#5)
7. [Two Pointers](#6)
8. [String Matching](#7)
9. [Stack](#8)
10. [Binary Tree](#9)
11. [Greedy](#10)

<a name="1"></a>
### Introduction 

<a name="2"></a>
#### What is a Database? 

A database is a collection of data stored in a format that can be easily accessed. In order to manage our databases we use a software called database management system (DBMS). DBMS are categorized as two broad categories:

Relational

NoSQL

2. Relational DBMS

We store data in tables that are linked to each other using relationships, each table stores data about the specific type of object. We use Structured Query Language (SQL) to work with these relational DBMS. We use SQL to query or modify our data. There are various RDBMS like:

MySQL
SQL Server
Oracle
...
All of these flavors are based on the standard specifications of SQL. So what I learn in this course mostly can be applied to any of these RDBMS. In this course we use MySQL, which is the most popular open source database in the world.

3. Non relational databases

In Non relational databases we don’t have tables or relationships, these databases are very different from relational databases and NoSQL systems don’t understand SQL and they have their own query language.

4. Course structure

5. What you will learn:

Retrieving data
Inserting data
Updating data
Deleting data
Even though we use MySQL in this course, what you will be learning will be applicable at least 90% to other DBMSs. There might be a slight difference in syntax though.

You also learn

Summarizing data for creating reports
Writing complex queries using subqueries
Built-in functions
As you process you see you are writing the same queries again and again and so you will learn about the followings for storing queries and reusing them later:

Views
Stored procedures
These are great for increasing your productivity.

Then we move on to advanced topics:
Triggers
Events
Transactions
Concurrency
If you want to stand out among the crowds you have to learn about:

Designing databases
Mosh dedicated a complete in-depth section on it.

Then we look at

Indexing for high performance, indexes are essential when your database grows in size, we can speed up our queries using indexes. If you have billions of records you want to query pretty quick using indexes
Finally we finish the course by

Securing databases
