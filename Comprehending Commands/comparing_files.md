# Comparing Files

### Now for your challenge! There are two files in /challenge:

/challenge/decoys_only.txt contains 100 fake flags
/challenge/decoys_and_real.txt contains all 100 fake flags plus the one real flag
Use diff to find what's different between these files and get your flag!

**Flag:** `pwn.college{IyEMMCJgsFhTwY-iECZGHypj46z.01MwMDOxwSO4gjNzEzW}`

```
#!/bin/bash

hacker@commands~comparing-files:~$ diff /challenge/decoys_only.txt /challenge/decoys_and_real.txt
52a53
> pwn.college{IyEMMCJgsFhTwY-iECZGHypj46z.01MwMDOxwSO4gjNzEzW}
```

## What I learned

I learnt the diff command which comapres and lists differences between two files

## References

NA
