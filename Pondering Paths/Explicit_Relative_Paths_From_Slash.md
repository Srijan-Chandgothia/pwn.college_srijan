# Explicit Relative Paths, From /

### This challenge will get you using . in your relative paths. Get ready!

**Flag:** `pwn.college{Yr0qYYIDJpiZ9MHBJT-cMuBBmal.QXwUTN0wSO4gjNzEzW}`

```
#!/bin/bash

hacker@paths~explicit-relative-paths-from-:~$ /challenge/run
Incorrect...
You are not currently in the / directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~explicit-relative-paths-from-:~$ cd /
hacker@paths~explicit-relative-paths-from-:/$ /challenge/run
Incorrect...
You invoked this challenge with an absolute path. This challenge needs a relative path!
hacker@paths~explicit-relative-paths-from-:/$ ./challenge/run
Correct!!!
./challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{Yr0qYYIDJpiZ9MHBJT-cMuBBmal.QXwUTN0wSO4gjNzEzW}
```

## What I learned

I learnt about relative paths and ./

## References

NA
