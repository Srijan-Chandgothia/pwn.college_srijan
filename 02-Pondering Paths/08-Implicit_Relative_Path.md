# Implicit Relative Path

### In this challenge, we'll learn how to explicitly use relative paths to launch run in this scenario. The way to do this is to tell Linux that you explicitly want to execute a program in the current directory, using . like in the previous levels. Give it a try now!

**Flag:** `pwn.college{8Z4JNZhBN1M--dU9R1kyuiv6WiV.QXxUTN0wSO4gjNzEzW}`

```
#!/bin/bash

hacker@paths~implicit-relative-path:~$ /challenge/run
Incorrect...
You are not currently in the /challenge directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~implicit-relative-path:~$ cd /challenge
hacker@paths~implicit-relative-path:/challenge$ run
bash: run: command not found
hacker@paths~implicit-relative-path:/challenge$ ./run
Correct!!!
./run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{8Z4JNZhBN1M--dU9R1kyuiv6WiV.QXxUTN0wSO4gjNzEzW}
```

## What I learned

I learnt more about ./ relative path to run programs in the current directory

## References

NA
