# Read 09

## Functional Programming

Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data.

### Pure function

A pure function is a function where the return value is only determined by its input values, without observable side effects.

Example on an impure function:

```js
let PI = 3.14;

const calculateArea = (radius) => radius * radius * PI;

calculateArea(10); // returns 314.0
```

It can be changed to pure by as follows:

```js
let PI = 3.14;

const calculateArea = (radius, pi) => radius * radius * pi;

calculateArea(10, PI); // returns 314.0
```

The benefit of using a pure function is that the code’s definitely easier to test. We don’t need to mock anything. So we can unit test pure functions with different contexts.

### Immutability

Immutability is unchanging over time or unable to be changed. When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.

### Referential transparency

pure functions + immutable data = referential transparency

Basically, if a function consistently yields the same result for the same input, it is referentially transparent.

### Functions as first-class entities

Functions as first-class entities can:

* refer to it from constants and variables.
* pass it as a parameter to other functions.
* return it as result from other functions.

The idea is to treat functions as values and pass functions like data. This way we can combine different functions to create new functions with new behavior.

### Higher-order functionswe

Higher-order function that either takes one or more functions as arguments, or returns a function as its result.

filter(), map(), and reduce() are examples on a higher-order function.

[Back to Home](README.md)
