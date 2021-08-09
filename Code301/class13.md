# CRUD:
 Each group of status code represents:
 1. 100s: These are informational status codes; they usually tell the client that the header part of the request has been received and the server will try to comply with a transmission demand of the client.
 2. 200s: These are the success codes. They tell the client that its request was accepted. In case of asynchronous processing of a request (202), this doesn’t mean the request was successfully processed only that it met all validation requirements at the time of sending.
3. 300s: These are redirection codes. They tell the client that the resource they are requesting isn’t available at the expected location anymore. 
4. 400s: These are the client error codes. They are all about invalid requests a client sent to a server. There are several causes to this, timeouts, wrong URI, missing authentication.
5. 500s: These are the server error codes. Often they indicate problems with overwhelmed servers or unreachable servers behind proxies, but sometimes they can be directly related to client requests that trigger error exceptions on the server. 

## What is a status code 202?:
Often used for asynchronous processing. This code tells the client that the request was valid, but its processing will finish sometime in the future. The response body should include an URL to the finished resource with some information about when it will be available.

## What is a status code 308?:
This tells the client to use another URL to access the resource and not use the current URL anymore. It’s helpful when we have multiple endpoints for one resource.

## What code would you use if an update didn’t return data to a client?
An update can be implemented with an HTTP PUT or PATCH method. The difference lies in the amount of data the client has to send to the backend.PUT requires the client to send an entire representation of a resource to update it. (Replace the old one with the new one).
PATCH requires the client only send parts of the representation of the resource to update it. (Add, update or delete these parts in the old version).

## What code would you use if a resource used to exist but no longer does?
A 204, ‘No Content’ error. For things like saving something they have just changed.

## What is the ‘Forbidden’ status code?
410 Gone 6

## Build A REST API With Node.js, Express, & MongoDB

## Why do we need to pull our MongoDB database string out of our server and put it into our .env?

This is because when working on the code locally, you want to store the database as a local environment variable. This adds security and flexibility

## What is middleware?
is software that provides common services and capabilities to applications outside of what's offered by the operating system.

## What does app.use(express.json()) do?
it is a method inbuilt in express to recognize the incoming Request Object as a JSON Object.

## What does the /:id mean in a route?
params object, with the name of the route parameter specified in the path as their respective keys

## What is the difference beween PUT and PATCH?
The main difference between the PUT and PATCH method is that the PUT method uses the request URI to supply a modified version of the requested resource which replaces the original version of the resource, whereas the PATCH method supplies a set of instructions to modify the resource.

## How do you make a defalut value in a schema?
Make mongoose string schema type default value as blank and make the field optional.

## What does a 500 error status code mean?
A 500 error means that there has been an error on the server. This is good to be placed within the catch of a try/catch statement, because if it fails, something is wrong within that function.

## What is the difference between a status 200 and a status 201?
201: successfully created object 200: everything was successful The 201 is more specific, so if it can be used, for example in a post route, it should be used. More information is always better!