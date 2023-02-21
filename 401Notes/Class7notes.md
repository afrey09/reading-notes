Bearer Authorization

Intro to JWT

1. What is a JSON Web Token (JWT)? "JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object"

2. When should we use JSON Web Tokens?
"Authorization: This is the most common scenario for using JWT. Once the user is logged in, each subsequent request will include the JWT, allowing the user to access routes, services, and resources that are permitted with that token. Single Sign On is a feature that widely uses JWT nowadays, because of its small overhead and its ability to be easily used across different domains.

Information Exchange: JSON Web Tokens are a good way of securely transmitting information between parties. Because JWTs can be signed—for example, using public/private key pairs—you can be sure the senders are who they say they are. Additionally, as the signature is calculated using the header and the payload, you can also verify that the content hasn't been tampered with."

3. Claims are expected in which structural component of a JWT? payload 

Are JWTs Secure?

1. If I get a JWT and I can decode the payload, how can we call that secure?

2. If sending a JWT, what must sender and receiver both know? Hint, it’s appended in the signature.

3. Explain how concatenated content and secret can be sent and received securely to a non-technical recruiter.

Videos
JWTs Explained

1. Why use JWT?


2. JWT is Compact and self-contained. Describe how this is useful to a non-technical friend.

3. What are the three components (the structure) of a JWT signature?

sources: