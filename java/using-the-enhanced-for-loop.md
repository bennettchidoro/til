# Using The Enhanced For Loop

Java provides us with plenty of ways to iterate over collections of data. Using the enhanced for loop, we can iterate over collections and arrays without knowing the index of the current element, and we can display our data in order from first to last.

Standard `for loop`:

```java
for (int i = 0; i < myArray.length; i++) {
  System.out.println(myArray[i]);
}
```
Enhanced `for loop`:

```java
for (int currentValue : myArray) {
  System.out.println(currentValue);
}
```
Starting from left to right we first tell our for loop to declare an `int` variable named `currentValue`. Each time through the loop, `currentValue` will hold a different element from `myArray` until there are no more elements.

Our example above can be read as: "for each int value `IN` myArray".
