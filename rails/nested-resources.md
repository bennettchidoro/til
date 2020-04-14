# Nested Resources

Say we have this relationship in our application defined in our models. `Movie` is the parent and `Review` is the child.

```ruby
class Movie < ApplicationRecord
  has_many :reviews
end

class Review < ApplicationRecord
  belongs_to :movie
end
```

Nested resources let us mimic this relationship in our `routes.rb` file.

```ruby
resources :movies do
  resources :reviews
end
```
By nesting reviews under movies, we get access to these routes.


```
| Prefix            | Verb    | URI Pattern                                     | Controller#Action   |
|---                |---      |---                                              |---                  |
| root              |  GET    |     /                                           |  movies#index       |
| movie_reviews     |  GET    |    /movies/:movie_id/reviews(.:format)          |  reviews#index      |
|                   |  POST   |    /movies/:movie_id/reviews(.:format)          |  reviews#create     |
| new_movie_review  |  GET    |    /movies/:movie_id/reviews/new(.:format)      |  reviews#new        |
| edit_movie_review |  GET    |    /movies/:movie_id/reviews/:id/edit(.:format) |  reviews#edit       |
| movie_review      |  GET    |    /movies/:movie_id/reviews/:id(.:format)      |  reviews#show       |
|                   |  PATCH  |    /movies/:movie_id/reviews/:id(.:format)      |  reviews#update     |
|                   |  PUT    |    /movies/:movie_id/reviews/:id(.:format)      |  reviews#update     |
|                   |  DELETE |    /movies/:movie_id/reviews/:id(.:format)      |  reviews#destroy    |
```
