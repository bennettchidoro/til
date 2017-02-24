# Does This Method Respond To An Object

Ruby provides us with the `respond_to?` method that will respond `true` or `false` depending whether or not the object will respond to the method that is given.

```ruby
10.respond_to(:upcase) # => false
10.respond_to(:eql?) # => true
10.respond_to(:gsub) # => false
```
