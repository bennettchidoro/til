# Using Function.prototype.apply()

JavaScript's [`Function.prototype.apply()
`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/apply) can be used to call a function with arguments as an array.

```JavaScript
function introduceYourself(name, from) {
  console.log("Hi! My name is " + firstName + " and I'm from " + from);

introduceYourself("Jim", "Wisconsin");
// Hi! My name is Jim and I'm from Wisconsin

introduceYourself.apply(undefined, ["Kat", "San Diego"]);
// Hi! My name is Kat and I'm from San Diego

}
```

<!-- Scenarios when apply() can be useful coming soon... -->
