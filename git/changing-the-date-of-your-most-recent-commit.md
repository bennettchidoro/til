# Changing The Date Of Your Most Recent Commit

For whatever reason, you might want to change the timestamp of your most recent commit. We can do this with the `git commit --amend` command. All we have to do is pass our command the `date` flag like such:

`git commit --amend --date="2017-02-28 10:08:07"`

Then, we can specify the actual date we want to our commit to have. The format for the date and time is `YYYY-MM-DD`
`hh-mm-ss`.
