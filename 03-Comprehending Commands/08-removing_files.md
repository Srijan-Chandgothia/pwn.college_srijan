# Removing Files

### This challenge will create a delete_me file in your home directory! Delete it, then run /challenge/check, which will make sure you've deleted it and then give you the flag!

**Flag:** `pwn.college{cam9syxJBb1Bq6R-7pE5RX5hC_G.QX2kDM1wSO4gjNzEzW}`

```
#!/bin/bash

hacker@commands~removing-files:~$ /challenge/check
It looks like /home/hacker/delete_me still exists! rm it.
hacker@commands~removing-files:~$ rm delete_me
hacker@commands~removing-files:~$ /challenge/check
Excellent removal. Here is your reward:
pwn.college{cam9syxJBb1Bq6R-7pE5RX5hC_G.QX2kDM1wSO4gjNzEzW}
```

## What I learned

I learnt the rm command to remove files

## References

NA
