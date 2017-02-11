# Mixins

Mixins provides us with the ability to reuse `css` declarations throughout our code, all while keeping it *dry*.

We define a mixin using the keyword `@mixin`:

```scss
@mixin button {
  border: 1px solid #ccc;
  font-size: 1em;
  text-transform: uppercase;
}
```

When we're ready to use our mixin, we use the `@include` keyword followed by the name of the mixin:

```scss
.btn-a {
  @include button;
  background: #777
}
```
