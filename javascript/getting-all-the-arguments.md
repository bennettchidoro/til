# Getting All The Arguments

Whenever we call a function, a special variable named `arguments` is added to the environment. This variable gives us all the arguments that are passed to our function.

```javascript
function twoArguments(a, b) {
  console.log("I'm a function with " + arguments.length + ' arguments!' )
}

twoArguments('Hello', 'World')

// → I'm a function with 2 arguments!
```

Above, we use the `.length` property that gives us the number of arguments passed to our function. It's important to note that the `arguments` variable is a lot like an array, but does not have any of the array methods available to it.
