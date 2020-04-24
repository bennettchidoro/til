# Custom URLs

Rails supports custom URLs and they're pretty simple to implement.
Say we wanted to add a route to support our custom URL
http://localhost:3000/signup.

In our `routes.rb`, we already have `resources :users` that provides us with a handful of routes. In order to add a custom route to `/signup`, we have to make a get request to that specific URL(`/signup`) that maps to the new action in our users controller.

```ruby
# config/routes.rb

Rails.application.routes.draw do
  # verb "url" => "name_of_controller#name_of_action"
  root 'movies#index'
  get "/signup" => "users#new"

  resources :users
end
```
Now when we navigate to `/signup` it will map to the new action in our `Users` controller and will allow us to create a new user.
