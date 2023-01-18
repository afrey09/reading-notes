API Design Best Practices

1. REST stands for Respresentational State Transfer

2. REST APIs are designed around resources. 

3. Resources - any object, data or service a client can access

4. The most common HTTP verbs: GET, POST, PUT, PATCH, DELETE

5. URIs are resource's unique identifies and should therefore be based on the resource it's aimning to identify

6. Example of a good URI : https://adventure-works.com/orders/1

7. A chatty web API refers to having too complex of a URI, which then creates a bigger request/load to impose on the web server. It's best to avoid chatty APIs "that expose a large number of small resources."

8. A successful GET request returns an HTTP status code 200(OK)

9. An unsuccessful GET request can return a 404(NOT FOUND) if the resource cannot be found or an HTTP code 204(NO CONTENT) if there is no response body included in the HTTP response.

10. A successfully created new resources, created by POST, returns an HTTP status code 201(CREATED). "The URI of the new resource is included in the location header of the response."

11. The DELETE operation, when successful, produces an HTTP status code 204(NO CONTENT).

Source: https://learn.microsoft.com/en-us/azure/architecture/best-practices/api-design