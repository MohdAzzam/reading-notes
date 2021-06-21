# Context API

Context provides a way to pass data through the component tree without having to pass props down manually at every level.

Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language.


Describe use cases for useMemo() and useReducer()
    1. Avoids a re-render if its props haven’t changed.
        - Imagine we have to process some data that we receive from an API that does not change between renders
    2. if the app using a complex object

Why do custom hooks need the `use` prefix?
    we could distinguish between helper functions and custom hooks. 

What do custom hooks usually do?
To share logic between components 

Using any list of custom hooks, research and name one that you think will be useful in your applications

useForm
useClippy
useLocalStorage

Describe how a hook that fetches API data might work?
hold the data using useState() then  by using useEffect
