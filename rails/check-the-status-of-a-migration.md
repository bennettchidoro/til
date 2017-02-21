# Check The Status Of A Migration

Rails provides us with the very helpful `rails db:migrate:status` command to see if we have any pending migrations. Here's some sample output from The [Ruby on Rails Tutorial](https://www.railstutorial.org/book) sample application.


```
Status   Migration ID    Migration Name
--------------------------------------------------
   up     20170203191007  Create users
   up     20170204070327  Add index to users email
   up     20170206174652  Add password digest to user
   up     20170216190206  Add remember digest to users
   up     20170220032050  Add admin to users
   up     20170220165715  Add activation to users
```
