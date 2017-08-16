# Breaking Down A Command

Typing and running Linux commands in your shell can seem like a very daunting task, especially if you're new to it. Understanding what a command consists of, is a good place to start learning how to master the shell. A Linux command is usually made up of a *program name*, followed by *options* and *arguments*. For example, this command to halt (shutdown) the system in ten minutes and display a message to all users that are logged in:

```bash
$ shutdown -h +10 "server maintenance"
```
In this command, `shutdown` is the program, `-h` is the option saying to halt the system, and `+10` and `"server maintenance"` are the arguments. The time argument can be a number in minutes with a `+` sign in front of it, or, an absolute time in hours and minutes, like 21:15.

Commands can be way more complex than this, but this is just the basis.
