# Resetting The Database

Ever feel the need to just blow away your database and get a fresh start? Rails provides us with the `rails:db:reset` command to do such that. Not only does it blow away the database, but it also re-create the development database, runs all the migrations, and runs the `db/seeds.rb` file.

```bash
$ rails:db:reset

Dropped database 'db/development.sqlite3'
Dropped database 'db/test.sqlite3'
Created database 'db/development.sqlite3'
Created database 'db/test.sqlite3'

```
