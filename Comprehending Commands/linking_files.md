# Linking Files

### In this level the flag is, as always, in /flag, but /challenge/catflag will instead read out /home/hacker/not-the-flag. Use the symlink, and fool it into giving you the flag!

**Flag:** `pwn.college{QMvtNZh1TeGk0QuSzxX3zLGalCt.QX5ETN1wSO4gjNzEzW}`

```
#!/bin/bash

hacker@commands~linking-files:~$ ln -s /flag /home/hacker/not-the-flag
hacker@commands~linking-files:~$ /challenge/catflag
About to read out the /home/hacker/not-the-flag file!
pwn.college{QMvtNZh1TeGk0QuSzxX3zLGalCt.QX5ETN1wSO4gjNzEzW}
```

## What I learned

I learnt to link files with symbolic links or symlinks

## References

NA
