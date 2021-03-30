# Functional programming

 Is a programming paradigm a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data .

* pure functions is :
  It returns the same result if given the same arguments (it is also referred as deterministic).

* It does not cause any observable side effects.
* If our function reads external files, it’s not a pure function
* Pure functions are stable, consistent, and predictable.
* Pure functions benefits is that the code’s definitely easier to test.

>any fuction `Reading Files` or `Random number generation` can not be pure 

`Observation`: `mutability` is discouraged in functional programming.

-----------------------------------

### Functions as first-class entities can:

* refer to it from constants and variables.
* pass it as a parameter to other functions.
* return it as result from other functions.

-----------------------

### Higher-order functions:

>When we talk about higher-order functions, we mean a function that either:
* takes one or more functions as arguments.
*  Or returns a function as its result

#### Map :

The idea of map is to transform a collection.

The map method transforms a collection by applying a function to all of its elements and building a new collection from the returned values.

#### Filter:

Given a collection, we want to filter by an attribute.
The filter function expects a true or false value to determine if the element should or should not be included in the result collection.

--------------------------------------

## Refactoring JavaScript for Performance and Readability 

 way to make the code readabil
 lead to easier to read code. There are no absolutes when it comes to clean code — there's always an edge case!