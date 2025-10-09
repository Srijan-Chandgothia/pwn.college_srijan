# Killing Processes

### In this challenge, /challenge/run will refuse to run while /challenge/dont_run is running! You must find the dont_run process and kill it. If you fail, pwn.college will disavow all knowledge of your mission. Good luck.

**Flag:** `pwn.college{Qrl-KEtxbztBdiA7vql5hYZW0rx.QXyQDO0wSO4gjNzEzW}`

```
#!/bin/bash

hacker@processes~killing-processes:~$ ps -ef
UID          PID    PPID  C STIME TTY          TIME CMD
root           1       0  0 19:21 ?        00:00:00 /sbin/docker-init -- /nix/var/nix/profiles/dojo-workspace/bin/dojo-i
root           7       1  0 19:21 ?        00:00:00 /run/dojo/bin/sleep 6h
root         135       1  0 19:21 ?        00:00:00 su -c /challenge/.launcher hacker
hacker       136     135  0 19:21 ?        00:00:00 /challenge/dont_run
hacker       137     136  0 19:21 ?        00:00:00 sleep 6h
hacker       139       0  0 19:21 pts/0    00:00:00 /nix/store/0nxvi9r5ymdlr2p24rjj9qzyms72zld1-bash-interactive-5.2p37/
hacker       145     139  0 19:21 pts/0    00:00:00 /run/dojo/bin/bash --login
hacker       163       1  0 19:21 ?        00:00:00 /nix/store/g0q8n7xfjp7znj41hcgrq893a9m0i474-ttyd-1.7.7/bin/ttyd --po
hacker       167     163  0 19:21 pts/1    00:00:00 /run/dojo/bin/bash --login
hacker       177     145  0 19:21 pts/0    00:00:00 ps -ef
hacker@processes~killing-processes:~$ kill 136
hacker@processes~killing-processes:~$ /challenge/run
Great job! Here is your payment:
pwn.college{Qrl-KEtxbztBdiA7vql5hYZW0rx.QXyQDO0wSO4gjNzEzW}
```

## What I learned

I learnt to kill processes

## References

NA
