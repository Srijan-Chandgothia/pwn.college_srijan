# Groups and Files

### In this level, I have made the flag readable by whatever group owns it, but this group is currently root. Luckily, I have also made it possible for you to invoke chgrp as the hacker user! Change the group ownership of the flag file, and read the flag!

**Flag:** `pwn.college{Uy93HJLoao8-bA5juYfa0G__lPU.QXxcjM1wSO4gjNzEzW}`

```
#!/bin/bash

hacker@permissions~groups-and-files:~$ chgrp hacker /flag
hacker@permissions~groups-and-files:~$ cat /flag
pwn.college{Uy93HJLoao8-bA5juYfa0G__lPU.QXxcjM1wSO4gjNzEzW}
```

## What I learned

I learnt to change group of a file

## References

NA
