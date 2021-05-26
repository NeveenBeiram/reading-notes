# OAuth


OAuth is an open standard for access delegation, commonly used as a way for Internet users to grant websites or applications access to their information on other websites but without giving them the passwords.This mechanism is used by companies such as Amazon, Google, Facebook, Microsoft and Twitter to permit the users to share information about their accounts with third party applications or websites.

Generally, OAuth provides clients a "secure delegated access" to server resources on behalf of a resource owner. It specifies a process for resource owners to authorize third-party access to their server resources without providing credentials. Designed specifically to work with Hypertext Transfer Protocol (HTTP), **OAuth** essentially allows access tokens to be issued to third-party clients by an authorization server, with the approval of the resource owner. The third party then uses the access token to access the protected resources hosted by the resource server.[source](https://en.wikipedia.org/wiki/OAuth)


## OAuth 2 Simplified

**Roles:**

* **The Third-Party Application:** "Client"
The client is the application that is attempting to get access to the user's account. It needs to get permission from the user before it can do so.

* **The API:** "Resource Server"
The resource server is the API server used to access the user's information.

* **The Authorization Server**
This is the server that presents the interface where the user approves or denies the request. In smaller implementations, this may be the same server as the API server, but larger scale deployments will often build this as a separate component.

* **The User: "Resource Owner"**
The resource owner is the person who is giving access to some portion of their account.




[What is OAuth Really All About? ](https://www.youtube.com/watch?v=t4-416mg6iU)

[OAuth2 simplified ](https://aaronparecki.com/oauth-2-simplified/)

[ Build a Node API with OAuth ](https://developer.okta.com/blog/2018/08/21/build-secure-rest-api-with-node)

[OAuth wiki ](https://en.wikipedia.org/wiki/OAuth)