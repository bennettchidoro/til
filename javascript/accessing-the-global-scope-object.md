# Accessing The Global Scope Object

Whenever we create a global variable in JavaScript, it is stored in the global scope. In browsers, the global scope object is stored in the window variable. We can access our global variables as a property of this object.


```JavaScript
var myAge = 28;

console.log("myAge" in window)
// true
console.log(window.myAge);
// 28
```
