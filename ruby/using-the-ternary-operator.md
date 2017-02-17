# Using The Ternary Operator

The ternary operator(`?`) allows us to shorten our `if/else` statements into a single line. Appropriately named *ternary* because it consists of three parts.


Conventional `if/else` statement: 
```ruby
if boolean?
  do_one_thing
else
  do_something_else
end
```

Converting the above `if/else` statement using the ternary operator `(?)`

```ruby
boolean? ? do_one_thing : do_something_else
```


If you ever get confused about ternary statements, it's best to think of it like this:

`if_this_is_a_true_value ? then_the_result_is_this : else_it_is_this`
