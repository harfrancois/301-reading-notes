# CRUD

source: https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/

# In your own words, describe what each group of status code represents:

#### 100’s

There is something wrong with the request that's being made. 

#### 200’s

Its green and good to go.

#### 300’s

what your looking for is not available any more.

#### 400’s

Invalid request made.

#### 500’s

Server error 

#### What is a status code 202?

It’s the basic status code to tell the client everything went good. 

#### What is a status code 308?

This tells the client to use another URL to access the resource and not use the current URL anymore. It’s helpful when we have multiple endpoints for one resource, but don’t want to implement reading from all of them.

#### What code would you use if an update didn’t return data to a client?

204 No Content

#### What code would you use if a resource used to exist but no longer does?

code 410

#### What is the ‘Forbidden’ status code?

code 403

# Build A REST API With Node.js, Express, & MongoDB - Quick

#### Why do we need to pull our MongoDB database string out of our server and put it into our .env?

lets us connect to the database

#### What is middleware?

code that receives your request before it gets to the server.

#### What does app.use(express.json()) do?

Lets you  use json as the body to our request.

#### What does the /:id mean in a route?

It's a parameter.

#### What is the difference between PUT and PATCH?

PUT updates all the information but PATCH updates only specific information.

#### How do you make a default value in a schema?

You would create a key value then a type and required.

#### What does a 500 error status code mean?

Code 500 means server error

#### What is the difference between a status 200 and a status 201?

Code 200 means request is understood and is being process and a 201 means request has been processed.
