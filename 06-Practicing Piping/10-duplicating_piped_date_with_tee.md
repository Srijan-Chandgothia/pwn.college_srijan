# Duplicating Piped Data With Tee

### This process' /challenge/pwn must be piped into /challenge/college, but you'll need to intercept the data to see what pwn needs from you!

**Flag:** `pwn.college{Ut_cEMVV1M1axHPN-YOB4NStg8t.QXxITO0wSO4gjNzEzW}`

```
#!/bin/bash

hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn | /challenge/college
Processing...
The input to 'college' does not contain the correct secret code! This code
should be provided by the 'pwn' command. HINT: use 'tee' to intercept the
output of 'pwn' and figure out what the code needs to be.
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn | tee pwn | /challenge/college
Processing...
The input to 'college' does not contain the correct secret code! This code
should be provided by the 'pwn' command. HINT: use 'tee' to intercept the
output of 'pwn' and figure out what the code needs to be.
hacker@piping~duplicating-piped-data-with-tee:~$ cat pwn
Usage: /challenge/pwn --secret [SECRET_ARG]

SECRET_ARG should be "Ut_cEMVV"
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn --secret Ut_cEMVV | /challenge/college
Processing...
Correct! Passing secret value to /challenge/college...
Great job! Here is your flag:
pwn.college{Ut_cEMVV1M1axHPN-YOB4NStg8t.QXxITO0wSO4gjNzEzW}
```

## What I learned

I learnt to duplicate data with tee

## References

NA
