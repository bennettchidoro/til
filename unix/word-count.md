# Word Count

The `wc` (word count) program gives us a print out of the number of lines, words, and bytes in our file.

```bash
$ wc myfile
    10     22     328 myfile
```

`myfile` has 10 lines, 22 whitespace-delimited words, and 328 bytes.

If we only wanted a word count, we could add the ` -w` option:

```bash
$ wc -w myfile
    22 myfile
```
