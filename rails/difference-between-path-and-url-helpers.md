# Difference Between Path and Url Helpers

After finishing chapter 10 of the [Ruby on Rails](https://www.railstutorial.org/book) Tutorial, I finally stopped and asked myself what the difference is between `_path` and `_url` helpers that Rails provides for us.

`_path` is the relative url to our domain.

So if we had something like `about_path`, it would be equivalent to `/about`.

`_url` provides us with an absolute path.

So something like `about_url`, would be equivalent to `www.localhost:3000/about`.

The Rails convention is to use `_url` when doing `redirects` because of the `HTTP` standard. For all other routing, we can just use the `_path` helper.
