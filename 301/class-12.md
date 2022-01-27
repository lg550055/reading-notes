# REST Methods Status Codes

## Status Codes Based On REST Methods
Clean API design uses HTTP codes to inform clients about the status of their requests.  A status code is a number between 100 and 600. The first digit defines the class of the status. A status code comes with a reason phrase. The code is for programmatic recognition; the phrase is for humans.   Understanding codes help us locate problems faster.

1. Describe what each group of status code represents:
  - 100’s = Informational. Request receive, will try to comply.
  - 200’s = Success.  Request accepted.
  - 300’s = Redirect.  Client to issue request to a new location.
  - 400’s = Client error, invalid request. Confrim input and try again.
  - 500’s = Server error.  Try request later.

2. What is a status code 202?  Accepted; valid request, but processing later (asynchronous).
3. What is a status code 308?  Permanent redirect; use another URL.
4. What code would you use if an update didn’t return data to a client?  204 No Content (code for updates that don't return data)
5. What code would you use if a resource used to exist but no longer does?  410 Gone.
6. What is the ‘Forbidden’ status code?  403 Forbidden (client may have authorized itself but does not have permission to access resource)

## Build A REST API With Node.js, Express, & MongoDB

1. Why do we need to pull our MongoDB database string out of our server and put it into our .env?  Because otherwise anyone with access to the code can alter the database.
2. What is middleware?  Code that runs once a request is made but before it gets passed to a route.
3. What does app.use(express.json()) do?  Allows the server to accept JSON.
4. What does the /:id mean in a route?  It means it is a parameter (we can access using req.params.id to identify the specific request).
5. What is the difference between PUT and PATCH?  PUT updates all information.  PATCH updates selected portions.
6. How do you make a default value in a schema?  Use the keyword 'default' for the key
7. What does a 500 error status code mean?  Server error (that had nothing to do with the client).
8. What is the difference between a status 200 and a status 201?  200 is a generic success code.  201 means successfully created a new objec.

--- 

### Resources

- [Status Codes Based On REST Methods](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)
- [Build A REST API With Node.js, Express, & MongoDB](https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw)

---

[Back to table of contents](../README.md)