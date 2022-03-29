# Class12 Reading Notes

[Status Codes Based On REST Methods](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)
In your own words, describe what each group of status code represents:

100’s = informational status codes
200’s = success codes
300’s = redirection codes, location is not avail
400’s = invalid request to server
500’s = unable to reach server, or too many requests to server

What is a status code 202? Accepted
What is a status code 308? Permanent Redirect 

What code would you use if an update didn’t return data to a client? 204

What code would you use if a resource used to exist but no longer does? 410

What is the ‘Forbidden’ status code? 403

Additional Resources
Videos
[Build A REST API With Node.js, Express, & MongoDB](https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw) - Quick - First 20 minutes
Why do we need to pull our MongoDB database string out of our server and put it into our .env? to connect the DB
What is middleware? software that provides common services and capabilities to applications outside of what's offered by the operating system

What does app.use(express.json()) do? parses incoming JSON requests and puts the parsed data in req

What does the /:id mean in a route? item id

What is the difference between PUT and PATCH?
PUT is a method of modifying resource where the client sends data that updates the entire resource .	PATCH is a method of modifying resources where the client sends partial data that is to be updated without modifying the entire data.
How do you make a default value in a schema?

What does a 500 error status code mean?
server-side

What is the difference between a status 200 and a status 201?
200 the request was received and understood and is being processed. 
A 201 status code indicates that a request was successful and as a result

----
## Things I want to know more about


---
### [Home](https://github.com/MISalz/301_Reading_Notes)