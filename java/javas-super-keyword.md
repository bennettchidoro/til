# Java's Super Keyword

When designing with inheritance, there's a chance you could run into a situation where you would want to use both the `superclass` version and the overriding `subclass` version of a method. In this case, we can use Java's `super` keyword.

```Java
class Mother {
  public void sayHi() {
    System.out.println("I am the Mother class!");
  }
}

class Child extends Mother {
  public void sayHi() {
    super.sayHi();
    System.out.println("I am the Child class!");
  }

  public static void main(String[] args) {
    Child c = new Child();
    c.sayHi();
  }
}
```

Going through the example from above, `Mother` is our superclass and `Child` is our subclass. Both have the same `sayHi()` method. We want to be able to use both methods, so we call our overriding `sayHi()` method in our `Child` class with the `super` keyword.

The output after running this program would be:
```Java
// I am the Mother class!
// I am the Child class!
```

Using the `super` keyword tells our program to first go run the superclass version, then come back and finish with the subclass version.
