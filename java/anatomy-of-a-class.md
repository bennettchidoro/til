# Anatomy Of A Class

Every Java application must have at least one `class`.

```java
public class MyFirstApp {

}

```
The `public` keyword makes it so everyone can access it, and the `class` keyword defines our class.


In addition to a `class`, every Java application must have at least one `main` method per application.

```java
public static void main(String[] args) {

}
```

`static` indicates it is a class method and can be called without first instantiating an object of the class.

`void` means our method doesn't return a value.

`String[] args` are arguments to the method. This method takes an array of Strings and the array will be called `args`.


Everything together:

```java
public class MyFirstApp {
  public static void main(String[] args) {

  }
}

```
