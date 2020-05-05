# helper_method

Bear with me as I jot down some notes. This might or might not go somewhere.

Helper methods (any methods defined in a file in your `helpers` directory) cannot be called from inside our controllers.

```ruby
# users_helper.rb

module SessionsHelper

  def current_user
    @current_user ||= User.find(session[:user_id]) if session[:user_id]
  end
end
```

If we tried calling this `current_user` helper method in any of our controllers we would get an error. On the other hand, the `current_user` method is available in all of our views.

All controllers inherit from the `ApplicationController (app/controllers/application_controller.rb)`, so if we want to be able to access a method in all of our controllers, it makes sense to define it here.

If we moved the `current_user` helper method from above, into our `ApplicationController`, it becomes accessible to all of our controllers, but not our views.

```ruby
# application_controller.rb

class ApplicationController < ActionController::Base

  def current_user
    @current_user ||= User.find(session[:user_id]) if session[:user_id]
  end

end
```

To make the `current_user` method available to all of our views, we have to define the `helper_method` and explicitly tell it which methods we want to include.

```ruby
# application_controller.rb

class ApplicationController < ActionController::Base

  def current_user
    @current_user ||= User.find(session[:user_id]) if session[:user_id]
  end

  helper_method :current_user
end
```
