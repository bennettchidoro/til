# Moving All Files From One Directory To Another

If we want to move all of the files from one directory to another, we can do it with the `mv`(move) command.

In my case, I wanted to move all of the files in my `/personal-repos` directory, into my newly created `/Code` directory.

```bash
$ mv -v ~/personal-repos/* ~/Code
```

The `-v` option means for "verbose" and it will show all the files, in my case, directories that were moved.

The wildcard `*` character just means to include everything.
