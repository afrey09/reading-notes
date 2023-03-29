Login and Auth

What is Role Based Access Control (RBAC)?  Where certain access is restricted based on someone's role. (Ie only teacher's being able to access where grades are updated)

Share some an example of RBAC including all possible CRUD operations and correlating roles.
  - A teacher can update/read a student's file
  - A student/parent can read their report
  - An administrator can have all crud access 


What are the Benefits of RBAC?
  - Reducing administrative work and IT support
  - Maximizing operational efficiency.
  - Improving compliance.

Compare and Contrast the following two Libraries and the following questions. Yes, they are similarly named.

react-cookie library

react-cookies component

Describe some react-cookie features.

    get(name, [options])
    Get a cookie value
      -name (string): cookie name
      -options (object):
        doNotParse (boolean): do not convert the cookie into an object no matter what
    
    getAll([options])
    Get all cookies
      -options (object):
        doNotParse (boolean): do not convert the cookie into an object no matter what

    set(name, value, [options])
    Set a cookie value
      -name (string): cookie name
      -value (string|object): save the value and stringify the object if needed
      -options (object): Support all the cookie options from RFC 6265
          -path (string): cookie path, use / as the path if you want your cookie to be accessible on all pages
          -expires (Date): absolute expiration date for the cookie
          -maxAge (number): relative max age of the cookie from when the -client receives it in seconds
          -domain (string): domain for the cookie (sub.domain.com or .allsubdomains.com)
          -secure (boolean): Is only accessible through HTTPS?
          -httpOnly (boolean): Can only the server access the cookie? Note: You cannot get or set httpOnly cookies from the browser, only the server.
          -sameSite (boolean|none|lax|strict): Strict or Lax enforcement

    
    remove(name, [options])
    Remove a cookie
      -name (string): cookie name
      -options (object): Support all the cookie options from RFC 6265
        -path (string): cookie path, use / as the path if you want your cookie to be accessible on all pages
        -expires (Date): absolute expiration date for the cookie
        -maxAge (number): relative max age of the cookie from when the client receives it in seconds
        -domain (string): domain for the cookie (sub.domain.com or .allsubdomains.com)
        -secure (boolean): Is only accessible through HTTPS?
        -httpOnly (boolean): Can only the server access the cookie? Note: You cannot get or set httpOnly cookies from the browser, only the server.
        -sameSite (boolean|none|lax|strict): Strict or Lax enforcement


Describe some react-cookies features.

  -.load(name, [doNotParse])
Load the cookie value.
Returns undefined if the cookie does not exist.
Deserialize any cookie starting with { or [ unless dotNotParse is true.
  -.loadAll()
Load all available cookies.
Returns an object containing all cookies.
  -.select([regex])
Find all the cookies with a name that match the regex.
Returns an object with the cookie name as the key. 
  -.save(name, value, [options])
Set a cookie.
  -.remove(name, [options])
Remove a cookie.
  -.plugToRequest(req, res): unplug()
Load the user cookies so you can do server-rendering and match the same result.
  -.setRawCookie(cookies)
Load the user cookies so you can do server-rendering and match the same result.
Also send back to the user the new cookies.


Which library would you prefer would you prefer? Why? react-cookie because it seems easier to use and was more recently published than react-cookies.

source: 
https://www.digitalguardian.com/blog/what-role-based-access-control-rbac-examples-benefits-and-more
npmjs.com/package/react-cookie
https://www.npmjs.com/package/react-cookies
