# Authentication

Authentication is the process of recognizing a user's identity. It is the mechanism of associating an incoming request with a set of identifying credentials.
`Who Are You`

--------------------------------

1. Singleton : One of software design pattern that Restrict the instantiation of the class, to be one instance.

2. We take advantage of Node.JS caching then this is trivial.

3. After reading about the singleton I think we can use the singilton pattern.

--------------------------------

1. Router Middleware : Router-level middleware works in the same way as application-level middleware, except it is bound to an instance of express.Router().

2. Dynamic Module Loading : "Dynamic loading is a mechanism by which a computer program can, at run time, load a library (or other binary) into memory, retrieve the addresses of functions and variables contained in the library, execute those functions or access those variables, and unload the library from memory."
 
3. CRUD -> REST Method Matches

```
       Create = PUT with a new URI POST to a base URI returning a newly created URI
       Read   = GET
       Update = PUT with an existing URI
       Delete = DELETE
```

4. Mock Testing : approach to unit testing that lets you make assertions about how the code under test is interacting with other system modules.

--------------------------------

## Securing Passwords

Password is the first defense against cyber criminals.
and also the password is the final check to get to your any account over intenet
We need to use  hashing algorithm befor we save the passwords to our DB.

Cryptographic hash algorithms MD5, SHA1, SHA256, SHA512, SHA-3 , hashing function

The benefit of hashing is that if someone steals the database with hashed passwords, they only make off with the hashes and not the actual plaintext passwords.



###### PROBLEMS WITH CRYPTOGRAPHIC HASH ALGORITHM

1. Brute Force attack : Attacker can simply keep trying different inputs until he does not find the right now that generates the same hash value 
2. Hash Collision attack:  Hash functions have infinite input length and a predefined output length 


BCrypt, IT's SLOW AND STRONG AS HELL : Bcrypt is an adaptive hash function based on the Blowfish symmetric block cipher cryptographic algorithm and introduces a work factor (also known as security factor), which allows you to determine how expensive the hash function will be.



###### Basic Auth  

provideing a userName and Password when making a request, a request contains a header field in the form of `Authorization: Basic <credentials>`

###### OWASP auth cheatsheet

I hope to know more about this in our class

###### Bcrypt

I hope to know more about this in our class and the Lab 