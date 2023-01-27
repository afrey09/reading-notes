OAuth

What is OAuth?
  "OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential. In authentication parlance, this is known as secure, third-party, user-agent, delegated authorization"

Give an example of what using OAuth would look like.
  When you log onto a website and it gives you the option to log on using another website's service login. For example, when you can use GitHub or Google to sign into Render

How does OAuth work? What are the steps that it takes to authenticate the user?

  1. The first website connects to the second website on behalf of the user, using
   OAuth, providing the user’s verified identity.
  2. The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
  3. The first site gives this token and secret to the initiating user’s client software.
  4. The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
  5. If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.
  6. The user approves (or their software silently approves) a particular transaction type at the first website.
  7. The user is given an approved access token (notice it’s no longer a request token).
  8. The user gives the approved access token to the first website.
  9. The first website gives the access token to the second website as proof of authentication on behalf of the user.
  10. The second website lets the first website access their site on behalf of the user.
  11. The user sees a successfully completed transaction occurring.
  12. OAuth is not the first authentication/authorization system to work this way on behalf of the end-user. In fact, many authentication systems, notably Kerberos, work similarly. What is special about OAuth is its ability to work across the web and its wide adoption. It succeeded with adoption rates where previous attempts failed (for various reasons)."

What is OpenID?
  "OpenID is for humans logging into machines, OAuth is for machines logging into machines on behalf of humans." It is about authentication using security technology

Source: <https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html>

What is the difference between authorization and authentication?
  "authentication is the process of verifying who a user is"
  "authorization is the process of verifying what they have access to"

What is Authorization Code Flow? It exchanges authorization for a token. The flow can be defined as the following steps.. 
  " (A)  The client initiates the flow by directing the resource owner's
        user-agent to the authorization endpoint.  The client includes
        its client identifier, requested scope, local state, and a
        redirection URI to which the authorization server will send the
        user-agent back once access is granted (or denied).

   (B)  The authorization server authenticates the resource owner (via
        the user-agent) and establishes whether the resource owner
        grants or denies the client's access request.

   (C)  Assuming the resource owner grants access, the authorization
        server redirects the user-agent back to the client using the
        redirection URI provided earlier (in the request or during
        client registration).  The redirection URI includes an
        authorization code and any local state provided by the client
        earlier.

   (D)  The client requests an access token from the authorization
        server's token endpoint by including the authorization code
        received in the previous step.  When making the request, the
        client authenticates with the authorization server.  The client
        includes the redirection URI used to obtain the authorization
        code for verification.

   (E)  The authorization server authenticates the client, validates the
        authorization code, and ensures that the redirection URI
        received matches the URI used to redirect the client in
        step (C).  If valid, the authorization server responds back with
        an access token and, optionally, a refresh token."


What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?
  "The PKCE-enhanced Authorization Code Flow introduces a secret created by the calling application that can be verified by the authorization server; this secret is called the Code Verifier. Additionally, the calling app creates a transform value of the Code Verifier called the Code Challenge and sends this value over HTTPS to retrieve an Authorization Code. This way, a malicious attacker can only intercept the Authorization Code, and they cannot exchange it for a token without the Code Verifier"

What is Implicit Flow with Form Post?
  "As an alternative to the Authorization Code Flow, OAuth 2.0 provides the Implicit Flow, which is intended for Public Clients, or applications which are unable to securely store Client Secrets. While this is no longer considered a best practice for requesting Access Tokens, when used with Form Post response mode, it does offer a streamlined workflow if the application needs only an ID token to perform user authentication"

What is Client Credentials Flow?
  "M2M apps use the Client Credentials Flow in which they pass along their Client ID and Client Secret to authenticate themselves and get a token."

What is Device Authorization Flow?
  "The Device Authorization Flow contains two different paths; one occurs on the device requesting authorization and the other occurs in a browser. The browser flow path, wherein a device code is bound to the session in the browser, occurs in parallel to part of the device flow path."

What is Resource Owner Password Flow?
  "Though we do not recommend it, highly-trusted applications can use the Resource Owner Password Flow (defined in OAuth 2.0 RFC 6749, section 4.3), which requests that users provide credentials (username and password), typically using an interactive form. Because credentials are sent to the backend and can be stored for future use before being exchanged for an Access Token, it is imperative that the application is absolutely trusted with this information.

Even if this condition is met, the Resource Owner Password Flow should only be used when redirect-based flows (like the Authorization Code Flow) cannot be used."

Source:<https://auth0.com/docs/get-started/authentication-and-authorization-flow>
