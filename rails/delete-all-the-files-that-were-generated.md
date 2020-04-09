# Delete All The Files That Were Generated

Sometimes we might end up making a mistake or misspelling something when we run a generator. Luckily, rails gives us the `destroy` command to delete all the files that were generated.

```
$ rails g resource revieew name:string stars:integer comment:text movie:references

invoke  active_record
      create    db/migrate/20200409035800_create_revieews.rb
      create    app/models/revieew.rb
      invoke    test_unit
      create      test/models/revieew_test.rb
      create      test/fixtures/revieews.yml
      invoke  controller
      create    app/controllers/revieews_controller.rb
...
```
Running `$ rails g destroy resource revieew name:string stars:integer comment:text movie:references` will delete all of the files that were generated.

```
invoke  active_record
      remove    db/migrate/20200409035148_create_reveiws.rb
      remove    app/models/reveiw.rb
      invoke    test_unit
      remove      test/models/reveiw_test.rb
      remove      test/fixtures/reveiws.yml
      invoke  controller
      remove    app/controllers/reveiws_controller.rb
```

Be sure to pass in the exact same options you used when running the generator.
