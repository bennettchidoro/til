# Avoiding Merge Commits From Git Pull

I kept running into the same issue where every time I would do a `git pull`, I would end up with a dreadful merge commit.
To avoid getting a merge commit when using `git pull` use:

```git
git pull --rebase
```

We can also set it as the default with:

```git
git config --global pull.rebase true
```

`git pull --rebase` is useful when you're working on a feature branch and you want to merge in the changes that your coworkers have made on the `master` branch. `git pull --rebase` will merge in the changes that your coworkers made onto your current feature branch. Then, once you merge your brach into `master`, you won't end up with a merge commit. 
