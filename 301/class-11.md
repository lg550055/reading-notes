# Mongo and Mongoose

## NoSQL vs SQL intro

1. What does SQL stand for?  Structured Query Language
2. What is a relational database?  Is a collection of items with pre-defined relationships between them.
3. What type of structure does a relational database work with?  Tables of rows and columns.
4. What is a ‘schema’?  The structure that holds the data and that all data must meet.
5. What is a NoSQL database?  Is a non-tabular database.
6. How does it work?  Like a JSON object; stores data in key:value pairs.
7. What is inside of a Mongo database?  Collections and documents.
8. Which is more flexible - SQL or MongoDB? and why.  MongoDB because it does not have a strict schema, which makes it easier to change the patterns for storing data.
9. What is the disadvantage of a NoSQL database?  Lack of data homogeneity and duplicate data to store and maintain.

## NoSQL vs SQL use cases

Five differences

SQL: Strict schema  vs  NoSQL: No schema
SQL: Relations  vs  NoSQL: No / few relations
SQL: Distributed data  vs  NoSQL: Nested data
SQL: Hard to scale  vs  NoSQL: Simple to scale
SQL: Limit on queries/s  vs  NoSQL: Great query performance


1. What kind of data is a good fit for an SQL database?  Normalized, distributed data with frecquent modifications.
2. Give a real world example.  Marketing data, scientific research date, financial data...
3. What kind of data is a good fit a NoSQL database?  Not homogeneous, with a lot more reads than writes.
4. Give a real world example.  Content and metadta store.
5. Which type of database is best for hierarchical data storage?  NoSQL; because it follows key:value logic.
6. Which type of database is best for scalability?  NoSQL; just add servers.

--- 

### Resources

- [NoSQL vs SQL](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)
- [NoSQL vs SQL video](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)
- [mongoose api](https://mongoosejs.com/docs/api.html#Model)
- [React Router](https://reactrouter.com/web/api/BrowserRouter)

---

[Back to table of contents](../README.md)