# Installing RVM

[RVM](http://rvm.io/), the ruby version manager, like the name says, is a flexible tool that lets us manage different versions of ruby among many other things.

```bash
$  curl -L https://get.rvm.io | bash -s stable
```

The above command installs all of the necessary dependencies in order for `rvm` to run. In order to verify `rvm` was properly installed, close your terminal and type:

```bash
rvm --version
```

You should see a version number with no errors.

*This assumes you have already install Apple's Command Line Tools for Xcode.*
