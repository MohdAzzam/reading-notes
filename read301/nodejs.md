# Node Js 

Node.js® is a JavaScript runtime built on Chrome’s V8 JavaScript engine

Node.js is an event-based, non-blocking, asynchronous I/O runtime that uses Google's V8 JavaScript engine and libuv library. It is used for developing applications that make heavy use of the ability to run JavaScript both on the client, as well as on server side and therefore benefit from the re-usability of code and the lack of context switching.

However, when we say that Node is built on the V8 engine, we don’t mean that Node programs are executed in a browser. They aren’t. Rather, the creator of Node (Ryan Dahl) took the V8 engine and enhanced it with various features, such as a file system API, an HTTP library, and a number of operating system–related utility methods.

-----------------------------

#### How Do I Install Node.js? 

From the official Node download page [Node Website](https://nodejs.org/en/download/)

after download the node from the webiste and install it in your own device run this command on CLI to check 
the version of the node `node -v`

you can write your JavaScript using the latest and most modern syntax. It also means that you don’t generally have to worry about compatibility issues — as you would if you were writing JavaScript that would run in different browsers.

---------------------------

##### Introducing npm, the JavaScript Package Manager

 Node comes bundled with a package manager called npm. To check which version you have installed on your system, type `npm -v`.


there is two way to install `npm` 
1. Installing a Package Locally
2. Installing a Package Globally 


when we install a packge `npm install lodash --save` 
This will create and auto-populate a package.json file in the same folder. Next, use npm


#### What Is Node.js Used For? 

To ease the development of complex JavaScript further, Node.js supports the CommonJS standard that allows for modularized development and the distribution of software in packages via the Node Package Manager (NPM).

-------------------

#### The Node.js Execution Model

In very simplistic terms, when you connect to a traditional server, such as Apache, it will spawn a new thread to handle the request. In a language such as PHP or Ruby, any subsequent I/O operations (for example, interacting with a database) block the execution of your code until the operation has completed. That is, the server has to wait for the database lookup to complete before it can move on to processing the result. If new requests come in while this is happening, the server will spawn new threads to deal with them. This is potentially inefficient, as a large number of threads can cause a system to become sluggish — and, in the worst case, for the site to go down. The most common way to support more connections is to add more servers.

Node.js, however, is single-threaded. It’s also event-driven, which means that everything that happens in Node is in reaction to an event. For example, when a new request comes in (one kind of event) the server will start processing it. If it then encounters a blocking I/O operation, instead of waiting for this to complete, it will register a callback before continuing to process the next event. When the I/O operation has finished (another kind of event), the server will execute the callback and continue working on the original request. Under the hood, Node uses the libuv library to implement this asynchronous (that is, non-blocking) behavior.

Node’s execution model causes the server very little overhead, and consequently it’s capable of handling a large number of simultaneous connections. The traditional approach to scaling a Node app is to clone it and have the cloned instances share the workload. Node.js even has a built-in module to help you implement a cloning strategy on a single server.

Downsides 
>The fact that Node runs in a single thread does impose some limitations. For example, blocking I/O calls should be avoided, CPU-intensive operations should be handed off to a worker thread, and errors should always be handled correctly for fear of crashing the entire process.



this is the way to create a Server in node js 
`const http = require('http');

http.createServer((request, response) => {
  response.writeHead(200);
  response.end('Hello, World!');
}).listen(3000);

console.log('Server running on http://localhost:3000'); `


##### What Kind of Apps Is Node.js Suited To? 

Static file servers
Web Application frameworks
Messaging middleware
Servers for HTML5 multi player games, or streaming audio/video
Real time applications
Cross-platform programs


JavaScript is everywhere, and Node is a vast and expansive subject. Nonetheless, I hope that in this article I’ve offered you the beginner-friendly, high-level look at Node.js and its main paradigms that I promised at the beginning. I also hope that when you re-read the definitions we looked at previously, things will make a lot more sense.

---------------------------------
 
#  Express

` npm install express --save ` 

Fast, unopinionated, minimalist web framework for Node.js
* Web Applications 
 Express is a minimal and flexible Node.js web application framework that provides a robust set of features for web and mobile applications.
* APIs 
  With a myriad of HTTP utility methods and middleware at your disposal, creating a robust API is quick and easy.
* Performance 
  Express provides a thin layer of fundamental web application features, without obscuring Node.js features that you know and love.

---------------------- 

## API

 is the acronym for Application Programming Interface, which is a software intermediary that allows two applications to talk to each other. Each time you use an app like Facebook, send an instant message, or check the weather on your phone, you’re using an API. 

 