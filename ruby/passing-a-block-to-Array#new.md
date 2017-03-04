# Passing A Block To Array#new

Creating a grid of any size is as easy as passing a block to `Array#new`.


Calling `Array#new` with an argument gives us an array of the specified length:

```ruby
Array.new(4)
# => [nil, nil, nil, nil]
```

When we pass `Array#new` a block, all of our fields get populated with the result of the block:

```ruby
Array.new(4) { Array.new(4) {'x'} }
# => [["x", "x", "x", "x"], ["x", "x", "x", "x"], ["x", "x", "x", "x"], ["x", "x", "x", "x"]]
```

Above, we pass our array four elements and a block that generates an array with another four elements that are all 'x'. We created a 4x4 grid populated with 'x' strings.
