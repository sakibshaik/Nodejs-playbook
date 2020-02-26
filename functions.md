We prefer using Arrow functions (also called "fat arrow functions").Having said that, There are big differences between arrow functions and classic function expressions. 
They’re more powerful in some situations, but terrible in others.Several traits which encapsulates Arrow functions that can make calling them more convenient, and leave out other behavior that isn’t as useful when calling a function.

As Arrow functions don't have their own this or arguments binding. Instead, those identifiers are resolved in the lexical scope like any other variable.

Also there is a  distinction between functions that are callable and functions that are constructable. A function which is constructable, can be called with new, i.e. new User(). A function which is callable, can be called without new (i.e. normal function call).

Functions created through function declarations or expressions are both constructable and callable.On the other hand,Arrow functions (and methods) are only callable. Also class constructors are only constructable.
When you try calling a non-callable function or trying to construct a non-constructable function, you end up with an runtime error.

Since Javascript functions are Variadic functions, arrow functions don't have their own arguments like function declarations / expressions.The [rest parameter](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/rest_parameters) syntax allows us to represent an indefinite number of arguments as an array. 

Arrow functions are more convenient for callbacks, promises, or for methods like map, reduce, and forEach.

