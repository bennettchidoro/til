# Specifying When A Validation Should Happen

I came across the `:on` option while doing some reading on validations and I
decided it was worthy of sharing.

The `:on` option lets us decide when a validation should happen.

```ruby
class Movie < ApplicationRecord
  # it will be possible to update a movie without including a name
  validates :name, presence: true, on: create
end
```

With this validation in place, our application will only check if we include a name attribute when our movie is created.
