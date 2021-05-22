# Event Driven Applications

Event-Driven Programming is a logical pattern that we can choose to confine our programming within to avoid issues of complexity and collision.

------------

Every time you interact with a webpage through it’s user interface, an event is happening. When you `click` a button a click event is triggered. When you press a key a `keydown` event is triggered. These events have associated functions that, when triggered, are executed to make a change to the user interface in some way.

Event-Driven Programming makes use of the following concepts:

- An Event Handler is a callback function that will be called when an event is triggered.
- A Main Loop listens for event triggers and calls the associated event handler for that event.

--------------

## EventEmitter 

Node.js natively provides us with a useful module called EventEmitter that allows us to get started incorporating Event-Driven Programming in our project right away. 

We access the `EventEmitter` class through the `events` module. Once imported we’ll need to create a new object from the class to start using it.

-----------------------

Why is access control important? 

To limitations the user previlage in our site To save the secure Data 

Describe an application that would need access control ?
Student Registration system 

What is a role used for? 

what you can do in the system or the website 

Why is role based access control more scalable than discretionary or mandatory access control? 

`Discretionary Access Control provides a much more flexible environment than Mandatory Access Control but also increases the risk that data will be made accessible to users that should not necessarily be given access.`


