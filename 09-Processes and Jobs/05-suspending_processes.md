# Suspending Processes

### This level's run wants to see another copy of itself running and using the same terminal. How? Use the terminal to launch it, then suspend it, then launch another copy while the first is suspended!

**Flag:** `pwn.college{A_bLoNkI7TvKb-PX34EMLkNcQRY.QX1QDO0wSO4gjNzEzW}`

```
#!/bin/bash

hacker@processes~suspending-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running in
this terminal... Let's check!

UID          PID    PPID  C STIME TTY          TIME CMD
root         161     129  0 19:34 pts/0    00:00:00 bash /challenge/run
root         163     161  0 19:34 pts/0    00:00:00 ps -f

I don't see a second me!

To pass this level, you need to suspend me and launch me again! You can
background me with Ctrl-Z or, if you're not ready to do that for whatever
reason, just hit Enter and I'll exit!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~suspending-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running in
this terminal... Let's check!

UID          PID    PPID  C STIME TTY          TIME CMD
root         161     129  0 19:34 pts/0    00:00:00 bash /challenge/run
root         168     129  0 19:34 pts/0    00:00:00 bash /challenge/run
root         170     168  0 19:34 pts/0    00:00:00 ps -f

Yay, I found another version of me! Here is the flag:
pwn.college{A_bLoNkI7TvKb-PX34EMLkNcQRY.QX1QDO0wSO4gjNzEzW}
```

## What I learned

I learnt to suspend processes using ctrl + z

## References

NA
