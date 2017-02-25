# Duck Typing

*Duck typing* is a programming concept that focuses on the methods that can be passed to an object rather than the class that the object comes from.


After reading about duck typing, the first thing that popped in my head was, "*I don't care where you come from, just as long as we can work together*." This helped me generalize the concept a little better.

Everything in Ruby is an object and all of these objects come from different classes. We're not really concerned with the type or class of an object, we're more concerned with what that object can do.

```ruby
def print_size(item)
  "The items size is #{item.zise}."
end

mystring = "This is a string"
print_size(mystirng)
=> "The items size is 16."

myarray = [1, 2, 3, 4, 5]
print_size(myarray)
=> "The items size is 5."
```

In the example above, we call `size` on the object without any regards to its class. If we pass our method an object that responds to `size`, it will give us the size back. Otherwise, it'll throw us an error.
