# Overriding Methods

A couple things to remember when working with overriding methods:

  1.  The arguments must be the same, and the return types must be compatible.
  2. The method can be *less* accessible, but not more.

```java
boolean sayHi(double d) {
  System.out.println("Hola");
  return true;
}

boolean sayHi(double a) {
  System.out.println("Holla");
  return false;
}
```
Alright, in the code above, pretend these two methods are both in a class and one `extends` the other. If we were to run our program it would compile.

```java
boolean sayBye(int x) {
  System.out.println("adiós");
  return true;
}

boolean sayBy(int f) {
  System.out.println("Tschüss");
  return 1;
}
```
This example would not compile, because the return types are different.
