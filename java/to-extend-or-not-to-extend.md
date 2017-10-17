# To Extend, Or Not to Extend

When you're asking yourself if one class should `extend` another, a simple way to test if it should is to use the "IS-A" test.

Let's say we have an `Animal` class as our superclass. We'll test a few subclasses to see if they should extend or not:

Elephant IS-A Animal :heavy_check_mark:

Cheetah IS-A Animal :heavy_check_mark:

Speed IS-A Animal ❌

The first two pass our "IS-A" test. The last one doesn't, but we can use the "HAS-A" test. In this case, Animal has a speed instance variable.

Remember, the "IS-A" test works anywhere in the inheritance tree.
