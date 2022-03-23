# Class08 Reading Notes
REST API https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design

<ol><li>What does REST stand for? 
Representational State Transfer
</li><li>REST APIs are designed around a ____.
Resources
</li><li>What is an identifer of a resource? Give an example.
https://adventure-works.com/orders/1
</li><li>What are the most common HTTP verbs?
GET, POST, PUT, PATCH, and DELETE.
</li><li>What should the URIs be based on?
URIs should be based on nouns (the resource) and not verbs (the operations on the resource).
</li><li>Give an example of a good URI.
https://adventure-works.com/orders
</li><li>What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?
to have a big request from the server.this can be a bad thing because it can request to much information and slow downt the request.
</li><li>What status code does a successful `GET` request return?
typically returns HTTP status code 200 (OK)
</li><li>What status code does an unsuccessful `GET` request return?
typically returns HTTP status code 200 (OK)
</li><li>What status code does a successful `POST` request return?
typically returns HTTP status code 200 (OK)(content)
</li><li>What status code does a successful `DELETE` request return?
the web server should respond with HTTP status code 204 (No Content),
</li>
</ol>

## Maturity model for web APIs:

Level 0: Define one URI, and all operations are POST requests to this URI.   
Level 1: Create separate URIs for individual resources.   
Level 2: Use HTTP methods to define operations on resources.   
Level 3: Use hypermedia (HATEOAS, described below).


----
## Things I want to know more about


---
### [Home](https://github.com/MISalz/301_Reading_Notes)