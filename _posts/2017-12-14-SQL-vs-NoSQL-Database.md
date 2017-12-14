---
layout: post
title: "SQL Vs NOSQL Database"
tags:
- SQL, NOSQL, MangoDB, Relational database, Schema, Structure, Nonstructure 
category:
- Database
---

In the world of `database technology`, there are two main types of databases: `SQL` and `NoSQL`—or, relational databases and non-relational databases. The difference speaks to how they’re built, the type of information they store, and how they store it. Relational databases are structured, like phone books that store phone numbers and addresses. Non-relational databases are document-oriented and distributed, like file folders that hold everything from a person’s address and phone number to their Facebook likes and online shopping preferences.

We call them SQL and NoSQL, referring to whether or not they’re written solely in structured query language (SQL). In this article, we’ll explore what SQL is, how it makes these databases different, and how each type structures the data it holds so you can easily determine which type is right for you.

## RELATIONAL DATABASES
First, let’s take a look at one of the main features that separates these two systems: the way they structure data. A relational database—or, an SQL database, named for the language it’s written in, Structured Query Language (SQL)—is the more rigid, structured way of storing data, like a phone book. Developed by IBM in the 1970s, a `relational database` consists of two or more tables with columns and rows. Each row represents an entry, and each column sorts a very specific type of information, like a name, address, and phone number. The relationship between tables and field types is called a schema. In a relational database, the `schema` must be clearly defined before any information can be added.

## Structured Query Language (SQL)
It is a programming language used by database architects to design relational databases. In an SQL database like MySQL, Sybase, Oracle, or IBM DM2, SQL executes queries, retrieves data, and edits data by updating, deleting, or creating new records. SQL is a lightweight, declarative language that does a lot of heavy lifting for the relational database, acting like a database’s version of a server-side script. One particular advantage of SQL is its simple-yet-powerful JOIN clause, which allows developers to retrieve related data stored across multiple tables with a single command.

### Popular SQL databases and RDBMS’s

- `MySQL`—the most popular open-source database, excellent for CMS sites and blogs.

- `Oracle`—an object-relational DBMS written in the C++ language. If you have the budget, this is a full-service option with     great customer service and reliability. Oracle has also released an Oracle NoSQL database.

- `IMB DB2`—a family of database server products from IBM that are built to handle advanced “big data” analytics.

- `Sybase`—a relational model database server product for businesses primarily used on the Unix OS, which was the first 
  enterprise-level DBMS for Linux.

- `MS SQL Serve`r—a Microsoft-developed RDBMS for enterprise-level databases that supports both SQL and NoSQL architectures.

- `Microsoft Azure`—a cloud computing platform that supports any operating system, and lets you store, compute, and scale         data in one place. A recent survey even put it ahead of Amazon Web Services and Google Cloud Storage for corporate data       storage.

- `MariaDB`—an enhanced, drop-in version of MySQL.

- `PostgreSQL`—an enterprise-level, object-relational DBMS that uses procedural languages like Perl and Python, in addition       to SQL-level code.


## NOSQL DATABASES: NON-RELATIONAL & DISTRIBUTED DATA

If your data requirements aren’t clear at the outset or if you’re dealing with massive amounts of unstructured data, you may not have the luxury of developing a relational database with clearly defined schema. Enter non-relational databases, which offer much greater flexibility than their traditional counterparts. Think of non-relational databases more like file folders, assembling related information of all types. If a `WordPress` blog used a NoSQL database, each file could store data for a blog post: social likes, photos, text, metrics, links, and more.

Unstructured data from the web can include sensor data, social sharing, personal settings, photos, location-based information, online activity, usage metrics, and more. Trying to store, process, and analyze all of this unstructured data led to the development of schema-less alternatives to SQL. Taken together, these alternatives are referred to as NoSQL, meaning “Not only SQL.” While the term NoSQL encompasses a broad range of alternatives to relational databases, what they have in common is that they allow you to treat data more flexibly.

How do NoSQL databases work? Instead of tables, NoSQL databases are `document-oriented`. This way, non-structured data (such as articles, photos, social media data, videos, or content within a blog post) can be stored in a single document that can be easily found but isn’t necessarily categorized into fields like a relational database does. It’s more intuitive, but note that storing data in bulk like this requires extra processing effort and more storage than highly organized SQL data. That’s why `Hadoop ,   an open-source computing` and `data analysis platform` capable of processing huge amounts of data in the cloud, is so popular in conjunction with NoSQL database stacks.

### Popular NoSQL Databases

- `MongoDB`—the most popular NoSQL system, especially among startups. A document-oriented database with JSON-like documents       in dynamic schemas instead of relational tables that’s used on the back end of sites like Craigslist, eBay, Foursquare.       It’s open-source, so it’s free, with good customer service. Read more in Should You Use MongoDB? A Look at the Leading       NoSQL Database.

- `Apache’s CouchDB`—a true DB for the web, it uses the JSON data exchange format to store its documents; JavaScript for         indexing, combining and transforming documents; and, HTTP for its API.

- `HBase`—another Apache project, developed as a part of Hadoop, this open-source, non-relational “column store” NoSQL DB is     written in Java, and provides BigTable-like capabilities.

- `Oracle NoSQ`L—Oracle’s entry into the NoSQL category.

- `Apache’s Cassandra DB`—born at Facebook, Cassandra is a distributed database that’s great at handling massive amounts of       structured data. Anticipate a growing application? Cassandra is excellent at scaling up. Examples: Instagram, Comcast,       Apple, and Spotify.

- `Riak`—an open-source key-value store database written in Erlang. It has fault-tolerance replication and automatic data         distribution built in for excellent performance.
