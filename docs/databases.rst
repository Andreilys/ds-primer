.. databases:

========
Databases
========

.. contents:: :local:


.. _introduction:

Introduction
============
Databases in the most basic terms, serve as a way of storing, organizing and retrieving information.
The two main kinds of databases are Relational and Non-Relational (NoSQL). Within both kinds of databases are a variety of other database sub-types which the following sections will explore in detail.

**Why It's Important:**

Often times a data scientist will have to work with a database in order to retrieve the data they need to build their models or to do data analysis.
Thus it's important that a scientist familiarize themselves with the different types of databases and how to query them.

.. Relational:

Relational
===========
A relational database is a collection of tables and the relationships that exist between these tables. These tables contain columns (table attributes) with rows that represent the data within the table.
You can think of the column as the header indicating the name of the data being stored, and the row being the actual data points that are stored in the database.
Often times these rows will have a unique identifier associated with them, called primary keys. Relationships between tables are created using foreign keys, whose primary function is to join tables together.

To get data out of a relational database, you would use SQL, with different relational databases using slightly different versions of SQL.
When interacting with the database using SQL, whether creating a table or querying it, you are creating what is called a Transaction. Transactions in relational databases represent a unit of work performed against the database.

An important concept with transactions in relational databases is maintaining ACID, which stands for:

  - Atomicity: A transaction typically contains many queries. Atomicity guarantees that if one query fails, then the whole transaction fails, leaving the database unchanged.
  - Consistency: This ensures that a transaction can only bring a database from one valid state to another, meaning a transaction cannot leave the database in a corrupt state.
  - Isolation: Since transactions are executed concurrently, this property ensures that the database is left in the same state as if the transactions were executed sequentially.
  - Durability: This property gurantees that once a transaction has been committed, its effects will remain regardless of any system failure.

Types
-------
While there are many different kinds of relational databases, the most popular are:

  - PostgreSQL: An open-source object-relational database management system that is ACID-compliant and transactional.
  - Oracle: A multi-model database management system that is produced and marketed by Oracle.
  - MySQL: An open-source relational database management system with a proprietary paid version available for additional functionality.
  - Microsoft SQL Server: A relational database management system developed by Microsoft.
  - Maria DB: A MySQL compabtable database engine forked from MySQL.

Advantages
----------
  - SQL standards are well defined and commonly accepted
  - Easy to categorize and store data that can later be queried
  - Simple to understand, since the table structure and relationships are intuitive ato most users
  - Data integrity, through strong data typing and validity checks to make sure that data falls within an acceptable range

Disadvantages
-------------
  - Poor performance with unstructured data types due to schema and type constraints
  - Can be slow and not scalable compared to NoSQL
  - Unable to map certain kinds of data such as graphs

.. Non-relational/NoSQL:

Non-relational/NoSQL
===========
Non-relational databases were developed from a need to deal with the exponential growth in data that was being gathered and processed. 
Additionally dealing with scalability, multi-structured data and geo-distribution were a few more reasons that NoSQL was created.
There are a variety of NoSQL implementations, each with their own approach to tackling these problems. 


Types
-------
  - Key-value Store: One of the simpler NoSQL stores that works by assigning a value for each key. 
    The database then uses a hash table to store unique keys and pointers for each data value. 
    They can be used to store user session data, and examples of these types of databases include Redis and Amazon Dynamo.
  - Document Store: Similar to a key-value store, however in this case the value contains structured or semi-structured data and is referred to as a document.
    A use case for document store could be for a blogging platform. Examples of document stores include MongoDB and Apache CouchDB.
  - Column Store: In this implementation, data is stored in cells grouped in columns of data rather than rows of data, with each column being grouped into a column family.
    These can be used in content management systems, and examples of these types of databases include Cassandra and Apache Hbase.
  - Graph Store: These are based on the Entity - Attribute - Value model. 
    Entities will have associated attributes and subsequent values when data is inserted.
    Nodes will store data about each entity, along with the relationships between nodes. 
    Graph stores can be used in applications such as social networks, and examples of these types of databases include Neo4j and ArangoDB.

Advantages
----------
  - High availability
  - Schema free or schema-on-read options
  - Ability to rapidly prototype applications
  - Elastic scalability
  - Can store massive amounts of data


Disadvantages
-------------
  - Since most NoSQL databases use eventual consistency instead of ACID, there may be a risk that data may be out of sync
  - Less support and maturity in the NoSQL ecosystem


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

* https://dzone.com/articles/the-types-of-modern-databases
* https://www.mongodb.com/nosql-explained
* https://www.channelfutures.com/cloud-2/the-limitations-of-nosql-database-storage-why-nosqls-not-perfect
* https://opensourceforu.com/2017/05/different-types-nosql-databases/