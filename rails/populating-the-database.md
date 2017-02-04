# Populating The Database

Rails gives us the ability to populate the database without having to do it manually through the rails console. We can populate the database through the `db/seeds.rb` file.
In this file, we have access to all of our applications methods and classes.


db/seeds/rb:
```ruby
Person.create(name: 'Steve Jobs')
Person.create(name: 'Mark Cuban')
Person.create(name: 'Michael Jordan')
```

After we are done entering our data we need to seed it in our database.
```bash
rake db:seed
```
