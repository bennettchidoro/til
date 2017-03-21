# Using The Switch Statement For Many Options

Rather than using your traditional `if/else` statements, you can use a `switch` statement if you have many options to choose from. `switch` statements tests an expression and can have many `case` statements which defines various possible values.

```javascript
switch(expr) {
  case "A":
    console.log("The first letter of the Alphabet is A");
    break;
  case "B":
    console.log("The second letter of the Alphabet is B");
    break;
  case "C":
    console.log("The third letter of the Alphabet is C");
    break;
}
```

In the `switch` statement above, if `expr` evaluates to "B", our program will match the value and the `console.log` statement for "B" will be executed.

If we forget to add the `break` statement, the next statement will be executed regardless if it matches or not.
