# Listing Processes

### In this level, I have once again renamed /challenge/run to a random filename, and this time made it so that you cannot ls the /challenge directory! But I also launched it, so you can find it in the running process list, figure out the filename, and relaunch it directly for the flag! Good luck!

**Flag:** `pwn.college{oMyDEQZHaD2xMXHWKyJDcKutlmD.QX4MDO0wSO4gjNzEzW}`

```
#!/bin/bash

hacker@processes~listing-processes:~$ ps -ef
UID          PID    PPID  C STIME TTY          TIME CMD
root           1       0  0 19:18 ?        00:00:00 /sbin/docker-init -- /nix/var/nix/profiles/dojo-workspace/bin/dojo-i
root           7       1  0 19:18 ?        00:00:00 /run/dojo/bin/sleep 6h
root         132       1  0 19:18 ?        00:00:00 /challenge/29454-run-8835
root         135     132  0 19:18 ?        00:00:00 sleep 6h
hacker       146       1  0 19:18 ?        00:00:00 /nix/store/g0q8n7xfjp7znj41hcgrq893a9m0i474-ttyd-1.7.7/bin/ttyd --po
hacker       150     146  0 19:18 pts/0    00:00:00 /run/dojo/bin/bash --login
hacker       160       0  0 19:18 pts/1    00:00:00 /nix/store/0nxvi9r5ymdlr2p24rjj9qzyms72zld1-bash-interactive-5.2p37/
hacker       166     160  2 19:18 pts/1    00:00:00 /run/dojo/bin/bash --login
hacker       176     166  0 19:19 pts/1    00:00:00 ps -ef
hacker@processes~listing-processes:~$ /challenge/29454-run-8835
Yahaha, you found me! Here is your flag:
pwn.college{oMyDEQZHaD2xMXHWKyJDcKutlmD.QX4MDO0wSO4gjNzEzW}
Now I will sleep for a while (so that you could find me with 'ps').
```

## What I learned

I learnt about the ps command for listing processes

## References

NA
