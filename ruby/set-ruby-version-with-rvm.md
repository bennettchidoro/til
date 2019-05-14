# Set Ruby Version With RVM

Depending on the project, there may come a time when we need to work with a lower or higher version of Ruby. [RVM](http://rvm.io/) lets us switch between versions with ease.

First, type `rvm list` into your terminal to see what Ruby versions you have available.

```
=* ruby-2.5.1 [ x86_64 ]
   ruby-2.6.3 [ x86_64 ]

# => - current
# =* - current && default
#  * - default
```
Then, type `rvm use 2.6.3` to switch to version 2.6.3.

To make sure the switch was was successful, type `ruby -v` and make sure the output matches the version you switched to.
