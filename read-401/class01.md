# Node Ecosystem, TDD, CI/CD

## Node Ecosystem

Since it’s inception in 1995, JavaScript has massively evolved and is one of the most widely-used programming languages

The JavaScript ecosystem is huge I read about this stuff and this is the description from the documentation

##### So what is JavaScript?

JavaScript is a lightweight, interpreted, prototype-based, multi-paradigm scripting language that is dynamic, and supports object-oriented, imperative, and functional programming styles.
JavaScript initially started as a language for the web browser, developed by Brendan Eich in 1995. Today JavaScript is one of the most influential languages, which has spread its roots into the backend and mobile development, machine learning, and many other branches.
In 2009, Ryan Dahl developed a JavaScript runtime called Node.js, which pushed the JavaScript language into a whole new direction. This lead to the creation of the first JavaScript Stack. No longer was JavaScript used only for animations and UI manipulation. With new inventions also came new problems and the right tools to solve them.

##### Node.js and NPM

Node.js is an open-source, cross-platform, JavaScript runtime environment that executes JavaScript code outside of a web browser. It’s built upon Chrome’s V8 JavaScript engine and is designed to build scalable and real-time network applications.
Npm (Node Package Manager) is the largest ecosystem of open source libraries in the world. Npm is a package manager for the JavaScript language and is the default package manager for the JavaScript runtime environment Node.js.
It consists of a command-line client, also called npm, and an online database of public and paid-for private packages called the npm registry.
The npm registry has become the center of JavaScript code sharing, and with more than one million packages, and many more are added every day.
Package Managers
A package manager or package management system is a collection of software tools that automates the process of installing, upgrading, configuring, and removing computer programs for a computer’s operating system in a consistent manner.
It’s no secret that npm is quite a popular package manager, but it’s not the only one. There is also a Bower and nowadays you’ll often come across Yarn as well.
The way a package manager works is you find any package in the registry and install it through the command-line, both globally and locally. The package manager does all the required setup for you. Then you can use this package in any Node.js or React or Angular app. You name it.
Each of these package managers has one goal, to set up a third-party module, but does so in a different manner.
With so many modules at hand, how do you know which one to choose? Behold Npm Trends. Npm Trends is a site that shows statistics of each package and also allows us to compare number downloads for different modules.

## Test Driven Development

Test-Driven-Development (TDD) is an increasingly popular, and practical, development methodology in today’s software industry, and it is easy to apply in Node.js.TDD forces much greater code test coverage


The process is: define a test that expects the output we want from our library, API, or whatever it is we’re testing to produce; ensure that the test fails – because we have not yet implemented any functionality; then write the implementation code required to make that test pass.

Modern languages and testing frameworks make this easy to achieve, and we’ve evolved to the point in technology where we can write concise, easily maintainable tests before even thinking about writing implementation code.

Node.js is quickly becoming a language of choice for REST API development, and Express has established itself as an almost de-facto standard web framework of choice. It allows us to build a RESTful web page capable of serving both HTML content and an API, along with much more besides.

One of the most important first steps when building an Express project is to test the APIs you create, and ensure they return what you expect.


----------------------------------------------------------

## continuous integration and continuous deployment

This work done via DevOps Engineer. 

Code=> Build=> Test=> Deploy=> Provision 

Helpful YouTube links:
1. [What is CICD?](https://www.youtube.com/watch?v=N9KbmHhesmE)

2. [DevOps CI/CD Explained in 100 Seconds](https://www.youtube.com/watch?v=scEDHsr3APg)

----------------------------------------------------------

## Array.map()

`map()` Manipulate the data from the array and set them into a new `Array` with the same length of orginal array also without changing the data in the original array that we send.
the map calls a provided callback function once for each element in an array, in order, and constructs a new array from the results. a callback is invoked only for indexes of the array which have assigned values (including `undefined`).

> *example*:`let numberArray=[1,2,3];` to map this array we use the method map like this `let increseValueByOne= numberArray.map(item=>item+1)`
there are two way to return the data to the new array like in the example we used implecit return  or we can use `let increseValueByOne= numberArray.map(item=>{return item+1})`

for more information visit this link [Array map()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map)
or Google it bro :p

-----------------------------------

## Array.reduce()

`reduce()` it will reduce the all data in array to one value called accumulator the accumulator can be anything (array[],string'',object {}...)
*example*:`let numberArray=[1,2,3];` to reduce this array we use our method reduce like this
`numberArray.reduce((accumulator, value) => {return accumulator + value;}, 0);`
we initalize the accumulter with 0 the return data of this function should be 6 

for more information visit this link [Array reduce()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/Reduce)
or Google it bro :p

-----------------------------------

## superagent()

> With normal Promise `.then`
```
let cityNormalPromis =(name)=>{
  superagent.get(`https://geocode.xyz/${name}?json=1`)
  .then(result=>{
    console.log(result.body);
  }).catch(err=>console.error(err))
}
```

-----------------------------------

> With `async` / `await` syntax
```
async function city(name){
  try{
    let data=await superagent.get(`https://geocode.xyz/${name}?json=1`);
    console.log(name,': latitude: ',data.body.latt , 'longitude: ', data.body.longt);

  }
  catch(e){
    console.error('ERROR While you call ')
    }
  }

city('seattle');
city('amman');
city('irbid');
```

-----------------------------------

## Promise
Promise is Async function handel resolve and reject data.
A promise says, “Hey, Javascript, you go ahead and do some work. I don’t care how long it takes and I’m going to go ahead and keep working … but let me know when you’re done .then() give me the data and let me deal with it myself ”
for more information watch this video [Promise](https://www.youtube.com/watch?v=4bPdjAerRzQ)
or Google it bro :p

-----------------------------------

## Are all callback functions considered to be Asynchronous? Why or Why Not?

The only way you know whether a callback is asynchronous is from its documentation. Typically, ones involving requests for external resources (ajax calls, for instance) are asynchronous, and others may or may not be.

"Simply taking a callback doesn't make a function asynchronous. There are many examples of functions that take a function argument but are not asynchronous. For example there's forEach in Array. It iterates over each item and calls the function once per item."

this qoute from this article [is all Callback considered Asynchronous](https://bytearcher.com/articles/does-taking-a-callback-make-a-function-asynchronous/)
