# APIs
> Most modern web applications expose APIs that clients can use to interact with the application.

## API Design Best Practices
> A well-designed web API should aim to support platform independece and service evolution.

1. What does REST stand for?  Representational State Transfer
2. REST APIs are designed around a: resource.
3. What is an identifer of a resource? Give an example.  A URI that uniquely identifies the resource.  https://adventure-works.com/orders/1
4. What are the most common HTTP verbs?  GET, POST, PUT, PATCH, and DELETE.
5. What should the URIs be based on?  Nouns; the resource.
6. Give an example of a good URI.  https://adventure-works.com/orders
7. What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?  An API that exposes a large number of small resources.  This is bad because it generates more requests, each of which impose a load on the server.  It is better to combine related information into a bigger resource that can be accessed by a single request.
8. What status code does a successful GET request return?  200 (OK)
9. What status code does an unsuccessful GET request return?  404 (Not Found)
10. What status code does a successful POST request return?  201 (Created), 200 (processed), 204 (No Content)
11. What status code does a successful DELETE request return?  400 (Bad Request)

## RegEx

How would you match a phone number from your city using RegEx?  \(318\)200-2555

--- 

### Resources

- [API Design Best Practices](https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design)
- [RegExr](https://regexr.com/)
- [Regex Tutorial](https://medium.com/factory-mind/regex-tutorial-a-simple-cheatsheet-by-examples-649dc1c3f285)
- [Regex 101](https://regex101.com/)

---

[Back to table of contents](../README.md)