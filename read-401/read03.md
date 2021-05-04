# Express REST API 

Express is one of the most popular http server framework for node js we can customize any thing using the middleware

REST API  is set of methods that clients can request information from the server via the HTTP protocol 


Middleware acts almost like extensions and provides additional functionalities in the `middle` of a request.


1. auth
2. 404 and 500 errors 
3. access database 

----------- 


2. true 
3. next
4. befor the route handler
5. if you are in the body and want to send another res


Request Object :  The req object represents the HTTP request and has properties for the request query string, parameters, body, HTTP headers

Response Object : will be emitted from the request object when the response headers have been received.

Application Middleware : app.use(thismiddlware)

Routing Middleware : for specific route