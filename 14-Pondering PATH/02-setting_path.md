# Setting PATH

### Let's practice. This level's /challenge/run will run the win command via its bare name, but this command exists in the /challenge/more_commands/ directory, which is not initially in the PATH. The win command is the only thing that /challenge/run needs, so you can just overwrite PATH with that one directory. Good luck!

**Flag:** `pwn.college{8WtAbljyeWBp3iw97Nhl6Piv6m3.QX1cjM1wSO4gjNzEzW}`

```
#!/bin/bash

hacker@path~setting-path:~$ PATH=/challenge/more_commands/
hacker@path~setting-path:~$ /challenge/run
Invoking 'win'....
Congratulations! You properly set the flag and 'win' has launched!
pwn.college{8WtAbljyeWBp3iw97Nhl6Piv6m3.QX1cjM1wSO4gjNzEzW}
```

## What I learned

I learnt to edit the PATH variable to add directories and invoke commands via bare name

## References

NA
