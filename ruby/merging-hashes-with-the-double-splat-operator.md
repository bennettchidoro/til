# Merging Hashes With The Double Splat Operator

Typically, we use the `merge` method to merge our hashes:

```ruby
> h1 = {:one => 1, :two => 2}
=> {:one=>1, :two=>2}
> h2 = {:three => 3, :four => 4}
=> {:three=>3, :four=>4}
> h1.merge(h2)
=> {:one=>1, :two=>2, :three=>3, :four=>4}
```
Using the double splat operator to merge our hashes:


```ruby
> h1 = {:one => 1, :two => 2}
=> {:one=>1, :two=>2}
> h2 = {:three => 3, :four => 4}
=> {:three=>3, :four=>4}
> {**h1, **h2}
=> {:one=>1, :two=>2, :three=>3, :four=>4}
```
