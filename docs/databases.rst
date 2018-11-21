.. databases:

========
Databases
========

.. contents:: :local:


.. _introduction:

Introduction
============
Databases in the most basic terms, serve as a way of storing, organizing and retrieving information.
The two main kinds of databases are Relational and Non-Relational (or NoSQL). Within both categories are a host of other database types which the following sections will explore in detail.

**Why It's Important:**

Often times a data scientist will have to work with a database in order to retrieve the data they need to build their models or to do data analysis.
Thus it's important that a scientist familiarize themselves with the different types of databases and how to query them.

.. Relational:

Relational
===========
A relational database is a collection of tables and the relationships that exist between these tables. These tables contain numerous columns (table attributes) with rows that represent the data within the table.
Often times these rows will have a unique identifier associated with them, called primary keys. Relationships between tables are created using foreign keys, whose primary function is to join tables together.

To get data out of a relational database, a data scientist would use SQL, with different relational databases using slightly different versions of SQL. 
When interacting with the database using SQL, whether creating a table or querying it, you are creating what is called a Transaction. Transactions in relational databases represent a unit of work performed against the database.

An important concept with transactions is ACID, which stands for:

  - Atomicity:
  - Consistency:
  - Independence:
  - Durability:

Types
-------
While there are many different kinds of relational databases, the most popular have proven to be:

  - PostgreSQL:
  - Oracle:
  - MySQL:
  - Microsoft SQL Server:
  - DB2:

Advantages
----------
  - SQL standards are well defined and commonly accepted
  - 

Disadvantages
-------------
  - Poor performance with unstrucutred data types due to schema and type constraints
  - 

.. Non-relational/NoSQL:

Non-relational/NoSQL
===========

Types
-------
  - Key-value Stores:
  - Wide column Stores:
  - Document Stores:
  - Graph Databases:
  - Search Engine:

Advantages
----------
  - High availability
  - Schema free or schema-on-read options


Disadvantages
-------------
  - 

Terminology
===========
Query
  A query can be thought of as a single action that is taken on a database

Transaction
  A transaction is a sequence of queries that make up a single unit of work performed against a database.


ACID
  Atomicity, Consistency, Isolation, Durability

Schema
  A schema is the structure of a database

Scalability
  Scalability when databases are concerned has to do with how databases handle an increase in transactions as well as data stored. The two main types are vertical scalability, which is concerned with adding more capacity to a single machine by adding additional RAM, CPU, etc. Horizontal scalability has to do with adding more machines and splitting the work amongst them.

Normalization
  This is a technique of organizing tables within a relational database. It involves splitting up data into seperate tables to reduce redundancy and improve data integrity.

Denormalization
  This is a technique of organizing tables within a relational database. It involves combining tables to reduce the number of JOIN queries.

.. rubric:: References

.. [1] https://dzone.com/articles/the-types-of-modern-databases
.. [2] 