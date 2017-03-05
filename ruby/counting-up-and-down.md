# Counting Up And Down

Ruby's `Integer` class gives us the ability to count up and down with the `#upto` and `#downto` methods. The integer that we start with is always the return value.

Counting to 5:

```ruby
> 1.upto(5) { |i| puts i }
1
2
3
4
5
#=> 1
```
Counting down from 5:

```ruby
> 5.downto(1) { |i| puts i }
5
4
3
2
1
#=> 5
```
