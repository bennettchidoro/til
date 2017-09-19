# Casting An Object Into A Particular Type

Casting in Java forces the object immediately after it to become that type of cast. Here's an example to paint a clearer picture:

```Java
int randomNum = (int) (Math.random() * 11);
```

In the example above, `Math.random()` returns a `double` and we 'cast' it to be an `int` in order to get a nice whole number. The cast, in our case, (`int`), always comes before the object that you want to 'cast'.
