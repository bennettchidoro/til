# Local Scope In Functions

`scope` refers to the current context of where we're currently at in our program. Understanding `scope` is key to becoming a better developer and writing better code.

When we define a variable within our function, that variable has local scope. This means that our variable is only visible within our function.


```javascript
function myFunction() {
  var name = "foo";
  console.log(foo);

  myFunction(); // "foo"
  console.log(name); // "undefined"
}
```
Trying to call `name` will throw an error because it is not defined outside of our function.
