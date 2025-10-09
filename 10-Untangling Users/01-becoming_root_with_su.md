# Becoming Root with su

### But THIS challenge (and only this challenge) does have a root password. That password is hack-the-planet, and you must provide it to su to become root! Go do that, and read the flag!

**Flag:** `pwn.college{8cypWn6pGbAo-DeE7UbRnyCr-j3.QX1UDN1wSO4gjNzEzW}`

```
#!/bin/bash

hacker@users~becoming-root-with-su:~$ su
Password:
root@users~becoming-root-with-su:/home/hacker# cat /flag
pwn.college{8cypWn6pGbAo-DeE7UbRnyCr-j3.QX1UDN1wSO4gjNzEzW}
```

## What I learned

I learnt to use su and enter password to become root

## References

NA
