# Searching for Manuals

### This level is tricky: it hides the manpage for the challenge by randomizing its name. Luckily, all of the manpages are gathered in a searchable database, so you'll be able to search the man page database to find the hidden challenge man page! To figure out how to search for the right manpage, read the man page manpage by doing: man man!

HINT 1: man man teaches you advanced usage of the man command itself, and you must use this knowledge to figure out how to search for the hidden manpage that will tell you how to use /challenge/challenge

HINT 2: though the manpage is randomly named, you still actually use /challenge/challenge to get the flag!

**Flag:** `pwn.college{M_GZ6TVw7ollJhHIEEdv1AdXw2R.QX2EDO0wSO4gjNzEzW}`

```
#!/bin/bash

hacker@man~searching-for-manuals:~$ man man
hacker@man~searching-for-manuals:~$ apropos challenge
wollhdvdww (1)       - print the flag!
hacker@man~searching-for-manuals:~$ man wollhdvdww
hacker@man~searching-for-manuals:~$ /challenge/challenge --wollhd 671
Correct usage! Your flag: pwn.college{M_GZ6TVw7ollJhHIEEdv1AdXw2R.QX2EDO0wSO4gjNzEzW}
```

## What I learned

I learnt to read the manual for man command and figure out how to search for other commands manuals

## References

NA
