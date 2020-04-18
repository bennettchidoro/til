# Undo Your Most Recent Local Commits

Say you made a mistake and committed the wrong files or something of along those lines.

```
$ git commit -m "Something terribly wrong"
```

Git is pretty forgiving and lets us right our wrongs.
We can run `$ git reset HEAD~` and all of our recent commits will be unstaged. Then, we can make the necessary changes and add our files.
