# The PATH Variable

### In this level, you will disrupt the operation of the /challenge/run program. This program will DELETE the flag file using the rm command. However, if it can't find the rm command, the flag will not be deleted, and the challenge will give it to you! Thus, you must make it so that /challenge/run also can't find the rm command!

**Flag:** `pwn.college{Mcom26ORjWyBAbpCYxKjZ_nXJjT.QX2cDM1wSO4gjNzEzW}`

```
#!/bin/bash

hacker@path~the-path-variable:~$ PATH=""
hacker@path~the-path-variable:~$ /challenge/run
Trying to remove /flag...
/challenge/run: line 4: rm: No such file or directory
The flag is still there! I might as well give it to you!
pwn.college{Mcom26ORjWyBAbpCYxKjZ_nXJjT.QX2cDM1wSO4gjNzEzW}
```

## What I learned

I learnt to blank out the PATH variable and not have rm command work properly

## References

NA
