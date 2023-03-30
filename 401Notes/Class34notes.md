API Integration

Review API Server Build

1. Explain the difference between a query string and a path parameter.
   Path parameters are used to determine a specific location for you program to look (i.e the endpoint). Query strings are used to filter the results of the query. The query string also appears after the ? in a URL and the path parameter appears before.


2. What would our API URL with a path id parameter be given the following information:
  1. Domain: http://our-site.com
  2. v3
  3. model name: stuff
  4. id: things
  http://our-site.com/v3/stuff/things

3. We have created a dynamic API with an “interface”. Describe how the interface works to a non-technical friend. The interface works by taking in a request and returnining a response. It allows the user to interact with the API.


Review Auth Server Build

1. Describe how you would use middleware to implement basic and bearer auth. You would use middleware to implement basic and bearer auth by using the middleware to check the request for the correct authorization header. If the header is not present, the middleware would return a 401 error. If the header is present, the middleware would check the header for the correct credentials. If the credentials are not correct, the middleware would return a 401 error. If the credentials are correct, the middleware would allow the request to continue.

2. Describe the handshake necessary to implement OAuth. The handshake necessary to implement OAuth is the user is redirected to the OAuth provider to authorize the application. The user is then redirected back to the application with an authorization code. The application then exchanges the authorization code for an access token. The application then uses the access token to make requests to the API.

3. Describe how Role Based Access Control works to a non-technical friend. Role Based Access Control allows you to assign permissions to users based on their role. For example, you could have a teacher with access to a student's file where they're able to read and update grades. The student however, or their parent, only has the access to read the grades.
