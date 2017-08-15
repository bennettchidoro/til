# Let's Write A Recursive Function

Recursion allows us to write our functions in a different manner. Whenever you hear the word recursive or recursion, it simply means the function is calling itself.

Here's an example of a recursive function:

```javascript
function factorial (number) {
  if (number <= 1) {
    return 1
  } else {
    return number * factorial(number - 1)
  }
}

factorial(5)
> 120
```
Walking through our function from top to bottom, we have our `if` statement to see if a number is less than or equal to 1. If it is, we return 1. Having this check is important so we don't throw an error when it comes to our recursive function being called. Going down to our `else` block, we make our recursive call to our `factorial()` function. The factorial of a number can be written as `n * !(n-1)`.

Each time we make it to our `else` block, our function is called again, and we start the process from top to bottom, until our `number <= 1` condition is satisfied.


Here's what's happening when we call `factorial(5)`:

```javascript
/*

 5 * factorial(5 - 1) is equal to  5 * factorial(4)
 5 * (4 * factorial(4 - 1) is equal to 5 * (4 * factorial(3))
 5 * (4 * (3 * factorial(3 - 1))) is equal to 5 * (4 * (3 * factorial(2)))
 5 * (4 * (3 * (2 * factorial(2 - 1)))) is equal to 5 * (4 * (3 * (2 * factorial(1))))

*/
```
