# Printing The Generated SQL

Sometimes you may want to see the SQL that a query method generates. Rails provides us with the `to_sql` method to do so. After writing your query, just tack on `to_sql` and the raw SQL will be printed.

```ruby
>> Movie.where("total_gross >= 300000000").order("total_gross desc").to_sql
```

```bash
=> "SELECT "movies".* FROM "movies" WHERE (total_gross >= 300000000) ORDER BY total_gross desc"
```
