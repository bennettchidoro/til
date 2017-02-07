# Rails Console Sandbox Mode

Rails gives us the option to start the console in sandbox mode. When we enter the console in sandbox mode any database operations we make are automatically "rolled back" when we exit the console.

Start the rails console in sandbox mode with: `$ rails c --sandbox`

![](https://s3.amazonaws.com/til-stuff/tty.gif?)

Sandbox mode comes in handy when we want to experiment with the database without permanently changing our data.
