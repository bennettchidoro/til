# Accessors

Ruby gives us the ability to create getters and setters with metapprogramming. Metaprogramming is a shorthand way to write a program with another program. `attr`, `attr_reader`, `attr_writer`, and `attr_accessor` all come from the `Module` class.

Using `attr` creates one getter method.

Using `attr_reader` creates one or more instance variables that "get" the values of each method.

Using `attr_writer` creates one or more instance variables that "set" the values of each method.

Using the `attr_accessor` method wraps `attr_writer` and `attr_reader` all into one.

```ruby
class DK
  attr_accessor :run, :jump, :smash
end

DK.instance_methods.sort - Object.instance_methods
=> [:jump, :jump=, :run, :run=, :smash, :smash=]
```
