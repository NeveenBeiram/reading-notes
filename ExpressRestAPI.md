# ExpressRestAPI.md 

## Name 3 real world use cases where you’d want to change the request with custom middleware

1. Encrypting a password or sensitive information.

2. Using methodOverride to utilize put and delete methods instead of post.

3. when we want to handle errors and reform the error to show message as we want.

## True or false: The route handler is middleware? 
False

## In what ways can a middleware function end the process and send data to the browser?
By sending a response and not using next();... or by passing a parameter in next() which will use an error handler.

## At what point in the request lifecycle can you “inject” middleware?

Anywhere before reaching the final function (the handler) which is the end point.

## What can cause express to error with “Request headers sent twice, cannot start a second response

if the we are in the Body or Finished state, but some function tried to set a header or statusCode.

## Terms

* Middleware :Middleware is software that provides common services and capabilities to applications outside of what's offered by the operating system. Data management, application services, messaging, authentication, and API management are all commonly handled by middleware.

* Request Object : The request object represents the HTTP request and has properties for the request query string, parameters, body, HTTP headers

* Response Object : The response object represents the HTTP response that an Express app sends when it gets an HTTP request.

* Application Middleware : Application-level-middleware are functions are bound to an instance of the app object by using `app.use` and `app.METHOD()` functions... these functions have no mount path and are executed every time the app receives a request.

* Routing Middleware : Router-level middleware works in the same way as application-level middleware, except it is bound to an instance of `express.Router()`

* Test Driven Development :It is a software development approach where each functionality is tested and validated...

 failed tests should be re-written until they pass before proceeding with writing new code.

* Behavioral Testing : It is mainly focused on the behavior of users rather than the technical functions of the software.


[Review: ES6 Classes](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes)

[Using Express Routing](https://expressjs.com/en/guide/routing.html)

[Express Routing](https://scotch.io/tutorials/learn-to-use-the-new-router-in-expressjs-4)





