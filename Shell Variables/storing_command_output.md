# Storing Command Output

### Read the output of the /challenge/run command directly into a variable called PWN, and it will contain the flag!

**Flag:** `pwn.college{ETKav93JuVXhQgcNOsU7yCjsdi-.QX1cDN1wSO4gjNzEzW}`

```
#!/bin/bash

hacker@variables~storing-command-output:~$ PWN=$(/challenge/run)
Congratulations! You have read the flag into the PWN variable. Now print it out
and submit it!
hacker@variables~storing-command-output:~$ echo $PWN
pwn.college{ETKav93JuVXhQgcNOsU7yCjsdi-.QX1cDN1wSO4gjNzEzW}
```

## What I learned

I learnt to store command outputs as variables

## References

NA
