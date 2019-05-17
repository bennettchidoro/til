# Difference Between Explicit And Implicit Receiver

Every time we call a method in Ruby, there must be an object that is receiving the method. The object that is receiving the method is called the `receiver`. If there's an object on the left-hand side, that's explicit. Anytime there's no object on the left-hand side, Ruby implicitly uses an object and that object is referenced by the variable `self`.

```ruby
class Greeting
  def hello
    "Hi!"
  end

  def greet_me
    self.hello # explicit receiver 'self'
    hello      # implicit because we don't mention the receiver, but Ruby implicitly uses the variable `self`
  end
end

obj = Greeting.new
obj.greet_me # 'obj' is the explicit receiver
```
