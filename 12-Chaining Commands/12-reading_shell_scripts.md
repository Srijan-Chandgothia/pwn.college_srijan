# Reading Shell Scripts

### In this level, we will learn to read shell scripts. /challenge/run is a shell script that requires you to put in a secret password, but that password is hardcoded into the script iself! Read the script (using, say, cat), figure out the password, and get the flag!

**Flag:** `pwn.college{oU-UQmb3yOThiAkFFW6oUJ7DRHY.0lMwgDOxwSO4gjNzEzW}`

```
#!/bin/bash

hacker@chaining~reading-shell-scripts:~$ cat /challenge/run
#!/opt/pwn.college/bash

read GUESS
if [ "$GUESS" == "hack the PLANET" ]
then
        echo "CORRECT! Your flag:"
        cat /flag
else
        echo "Read the /challenge/run file to figure out the correct password!"
fi
hacker@chaining~reading-shell-scripts:~$ /challenge/run
hack the PLANET
CORRECT! Your flag:
pwn.college{oU-UQmb3yOThiAkFFW6oUJ7DRHY.0lMwgDOxwSO4gjNzEzW}
```

## What I learned

I learnt to read scripts

## References

NA
