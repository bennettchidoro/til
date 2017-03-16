# Get A List Of A Method's Parameters


Use `Method#parameters` to return a list of a method's parameters. This method returns the type of each parameter.

```ruby
def name(name, options = {})
end

method(:name).parameters
#=> [[:req, :name], [:opt, :options]]
```
