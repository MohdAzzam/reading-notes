# Bearer Authorization

1. Register your application to get a client_id and client_secret
2. Ask the client if they want to sign in via a third party
3. Make a request to a third-party API endpoint
4. Make a request to the access token endpoint
5. Receive access token
6. Redirect to a third party authentication endpoint
7. Receive authorization code



- what the user can do 

- allow the user to hit api 

- more security 



### What is JSON Web Token? 

JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA. 


- we can use JWT to Authorization 
  allowing the user to access routes, services, and resources that are permitted with that token.

What is the JSON Web Token structure? 
1. Header : containes the algo and the type
2. Payload: which contains the claims `The User`
3. Signature hash algo base64(header) + payload 

seperated with dot 

aaaaa.bbbbb.ccccc

the user agent sendthe JWT  Authorization header using the Bearer