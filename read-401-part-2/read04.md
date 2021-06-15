# Routing 

Do child components have direct access to props/state from the parent? 

No 

When a component “wraps” another component, how does the child component’s output get rendered?

Concretely, a higher-order component is a function that takes a component and returns a new component.


Can a component, such as `<Content />`, which is a child also be used as a standalone?
The stand alone component have no parent

listing them out individually as the new props for the child component. 

## React Router  

    React Router has been broken into three packages: react-router, react-router-dom, and react-router-native.

    When starting a new project, you need to determine which type of router to use. 
    For browser based projects, there are BrowserRouter and HashRouter components.
    The BrowserRouter should be used when you have a server that will handle dynamic requests (knows how to respond to any possible URI)
    the HashRouter should be used for static websites (where the server can only respond to requests for files that it knows about).


    path-to-regexp package to determine if a route element’s path prop matches the current location. It compiles the path string into a regular expression, which will be matched against the location’s pathname.

Creating our routes

    Routes can be created anywhere inside of the router, but often it makes sense to render them in the same place. You can use the `<Switch>` component to group Routes. The Switch will iterate over its children elements (the routes) and only render the first one that matches the current pathname.


**I hope to understand everything in our lecture tomorrow**