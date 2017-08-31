# Using Map Instead of A For Loop

Instead of using our typical `for` loops to iterate over an array, we can can use the `map` method. `map` creates a new array and does something to every element in the array that we're calling it on.

```javascript
var ourArray = [1, 2, 3];

var addTwoToEachNumber = ourArray.map(function(x) {
  return x + 2;
});

console.log(addTwoToEachNumber);
// [ 3, 4, 5 ]

console.log(ourArray);
// The contents of ourArray stays the same
// [1, 2, 3]
```
