# Redirecting Input

### In this level, we will practice using /challenge/run, which will require you to redirect the PWN file to it and have the PWN file contain the value COLLEGE! To write that value to the PWN file, recall the prior challenge on output redirection from echo!

**Flag:** `pwn.college{039ZriFAbb6mZsNvq77tK5ydR49.QXwcTN0wSO4gjNzEzW}`

```
#!/bin/bash

hacker@piping~redirecting-input:~$ echo COLLEGE > PWN
hacker@piping~redirecting-input:~$ /challenge/run < PWN
Reading from standard input...
Correct! You have redirected the PWN file into my standard input, and I read
the value 'COLLEGE' out of it!
Here is your flag:
pwn.college{039ZriFAbb6mZsNvq77tK5ydR49.QXwcTN0wSO4gjNzEzW}
```

## What I learned

I learnt to redirect inputs

## References

NA
