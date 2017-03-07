# Making Your Program Sleep

Ruby's `Kernel` module provides us with the `#sleep` method.
It takes in a duration, which can be any positive integer and it suspends the current thread for the duration you pass in.

According to Wikipedia:

> In computer science, a thread of execution is the smallest sequence of programmed instructions that can be managed independently by an operating system scheduler. A thread is a light-weight process.

`#sleep` in action:
```ruby
3.downto(1) { |x| puts x, ""; sleep 1 }

3

2

1

#=> 3
```

You can't see it, so just imagine it. The code sample above counts down from `3`, but before the next integer is printed out, the program suspends for 1 second.
