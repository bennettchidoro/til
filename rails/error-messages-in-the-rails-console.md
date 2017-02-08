# Error Messages In The Rails Console

Sometimes we want to see the effects of adding a validation in our model. Consider the following scenario where there is a minimum length on our password attribute:

```ruby
# User model
validates :password, presence: true, length: { minimum: 6 }            
```

After jumping into the rails console and creating a new user with a password that violates our validation. We can check our error messages like so:

```ruby
new_user.errors.full_messages
=> ["Password is too short (minimum is 6 characters)"]
```
