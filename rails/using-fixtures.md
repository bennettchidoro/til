# Using Fixtures

Fixtures allow us to provide sample data to our applications database before running our tests. They are written in [YAML](http://www.yaml.org/start.html) and only one file per model is included.

We can locate fixtures in the `test/fixtures` directory

```YAML
# users.yml
rob:
  name: Rob Zombie
  email: robz@zombie.com
  password_digest: <%= User.digest('password') %>
```

Each fixture is given and name and is followed by an indented list of key/value pairs separated by a colon.

Above, we define a user named *rob* with `name`, `email` and `password_digest` keys as well as their corresponding values.

Once we've defined our fixtures, we can now write tests already having predefined data in our testing database.
