# Running Pretend Generations

Say you're about to run the `rails generate` command, but you're not sure what all is going to be generated. To run a pretend generation, you can run the `rails generate` command with the `--pretend` flag.

```bash
$ rails generate controller Users --pretend
```

Output:
```
      create  app/controllers/users_controller.rb
      invoke  erb
      create    app/views/users
      invoke  test_unit
      create    test/controllers/users_controller_test.rb
      invoke  helper
      create    app/helpers/users_helper.rb
      invoke    test_unit
      invoke  assets
      invoke    coffee
```

Running the above command will show you everything that will be generated, but none of the files will actually created.
