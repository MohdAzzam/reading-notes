# Express 

Fast, unopinionated, minimalist web framework for Node.js

-----------------------------


## PUT Vs PATCH 

The main difference between the PUT and PATCH method is that the PUT method uses the request URI to supply a modified version of the requested resource which replaces the original version of the resource, whereas the PATCH method supplies a set of instructions to modify the resource.

-----------------------------

### 3 Services or tools that allow you to “mock” an API for development

1. Nock
2. MockServer
3. Stoplight

-----------------------------
#### APIDoc

`200 ok Successful request and response.`
`400 Bad Request or  Malformed parameters `
`401 Not Authenticated`
`403 Forbidden`
`404 Not found `

```

200	OK	The request was successful.
201	Created	The resource was successfully created.
202	Async created	The resource was asynchronously created
400	Bad request	Bad request
401	Unauthorized	Your API key is invalid.
402	Over quota	Over plan quota on this endpoint.
404	Not found	The resource does not exist.
422	Validation error	A validation error occurred.
429	Too Many Requests	The rate limit was exceeded.
50X	Internal Server Error	An error occurred with our API.

```
#### Swagger

```

        '200':
          description: OK
        '400':
          description: Bad request. User ID must be an integer and larger than 0.
        '401':
          description: Authorization information is missing or invalid.
        '404':
          description: A user with the specified ID was not found.
        '5XX':

```

### SOAP and ReST

SOAP Simple Object Access Protocol.It is a protocol and use xmal from message fromat relies on layer protocols 

REST  Representational State Transfer approach to architectural  

[REST VS SOAP](https://www.youtube.com/watch?v=xq09ow7RuZA)



1. nodejs express js superagent 
2. SOAP and ReST Swagger  APIDoc 
3. everything I read about it today 