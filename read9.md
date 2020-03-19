# REFACTORING
- Refactoring code is making it more readable and makes it run more efficiently.
- Pure functions: return the same results if given the same argument, and do not cause observable side-effects.i.e
``` js 
let PI = 3.14;const calculateArea = (radius, pi) => radius * radius * pi;calculateArea(10, PI); 
// returns 314.0
```
- if the PI was not put in as an argument then the function would be impure. Same as if the function reads files since the content always changes. Functions that rely on random generators as well.
- If a function consistently returns the same results for the same input then it is referentially transparent.
- Functions as first-class entities can:- refer to it from constants and variables, pass it as a parameter to other functions, and return it as result from other functions
- High-order functions:- takes one or more functions as arguments or returns a function as its result.