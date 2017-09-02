# Getting Comfortable With The Filesystem

Understanding Linux files and their layout can help you on your quest to mastering the shell.

Every Linux file is made up of a directory. Just think of a directory as a folder or container of some sort. There can be many directories within one directory. These are called `subdirectories`.

The topmost directory is called the `root` directory. It is represented with a slash `/`.

 A `path` is a where a directory or file is located on a filesystem. Think of a `path` as an address to that file or directory. "Names and slashes" are used to represent paths.

```bash
$ /a/b/c
```
In the path above, `/`, refers to the `root` directory, which contains a directory called `a`, which contains a directory called `b`, which contains a directory called `c`. An `absolute` path always starts with the root directory.
