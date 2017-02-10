# Strong Parameters

Rails gives us strong parameters to protect against mass assignment vulnerabilities. Strong parameters allow us to state which parameters are required and which ones are permitted.

```ruby
# Users controller
def create
  @user = User.new(params[:user])
end
```

The above would throw an `ActiveModel::ForbiddenAttributes` exception.

```ruby
# Users controller
def create
  @user = User.new(user_params)
end

private

def user_params
  params.require(:user).permit(:name, :email)
end
```

This returns our params hash with only the permitted attributes allowed. 
