# Redirecting Script Output

### All of the various redirection methods work: > for stdout, 2> for stderr, < for stdin, >> and 2>> for append-mode redirection, >& for redirecting to other file descriptors, and | for piping to another command.

In this level, we will practice piping (|) from your script to another program. Like before, you need to create a script that calls the /challenge/pwn command followed by the /challenge/college command, and pipe the output of the script into a single invocation of the /challenge/solve command!

**Flag:** `pwn.college{cTFSo3j10waUKTDzn1BK_nTXIs3.QX4ETO0wSO4gjNzEzW}`

```
#!/bin/bash

hacker@chaining~redirecting-script-output:~$ echo "/challenge/pwn;/challenge/college" > x.sh
hacker@chaining~redirecting-script-output:~$ bash x.sh | /challenge/solve
Correct! Here is your flag:
pwn.college{cTFSo3j10waUKTDzn1BK_nTXIs3.QX4ETO0wSO4gjNzEzW}
```

## What I learned

I learnt to redirect script outputs

## References

NA
