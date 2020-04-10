# Resource Generator

Sometimes you may need to create migrations, a model, routes and a controller. Rails calls all of these a resource. Resources are so common that Rails provides us with a resource generator.

The resource generator takes the same options as the model generator followed by a list of fields and types separated by colons.

```
$ rails g resource review name:string stars:integer comment:text movie:references

Running via Spring preloader in process 7000
      invoke  active_record
      create    db/migrate/20200410022923_create_reviews.rb
      create    app/models/review.rb
      invoke    test_unit
      create      test/models/review_test.rb
      create      test/fixtures/reviews.yml
      invoke  controller
      create    app/controllers/reviews_controller.rb
      invoke    erb
      create      app/views/reviews
      invoke    test_unit
      create      test/controllers/reviews_controller_test.rb
      invoke    helper
      create      app/helpers/reviews_helper.rb
      invoke      test_unit
      invoke    assets
      invoke      scss
      create        app/assets/stylesheets/reviews.scss
      invoke  resource_route
       route    resources :reviews
```

Running the above command creates all of these files.
