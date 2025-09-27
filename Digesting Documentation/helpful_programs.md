# Helpful Programs

### In this level, you will practice reading a program's documentation with --help. Try it out!

**Flag:** `pwn.college{0yFSADrL7gFG-KKJE-GxnZfVIE0.QX3IDO0wSO4gjNzEzW}`

```
#!/bin/bash

hacker@man~helpful-programs:~$ /challenge/challenge --h
usage: a challenge to make you ask for help [-h] [--fortune] [-v] [-g GIVE_THE_FLAG] [-p]

optional arguments:
  -h, --help            show this help message and exit
  --fortune             read your fortune
  -v, --version         get the version number
  -g GIVE_THE_FLAG, --give-the-flag GIVE_THE_FLAG
                        get the flag, if given the correct value
  -p, --print-value     print the value that will cause the -g option to give you the flag
hacker@man~helpful-programs:~$ /challenge/challenge --p
The secret value is: 70
hacker@man~helpful-programs:~$ /challenge/challenge --g 70
Correct usage! Your flag: pwn.college{0yFSADrL7gFG-KKJE-GxnZfVIE0.QX3IDO0wSO4gjNzEzW}
```

## What I learned

I used help command to figure out how to get the flag

## References

NA
