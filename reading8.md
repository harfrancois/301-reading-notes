# API Design Best Practices

source: https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design

## What does REST stand for?

Representational State Transfer.

## REST APIs are designed around a?

resources

## What is an identifer of a resource? Give an example.

A resource has an identifier, which is a URI that uniquely identifies that resource. For example, the URI for a particular customer order.
https://adventure-works.com/orders/1


## What are the most common HTTP verbs?

GET, POST, PUT, PATCH, and DELETE.

## What should the URIs be based on?

 URIs should be based on nouns (the resource) and not verbs (the operations on the resource).

## Give an example of a good URI.

https://adventure-works.com/orders // Good

## What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

APIs that expose a large number of small resources. Its bad because of the load size impose on the server.

## What status code does a successful GET request return?

A successful GET method typically returns HTTP status code 200 (OK).

## What status code does an unsuccessful GET request return?

Return 404 (Not Found).

## What status code does a successful POST request return?

Returns HTTP status code 201 (Created).

## What status code does a successful DELETE request return?

Return HTTP 404 (Not Found).