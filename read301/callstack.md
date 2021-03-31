# Call stack

A **call stack** is a mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions — what function is currently being run and what functions are called from within that function.

------------------------------------------

* When a script calls a function, the interpreter adds it to the call stack and then starts carrying out the function.
* Any functions that are called by that function are added to the call stack further up, and run where their calls are reached.
* When the current function is finished, the interpreter takes it off the stack and resumes execution where it left off in the last code listing.
* If the stack takes up more space than it had assigned to it, it results in a "stack overflow" error.

`function greeting() {
   // [1] Some code here
   sayHi();
   // [2] Some code here
}
function sayHi() {
   return "Hi!";
}

// Invoke the `greeting` function
greeting();

// [3] Some code here`

The code above would be executed like this:

  1. Ignore all functions, until it reaches the `greeting()` function invocation
  2. Add the greeting() function to the call stack list.
    `Call stack list:`
    `- greeting`
  3. Execute all lines of code inside the `greeting()` function.
  4. Get to the `sayHi()` function invocation.
  5. Add the `sayHi()` function to the call stack list.
    Call stack list:
    - sayHi
    - greeting
  6. Execute all lines of code inside the sayHi() function, until reaches its end.
  7. Return execution to the line that invoked sayHi() and continue executing the rest of the `greeting()` function.
  8. Delete the `sayHi()` function from our call stack list.
  9. When everything inside the greeting() function has been executed, return to its invoking line to continue executing the rest of the JS code
  10. Delete the greeting() function from the call stack list.

   ` Call stack list:    EMPTY`


In summary, then, we start with an empty Call Stack. Whenever we invoke a function, it is automatically added to the Call Stack. Once the function has executed all of its code, it is automatically removed from the Call Stack. Ultimately, the Stack is empty again.


------------------------- 

The call stack is primarily used for function invocation (call). Since the call stack is single, function(s) execution, is done, one at a time, **from top to bottom**. It means the call stack is `synchronous`.

In Asynchronous JavaScript, we have a callback function, an event loop, and a task queue. The callback function is acted upon by the call stack during execution after the call back function has been pushed to the stack by the event loop.

At the most basic level, a call stack is a data structure that uses the` Last In, First Out (LIFO)` principle to temporarily store and manage function invocation (call).


*LIFO*: When we say that the call stack, operates by the data structure principle of Last In, First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.

Manage function invocation (call): The call stack maintains a record of the position of each stack frame. It knows the next function to be executed (and will remove it after execution). This is what makes code execution in JavaScript synchronous.

**What causes a stack overflow?**
A stack overflow occurs when there is a `recursive function` (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.

Here is an example:

function callMyself(){
  callMyself();
}

callMyself();
The callMyself() will run until the browser throws a “Maximum call size exceeded”. And that is a stack overflow.

##### In summary

The key takeaways from the call stack are:
1. It is single-threaded. Meaning it can only do one thing at a time.
2. Code execution is synchronous.
3. A function invocation creates a stack frame that occupies a temporary memory.
4. It works as a LIFO — Last In, First Out data structure.


#### Reference errors

* This is as simple as when you try to use a variable that is not yet declared you get this type os errors.
* when using const and let, they are hoisted like var and function but there is a time between the hoisting and being declared so when you try to access them a reference error occurs, is called **Temporal Dead Zone**.


#### Syntax errors

* This occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.


#### Range errors

* when you try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.

#### Type errors

* This types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.

## Debugging


* The easiest and maybe the most common way its to simply `console.log()` the variables you want to check or, by using chrome developer tools, open your page with your JS code (press `cmd+o` in macOS or `Ctrl+o` in Windows) and choose your file to debug, click the line you wanna debug and refresh your page again (`F5`).
* The breakpoint can also be achieved by putting a debugger statement in your code in the line you want to break.
* Using Node.js with Visual Studio Code you can press the debug tab and add a configuration You can run the debugger by pressing `F5` or pressing the green play button.

#### Handling errors

* we usually `try` to `catch` the errors so we can gracefully fallback to a default state of our application in case of an error (this fallback can be a 404 page which is normally not that graceful but is better than a page to just stop working).

#### Tools to avoid runtime errors

you can use tools like:
* quokka to evaluate your code as you type.
* eslint to make sure your style guide is consistency and it will grab you an error or two along the way.
* You can check out stuff like TypeScript.
