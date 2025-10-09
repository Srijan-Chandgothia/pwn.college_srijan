# Process Exit Codes

### In this challenge, you must retrieve the exit code returned by /challenge/get-code and then run /challenge/submit-code with that error code as an argument. Good luck!

**Flag:** `pwn.college{8TICubfMY_8HQO_9TB8IoznPdLO.QX5YDO1wSO4gjNzEzW}`

```
#!/bin/bash

hacker@processes~process-exit-codes:~$ /challenge/get-code
Exiting with an error code!
hacker@processes~process-exit-codes:~$ echo $?
68
hacker@processes~process-exit-codes:~$ /challenge/submit-code -68
Incorrect... Make sure to use $? immediately after running /challenge/get-code.
Your shell will overwrite the $? variable with the exit value of any other
command you run!
hacker@processes~process-exit-codes:~$ /challenge/submit-code 68
CORRECT! Here is your flag:
pwn.college{8TICubfMY_8HQO_9TB8IoznPdLO.QX5YDO1wSO4gjNzEzW}
```

## What I learned

I learnt about process exit codes

## References

NA
