# Help for Builtins

### In this challenge, we'll practice using help to look up help for builtins. This challenge's challenge command is a shell builtin, rather than a program. Like before, you need to lookup its help to figure out the secret value to pass to it!

**Flag:** `pwn.college{gfywTLr4n7xlXN5pC0QJdDs1zG1.QX0ETO0wSO4gjNzEzW}`

```
#!/bin/bash

hacker@man~help-for-builtins:~$ help challenge
challenge: challenge [--fortune] [--version] [--secret SECRET]
    This builtin command will read you the flag, given the right arguments!

    Options:
      --fortune         display a fortune
      --version         display the version
      --secret VALUE    prints the flag, if VALUE is correct

    You must be sure to provide the right value to --secret. That value
    is "gfywTLr4".
hacker@man~help-for-builtins:~$ /challenge/challenge --secret "gfywTLr4"
bash: /challenge/challenge: No such file or directory
hacker@man~help-for-builtins:~$ challenge --secret "gfywTLr4"
Correct! Here is your flag!
pwn.college{gfywTLr4n7xlXN5pC0QJdDs1zG1.QX0ETO0wSO4gjNzEzW}
```

## What I learned

I learnt to use the help command for builtin programs

## References

NA
