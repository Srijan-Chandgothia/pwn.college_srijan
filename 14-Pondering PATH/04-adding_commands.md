# Adding Commands

### Previously, the win command that /challenge/run executed was stored in /challenge/more_commands. This time, win does not exist! Recall the final level of Chaining Commands, and make a shell script called win, add its location to the PATH, and enable /challenge/run to find it!

**Flag:** `pwn.college{4rEuVTrPt0El-ALKEMCguYd1OA0.QX2cjM1wSO4gjNzEzW}`

```
#!/bin/bash

hacker@path~adding-commands:~$ cat > /home/hacker/win
#!/bin/bash
/run/dojo/bin/cat /flag
^C
hacker@path~adding-commands:~$ chmod a+x /home/hacker/win
hacker@path~adding-commands:~$ PATH="/home/hacker"
hacker@path~adding-commands:~$ /challenge/run
Invoking 'win'....
pwn.college{4rEuVTrPt0El-ALKEMCguYd1OA0.QX2cjM1wSO4gjNzEzW}
```

## What I learned

I learnt to add commands

## References

NA
