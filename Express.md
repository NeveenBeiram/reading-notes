![express](./express.png)

## What’s the difference between PUT and PATCH?

* ***PUT***  

    is used to update (modifies) the entire resource data .

* ***PATCH*** 

    applies a partial update to the resource,so you can update one value and it won’t affect or change anything else.

<hr>

## Provide links to 3 services or tools that allow you to “mock” an API for development like json-server?

1. ***[Postman](https://www.postman.com/features/mock-api/)***

2. ***[mockoon](https://mockoon.com/)***

3. ***[Stoplight](https://stoplight.io/)***

<hr>

## Compare and contrast Swagger and APIDoc.js 1 Which HTTP status codes should be sent with each type of (un)successful API call?

* ***Swagger*** Test and Document Your APIs , free cloud-based API testing and documentation tool to simplify the validation of any API and generate its corresponding OpenAPI documentation.

* ***APIDoc.js*** Inline Documentation for RESTful web APIs. It creates a documentation from API annotations in your source code.


<hr>

## Compare and contrast SOAP and ReST
<!-- 
SOAP and REST both allow you to create your own API, it possible to transfer data from an application to other applications.

* **SOAP** is a standardized protocol that sends messages using other protocols such as HTTP and SMTP. As SOAP is an official protocol, it comes with strict rules and advanced security features. Higher complexity, it requires more bandwidth and resources which can lead to slower page load times.

* **REST** stands for Representational State Transfer. It’s an architectural style that defines a set of recommendations for designing loosely coupled applications that use the HTTP protocol for data transmission. REST doesn’t prescribe how to implement the principles at a lower level.

//// -->
SOAP stands for Simple Object Access Protocol, it was designed before REST, and it allows programs built on different platforms and languages to exchange data in an easy manner.

REST stands for Representational State Transfer, it is an architectural style that uses HTTP verbs of GET, POST, PUT, DELETE to work with the required components.

SOAP needs more bandwidth than REST, since its messages contain a lot of information... which also makes REST far easier to write.

SOAP offers additional features when it comes to security. Also, SOAP is better for stateful operations.