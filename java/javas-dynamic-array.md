# Java's Dynamic Array

Up until now, I had no idea that arrays in Java weren't dynamic. As in once initialized, there is no modifying them. Luckily, Java includes an `ArrayList` class that lets us do just that.


```Java
import java.util.*;

ArrayList<String> myString = ArrayList<String>();
```

After adding the import statement we can define our `ArrayList`. The `<String>` in angle brackets means make a list of String objects.

Now we can do things like add to our ArrayList:

```Java
String a = new String();
myString.add("a");
```

See if it contains a certain value:

```Java
boolean isIn = myList.contains("a");

// true
```

Find out if it's empty:

```Java
boolean isEmpty = myList.isEmpty();

// false
```

Remove a value:

```Java
myList.remove(a)

// Our ArrayList is now empty :(
```
