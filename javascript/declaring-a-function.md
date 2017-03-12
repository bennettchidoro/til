# Declaring A Function

In JavaScript, we can use `functions` to divide our code up and make it more reusable. We write `functions` in order to address a particular set of problems or complete a particular set of tasks.

We declare a function using the `function` keyword, followed by the name of the function written in [camel case](https://en.wikipedia.org/wiki/Camel_case) letters and a set of parenthesis`()`:

```javascript
function sayHello() {

}
```

Whatever code we want to be executed can be placed between the curly brackets`{}`:

```javascript
function sayHello() {
  console.log("Hello!");
}
```
In order to call or invoke our function, we just use the function name followed by a set of parenthesis`()`:

```bash
> sayHello();
Hello!
```
