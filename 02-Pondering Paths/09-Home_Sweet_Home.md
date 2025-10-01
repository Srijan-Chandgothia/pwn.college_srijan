# Home Sweet home

### In this challenge, /challenge/run will write a copy of the flag to any file you specify as an argument on the commandline, with these constraints:

Your argument must be an absolute path.
The path must be inside your home directory.
Before expansion, your argument must be three characters or less.
Again, you must specify your path as an argument to /challenge/run as so:
```
hacker@dojo:~$ /challenge/run YOUR_PATH_HERE
```

**Flag:** `pwn.college{8rSibsFf3Nh-hmO7Uu6O2yJ5Q5B.QXzMDO0wSO4gjNzEzW}`

```
#!/bin/bash

hacker@paths~home-sweet-home:~$ /challenge/run
You must provide an argument to /challenge/run when you invoke it!
hacker@paths~home-sweet-home:~$ /challenge/run /home/hacker/flag
The argument you provided must not have been longer than 3 characters (it's
currently 17 characters long)!
hacker@paths~home-sweet-home:~$ /challenge/run ~/flag
The argument you provided must not have been longer than 3 characters (it's
currently 6 characters long)!
hacker@paths~home-sweet-home:~$ /challenge/run ~/f
Writing the file to /home/hacker/f!
... and reading it back to you:
pwn.college{8rSibsFf3Nh-hmO7Uu6O2yJ5Q5B.QXzMDO0wSO4gjNzEzW}
```

## What I learned

I learnt about ~ meaning the home destination

## References

NA
