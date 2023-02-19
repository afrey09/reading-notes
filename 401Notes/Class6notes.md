AUTHENTICATION

Securing Passwords

Explain to a non-technical friend how you would safely hash and store a password.

What is Bcrypt? "Bcrypt is an adaptive hash function based on the Blowfish symmetric block cipher cryptographic algorithm and introduces a work factor (also known as security factor)"

Why might you use something like Bcrypt? It is extremely secure again brute force attacks because of the work factor.

Basic Auth

What is Basic Authentication? "a method for an HTTP user agent (e.g. a web browser) to provide a user name and password when making a request"

What properties are necessary in the header of a Basic Auth request? "ID and password joined by a single colon :"
How are username:password in Basic Auth encoded? "...with Base64 in transit and not encrypted or hashed in any way."

OWASP auth cheatsheet

Define the authentication process to a non-technical recruiter. It is the process of ensuring that a user is who they say they are by using a username and password.

How should your error messaging respond (both HTTP and HTML)? Why? "In a generic manner..The objective is to prevent the creation of a discrepancy factor, allowing an attacker to mount a user enumeration action against the application."

Bookmark this link also and consider OWASP fundamentals any time you interact with authentication. Applications developed with security in mind from inception have fewer vulnerabilities throughout their lifecycle.
Authentication - OWASP Cheat Sheet Series

Additional Questions
Looking ahead at this module’s course schedule, What do you look forward to learning?
Role-based authentication

What are your learning goals after reading and reviewing the class README?
To get comfortable in my understanding of authorization

SOURCES:
https://thehackernews.com/2014/04/securing-passwords-with-bcrypt-hashing.html
https://en.wikipedia.org/wiki/Basic_access_authentication

