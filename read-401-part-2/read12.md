# Redux - Combined Reducers 

Why choose Redux instead of the Context API for global state? 

You have larger amounts of application state that are needed in many places in the app
The app state is updated frequently over time
The logic to update that state may be complex
The app has a medium or large-sized codebase, and might be worked on by many people


What is the purpose of a reducer?
A reducer is a function that determines changes to an application’s state. It uses the action it receives to determine this change. We have tools, like Redux, that help manage an application’s state changes in a single store so that they behave consistently.

What does an action contain?

An action is a plain JavaScript object that has a type field. You can think of an action as an event that describes something that happened in the application.


Why do we need to copy the state in a reducer?

f the changes outside the store are intended to modify the state, dispatch should be used instead. In addition to update of the state, dispatch also notifies every subscriber of the store about the changes.
The only way to change the state is to emit an action, an object describing what happened.