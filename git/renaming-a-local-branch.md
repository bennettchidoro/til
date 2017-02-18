# Renaming A Local Branch

In order to rename a local branch, we can pass the `-m` flag to the `git branch` command. If you are currently on the branch you want to rename, all you need to do is specify the new branch name.

```bash
$ git branch -m <new-branch-name>
```

Renaming a branch other than the one you are on:

```bash
$ git branch -m <old-branch-name> <new-branch-name>
```
