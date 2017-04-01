# Download An Entire Website Using Wget

GNU's `wget` command let's us retrieve files using HTTP, HTTPS and FTP. The mirror feature in `wget` gives us the ability to create entire local copies of a website.

```bash
$ wget -mk -w 20 http://www.example.com/
```
The `-m` flag turns on mirroring options.

The `-k` flag makes it so the original links on every page no longer point to the real URLs. They now point to your local download.

The `-w` flag is the wait option. In our command above, we tell it to wait 20 seconds in between retrievals.
