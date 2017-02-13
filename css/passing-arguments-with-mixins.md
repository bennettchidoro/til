# Passing Arguments With Mixins

Not only do mixins provide us with the ability to reuse our `css` declarations
throughout our code, we can also pass arguments to them.

```scss
@mixin button ($radius, $color) {
  border-radius: $radius;
  color: $color;
}
```

In the example above, we have two arguments: $radius and $color. We denote arguments by putting the `$` followed by the name of the property.

Using our mixin:

```scss
.btn-a {
  @include button(4px, red)
}
```
Passing the incorrect number of arguments will throw us an error message.
