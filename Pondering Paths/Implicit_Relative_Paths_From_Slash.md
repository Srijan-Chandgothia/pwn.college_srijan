# Implicit Relative Paths, From /

### Let's try it here! You'll need to run /challenge/run using a relative path while having a current working directory of /. For this level, I'll give you a hint. Your relative path starts with the letter c 😊

**Flag:** `pwn.college{wAdg5PyddpyaYtWKe18msTGp4dn.QX5QTN0wSO4gjNzEzW}`

```
#!/bin/bash

hacker@paths~implicit-relative-paths-from-:~$ /challenge/run
Incorrect...
You are not currently in the / directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~implicit-relative-paths-from-:~$ cd /
hacker@paths~implicit-relative-paths-from-:/$ /challenge/run
Incorrect...
You invoked this challenge with an absolute path. This challenge needs a relative path!
hacker@paths~implicit-relative-paths-from-:/$ challenge/run
Correct!!!
challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{wAdg5PyddpyaYtWKe18msTGp4dn.QX5QTN0wSO4gjNzEzW}
```

## What I learned

I learnt to invoke programs using relative paths

## References

NA
