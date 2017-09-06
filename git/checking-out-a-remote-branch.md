# Checking Out A Remote Branch

`git` gives us some useful commands when working with remote branches.

You might have a remote branch that you want to get on your local machine in order to see what new features your coworker has implemented. To do this, you can run:

```bash
$ git fetch origin
```

Then:
```bash
$ git checkout -b branch_name origin/branch_name
```

In our case, `git fetch` is getting our data from our remote repository, but it's not integrating any of the data being fetched.

After we fetch our data, we then checkout the specified branch name that our coworker has implemented the new features on. `origin/branch_name` is a remote-tracking branch.
