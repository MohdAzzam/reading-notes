# Custom Hooks

It is a JS function his name starts with `use` and that may call other Hooks.

---------------------

A custom Hook doesn't need to have a specific signature.

 We can decide if  it takes as arguments.
 it's look like any Js function

---------------------

useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one.

 useReducer also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks.


