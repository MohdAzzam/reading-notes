# Hooks API

A Hook is a special function that lets you `hook into` React features. For example, useState is a Hook that lets you add React state to function components. We’ll learn other Hooks later.


Functions can’t have local React state inside them. You can’t extract behavior like `watch window size and update the state` or “animate a value over time” from a class component without restructuring your code or introducing an abstraction like Observables. Both approaches hurt the simplicity that we like about React.


Hooks solve exactly that problem. Hooks let you use React features (like state) from a function — by doing a single function call. React provides a few built-in Hooks exposing the “building blocks” of React: state, lifecycle, and context.

 Since Hooks are regular JavaScript functions, you can combine built-in Hooks provided by React into your own `custom Hooks`. This lets you turn complex problems into one-liners and share them across your application .
