CRUD

1. 100s - These are informational status codes; they usually tell the client that the header part of the request has been received and the server will try to comply with a transmission demand of the client. Like using a different protocol or telling the client that its request will fail before they start sending the body.

 200s - These are the success codes. They tell the client that its request was accepted. In case of asynchronous processing of a request (202), this doesn’t mean the request was successfully processed only that it met all validation requirements at the time of sending.

 300s - These are redirection codes. They tell the client that the resource they are requesting isn’t available at the expected location anymore. This can have multiple reasons, be temporary or permanent, but the client has to issue a request to the new location.

 400s - These are the client error codes. They are all about invalid requests a client sent to a server. There are several causes to this, timeouts, wrong URI, missing authentication, etc. A client is sending incorrect input and should confirm the input parameters are correct before retrying the request.

 500s - These are the server error codes. Often they indicate problems with overwhelmed servers or unreachable servers behind proxies, but sometimes they can be directly related to client requests that trigger error exceptions on the server. These errors can be temporary or permanent. Usually it’s best for the client to retry the same request

 2. 202 - Accepted - Often used for asynchronous processing. This code tells the client that the request was valid, but its processing will finish sometime in the future. The response body should include an URL to the finished resource with some information about when it will be available, or an URL to some monitoring endpoint that tells the client when the resource is available.

 3. 308 - Permanent Redirect - This tells the client to use another URL to access the resource and not use the current URL anymore. It’s helpful when we have multiple endpoints for one

 4. 204 - No Content - A proper code for updates that don’t return data to the client, for example when just saving a currently edited document.

 5. 410 Gone - This is like 404 but we know that the resource existed in the past, but it got deleted or somehow moved, and we don’t know where.

 6. 403 Forbidden - The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.


SOURCE:https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/


Building a quick REST API with Node.js, Express & MongoDB

1. Why do we need to pull our MongoDB database string out of our server and put it into our .env? We have to pull it into a variable in our .env. Then we add in the process.env.____ whatever you named it. At the beginning, we add require('dotenv').config(). And then we are able to connect to the database

2. What is middleware? Code that runsw when the server gets a request but before it gets passed to your routes.

"Middleware is software that lies between an operating system and the applications running on it. Essentially functioning as hidden translation layer, middleware enables communication and data management for distributed applications."

3. What does app.use(express.json()) do? Essentially lets our server accept JSON as a body instead of a post or get element

4. What does the /:id mean in a route? It means it is a parameter where we can request anything following the id

5. What is the difference between PUT and PATCH? Patch - We only want to update based on what the user passes us. PUT - updates everything

6. How do you make a default value in a schema? default: value.now

7. What does a 500 error status code mean? that there is an error on our server and it had nothing to do with the user causing an error

8. What is the difference between a status 200 and a status 201? 201 = created 200 = everything was successful

SOURCE:https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw
       https://azure.microsoft.com/en-us/resources/cloud-computing-dictionary/what-is-middleware/

