# Props and State 

Does a deployed React application require a server?

You don’t necessarily need a static server in order to run a Create React App project in production. It also works well when integrated into an existing server side app.

Why do we prefer to test a React application at the behavior rather than the unit level?

we need to test the UI 

What does npm run build do?

`npm run build` creates a build directory with a production build of your app. Set up your favorite HTTP server so that a visitor to your site is served index.html, and requests to static paths like


Describe the actual composition / architecture of a React application

`Composition`

 Components written by different people should work well together.


Behavior-driven development

Acceptance Tests

is the system meet the requirment or not 


mounting  ** is the phase in which our React component mounts on the DOM **

build 

--------------------

`setState` is the only legitimate way to update state after the initial state setup.

Handling Events

Handling events with React elements is very similar to handling events on DOM elements. There are some syntax differences:

React events are named using camelCase, rather than lowercase.

With JSX you pass a function as the event handler, rather than a string.


Components let you split the UI into independent, reusable pieces, and think about each piece in isolation

Conceptually, components are like JavaScript functions. They accept arbitrary inputs (called “props”) and return React elements describing what should appear on the screen.

Components can refer to other components in their output
Whether you declare a component as a function or a class, it must never modify its own props

All React components must act like pure functions (do not attempt to change their inputs and always return the same result for the same inputs) with respect to their props
