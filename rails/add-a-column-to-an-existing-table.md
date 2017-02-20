# Add A Column To An Existing Table

Rails allows us to run migrations from within with the `rails generate migration` command. Say we want to add an `admin` attribute to our existing `users` table. We would type:

```bash
$ rails generate migration add_admin_to_users admin:boolean
```
The above command would generate a `timestamp_add_admin_to_users.rb` file.

```ruby
# db/migrate/[timestamp]_add_admin_to_users.rb

class AddAdminToUsers < ActiveRecord::Migration[5.0]
  def change
    add_column :users, :admin, :boolean
  end
end
```
To run our migration, we would simply type: `rails db:migrate`
