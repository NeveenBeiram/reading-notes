# Authentication 

1. Explain what a “Singleton” is (in Computer Science terms)

In software engineering, the singleton pattern is a software design pattern that restricts the instantiation of a class to one "single" instance. This is useful when exactly one object is needed to coordinate actions across the system. The term comes from the mathematical concept of a singleton.
[source](https://en.wikipedia.org/wiki/Singleton_pattern)

2. Explain how the Singleton pattern can be used with Node modules, specifically with classes
Hide the constructor of the class.
Define a public static operation (getInstance()) that returns the sole instance of the class.

3. If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?

Middleware functions are functions that have access to the request object (req), the response object (res), and the next middleware function in the application’s request-response cycle. The next middleware function is commonly denoted by a variable named next.

[source](https://medium.com/@selvaganesh93/how-node-js-middleware-works-d8e02a936113)

## Term

* Router Middleware:It is a function that comes between the request and the response and can modify the data, then calls the next middleware or the endpoint function.

* Dynamic Module Loading:Dynamic loading is a mechanism by which a computer program can, at run time, load a library (or other binary) into memory, retrieve the addresses of functions and variables contained in the library, execute those functions or access those variables, and unload the library from memory. Applications can still operate and run without these dependencies or modules, and they are only imported and injected into the application when only needed.

* Singleton Pattern:A singleton is a software engineering design pattern that uses the single instance of a class to control the instantiation of objects from the class. We can't create more than one instance of the class, and all programming operations done by the class are managed through this single instance.

* CRUD -> REST Method Matches:create --> POST, read --> GET, update --> PUT/PATCH, delete --> DELETE

* Mock Testing:It is a way to perform unit tests for functions that require specific operations before and after they are called. We mock some functions to eliminate the logging effect to the console so it won't be crowded with unnecessary messages. There are many uses for mock tests, like using it to test server routes without having the server run on a specific port.
 (simulate the behavior of the real ones).




<hr>

* Securing Passwords:

Passwords are the first line of defense against cyber criminals. It is the most vital secret of every activity we do over the internet and also a final check to get into any of your user account, whether it is your bank account, email account, shopping cart account or any other account you have.
We all know storing passwords in clear text in your database is ridiculous. Many desktop applications and almost every web service including, blogs, forums eventually need to store a collection of user data and the passwords, that has to be stored using a hashing algorithm.
Cryptographic hash algorithms MD5, SHA1, SHA256, SHA512, SHA-3 are general purpose hash functions, designed to calculate a digest of huge amounts of data in as short a time as possible. Hashing is the greatest way for protecting passwords and considered to be pretty safe for ensuring the integrity of data or password.

* Basic Auth: 
In the context of an HTTP transaction, basic access authentication is a method for an HTTP user agent (e.g. a web browser) to provide a user name and password when making a request. In basic HTTP authentication, a request contains a header field in the form of `Authorization: Basic <credentials>`, where credentials is the Base64 encoding of ID and password joined by a single colon :.

* OWASP auth cheatsheet:Authentication is the process of verifying that an individual, entity or website is whom it claims to be. Authentication in the context of web applications is commonly performed by submitting a username or ID and one or more items of private information that only a given user should know.

Session Management is a process by which a server maintains the state of an entity interacting with it. This is required for a server to remember how to react to subsequent requests throughout a transaction. Sessions are maintained on the server by a session identifier which can be passed back and forward between the client and server when transmitting and receiving requests. Sessions should be unique per user and computationally very difficult to predict.

* bcrypt docs:library helps in hashing passwords. 

### sources :

[Securing Passwords](https://thehackernews.com/2014/04/securing-passwords-with-bcrypt-hashing.html)
[Basic Auth](https://en.wikipedia.org/wiki/Basic_access_authentication)
[OWASP auth cheatsheet](https://www.owasp.org/index.php/Authentication_Cheat_Sheet)
[bcrypt docs](https://www.npmjs.com/package/bcrypt)