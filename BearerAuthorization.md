# Bearer Authorization

* 
    * Ask the client if they want to sign in via a third party
    * Redirect to a third party authentication endpoint
    * Register your application to get a client_id and client_secret
    * Make a request to a third-party API endpoint
    * Receive authorization code
    * Make a request to the access token endpoint
    * Receive access token
* What can you do with an authorization code?
    It allows the user to get access for Tokens
* What can you do with an access token?
   Access tokens are the thing that applications use to make API requests on behalf of a user. The access token represents the authorization of a specific application to access specific parts of a user’s data.
* What’s a benefit of using OAuth instead of your own basic authentication?
    It allows limited access to the user's data and allows accessing when authorization tokens expire. It has ability to share data for users without having to release personal information. It is easier to implement and provides stronger authentication

<hr>

## Term

* Client ID:The client_id is a public identifier for apps. Even though it’s public, it’s best that it isn’t guessable by third parties, so many implementations use something like a 32-character hex string. It must also be unique across all clients that the authorization server handles. If the client ID is guessable, it makes it slightly easier to craft phishing attacks against arbitrary applications.

* Client Secret:he client_secret is a secret known only to the application and the authorization server. It must be sufficiently random to not be guessable, which means you should avoid using common UUID libraries which often take into account the timestamp or MAC address of the server generating it. A great way to generate a secure secret is to use a cryptographically-secure library to generate a 256-bit value and converting it to a hexadecimal representation

* Authentication Endpoint:Endpoint authentication is an authentication mechanism used to verify the identity of a network's external or remote connecting device. These endpoint devices include laptops, smartphones, tablets, and servers. This method ensures that only valid or authorized endpoint devices are connected to a network. These endpoint devices include laptops, smartphones, tablets and servers.

* Access Token Endpoint: is the place where apps make a request to receive access tokens.

* API Endpoint:It is the point of entry in a communication channel when two systems are interacting. source. A route is the name you use to access the endpoint.

* Authorization Code:The authorization code is a temporary code that the client will exchange for an access token. The code itself is obtained from the authorization server where the user gets a chance to see what the information the client is requesting, and approve or deny the request. 

* Access Token: : is an object encapsulating the security identity of a process or thread. A token is used to make security decisions and to store tamper-proof information about some system entity.


<hr>

### JWT (JSON Web Token)

JSON Web Token (JWT) is an open standard (RFC 7519)
compact and self-contained way for securely transmitting information between parties as a JSON object.
digitally signed.
sent through URL, POST request, HTTP Header
can be encrypted to also provide secrecy between parties

<hr>

[JWTs Explained](https://www.youtube.com/watch?v=926mknSW9Lo)

[Intro to JWT](https://jwt.io/introduction/)

[Are JWTs Secure?](https://stackoverflow.com/questions/27301557/if-you-can-decode-jwt-how-are-they-secure)

[npm jsonwebtoken docs](https://www.npmjs.com/package/jsonwebtoken)


