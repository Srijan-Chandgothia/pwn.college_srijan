# Position Thy Self

### This challenge will require you to execute the /challenge/run program from a specific path (which it will tell you). You'll need to cd to that directory before rerunning the challenge program. Good luck!

**Flag:** `pwn.college{E66zA99DHcb_wwVFLHO-RKWHlap.QX2QTN0wSO4gjNzEzW}`

```
#!/bin/bash

hacker@paths~position-thy-self:~$ /challenge/run
Incorrect...
You are not currently in the /proc/142/fd directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-thy-self:~$ cd /proc/142/fd
hacker@paths~position-thy-self:/proc/142/fd$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{E66zA99DHcb_wwVFLHO-RKWHlap.QX2QTN0wSO4gjNzEzW}
```

## What I learned

I learnt to navigate to different directories using commands

## References

NA
