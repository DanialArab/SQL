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
    1. 

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


