# Designing A Class

When designing a class in Java, it helps to think about what your object *knows* (instance variables), and what your object can *do* (methods).


Say we're designing a `Television` class. A television object might know its `channel`, its `volume`, and whether its `power` is on or not. Some of the things our television object might be able to do is `setChannel()`, `setPower()`, and `setVolume()`.

Thinking about these beforehand should give you an overall better view as to how your object behaves when implemented correctly.


```Java
class Television {
  int channel;
  int volume;
  boolean power;

  setChannel() {
    // do stuff
  }
  setPower() {
    // do stuff
  }
  setVolume() {
    // do stuff
  }
}
```
