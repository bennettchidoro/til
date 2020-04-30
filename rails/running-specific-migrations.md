# Running Specific Migrations

For whatever reason, at some point in time, you may want to run specific migrations. Rails has us covered.

First, to view a list of migrations, run `$ rails db:migrate:status`

```
Status   Migration ID    Migration Name
--------------------------------------------------
   up     20200311141509  Create movies
   up     20200318004711  Add fields to movies
   up     20200405185103  Add more fields to movies
   up     20200410022923  Create reviews
   up     20200423020042  Create users
   down   20200424060202  Add username to user
```

Now, in order to run a specific migration, all we have to do is run:
<br>
`$ rails db:migrate:up VERSION=20200424060202`

Be sure to specify up or down and to pass in the correct version number of the migration you want to run.
