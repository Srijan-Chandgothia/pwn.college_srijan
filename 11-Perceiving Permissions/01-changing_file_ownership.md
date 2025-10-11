# Changing File Ownership

### In this level, we will practice changing the owner of the /flag file to the hacker user, and then read the flag. For this challenge only, I made it so that you can use chown to your heart's content as the hacker user (again, typically, this requires you to be root). Use this power wisely and chown away!

**Flag:** `pwn.college{ggX9u0vxVOL2lsIgHd0Htt-W281.QXxEjN0wSO4gjNzEzW}`

```
#!/bin/bash

hacker@permissions~changing-file-ownership:~$ chown hacker /flag
hacker@permissions~changing-file-ownership:~$ cat /flag
pwn.college{ggX9u0vxVOL2lsIgHd0Htt-W281.QXxEjN0wSO4gjNzEzW}
```

## What I learned

I learnt to change the file owner of a file

## References

NA
