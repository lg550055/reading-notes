# Authentication

## CRUD Basics
> CRUD is an acronym that stands for Create, Read, Update and Delete.  CRUD represents the four basic functions that models should be able to do and are considered necessary to implement a persistent storage application. Create new data, read or view the data, edit or update the data, and delete it when appropriate.

1. Which HTTP method would you use to update a record through an API?
PUT, which replaces current data of the target resource with the uploaded content.

2. Which REST methods require an ID parameter?
PUT, PATCH and DELETE, each requires en ID to ensure we are affecting the intended resource.  GET if we intend to access a single resource (as opposed to a collection).


## Speed Coding: Building a CRUD API

1. What’s the relationship between REST and CRUD?
The REST methods (post, get, put and delete) enable us to perform CRUD operations.

2. If you had to describe the process of creating a RESTful API in 5 steps, what would they be?
  1. Set up framework -server, dependencies, port
  2. Define schema
  3. Connect database
  4. Build routes -get, post, put and delete
  5. Test

--- 

### Resources

- [CRUD Basics](https://medium.com/geekculture/crud-operations-explained-2a44096e9c88)
- [Speed Coding: Building a CRUD API](https://www.youtube.com/watch?v=EzNcBhSv1Wo)

---

[Back to table of contents](../README.md)