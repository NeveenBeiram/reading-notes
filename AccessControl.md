# Access Control (ACL)

* When is Basic Authorization used vs. Bearer Authorization?

in the sign in process, to verify the username and password Bearer Authorization --> after sign in process to ensure that the user still logged in.

* What does the JSON Web Token package do?

JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.

Although JWTs can be encrypted to also provide secrecy between parties, we will focus on signed tokens. Signed tokens can verify the integrity of the claims contained within it, while encrypted tokens hide those claims from other parties. When tokens are signed using public/private key pairs, the signature also certifies that only the party holding the private key is the one that signed it.


* What considerations should we make when creating and storing a SECRET?

Security of the secret (encrypt it)
Save it in an environmental variable (dotenv)

<hr>

### Term

* encryption:is the process of converting data and information into a secret code to hide it's true meaning.

* token:is like a password given to the user that refer that the user has an access or permission to a given operation. it consists of Header (holds the algorithm and type of the token) Payload (information about the user) Signature (token security issues)

* bearer:is an authentication type that holds a token with it and used after the sing in process.

* secret: is a private data between your app/api and the authorization server that grant token only to the eligible users.

* JSON Web Token:: JWT is a package that allow us to define generate and verify tokens to the user.

<hr>

* RBAC = Role Based Access Control
is the idea of assigning system access to users based on their role in an organization. It's important to remember that not every employee needs a starring role.

* ACL ---> is a means of defining access rights by a given user or user group, to a specific object, such as a document. like read only or read and write.

[RBAC tutorial](https://www.youtube.com/watch?v=C4NP8Eon3cA)
[5 steps to RBAC](https://www.csoonline.com/article/3060780/security/5-steps-to-simple-role-based-access-control.html)
[wiki - RBAC](https://en.wikipedia.org/wiki/Role-based_access_control)