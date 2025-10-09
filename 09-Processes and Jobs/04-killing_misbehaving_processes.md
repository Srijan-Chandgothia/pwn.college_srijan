# Killing Misbehaving Processes

### In this challenge, there's a decoy process that's hogging a critical resource - a named pipe (FIFO) at /tmp/flag_fifo into which (like in the Practicing Piping FIFO challenge) /challenge/run wants to write your flag. You need to kill this process.

**Flag:** `pwn.college{YD4DPvh4uEbWeuN57ptrUFMpMFW.0FNzMDOxwSO4gjNzEzW}`

```
#!/bin/bash

hacker@processes~killing-misbehaving-processes:~$ ps -ef
UID          PID    PPID  C STIME TTY          TIME CMD
root           1       0  0 19:31 ?        00:00:00 /sbin/docker-init -- /nix/var/nix/profiles/dojo-workspace/bin/dojo-i
root           7       1  0 19:31 ?        00:00:00 /run/dojo/bin/sleep 6h
root         137       1  0 19:31 ?        00:00:00 /bin/bash /challenge/.init
root         138       1  0 19:31 ?        00:00:00 /bin/bash /challenge/.init
root         139       1  0 19:31 ?        00:00:00 su -c exec /challenge/decoy > /tmp/flag_fifo hacker
root         140     137  0 19:31 ?        00:00:00 sleep 6h
root         141     138  0 19:31 ?        00:00:00 sleep 6h
hacker       142     139  0 19:31 ?        00:00:00 /usr/bin/python /challenge/decoy
hacker       144       0  0 19:31 pts/0    00:00:00 /nix/store/0nxvi9r5ymdlr2p24rjj9qzyms72zld1-bash-interactive-5.2p37/
hacker       150     144  0 19:31 pts/0    00:00:00 /run/dojo/bin/bash --login
hacker       168       1  0 19:31 ?        00:00:00 /nix/store/g0q8n7xfjp7znj41hcgrq893a9m0i474-ttyd-1.7.7/bin/ttyd --po
hacker       172     168  0 19:31 pts/1    00:00:00 /run/dojo/bin/bash --login
hacker       182     150  0 19:31 pts/0    00:00:00 ps -ef
hacker@processes~killing-misbehaving-processes:~$ kill 142
hacker@processes~killing-misbehaving-processes:~$ /challenge/run
Sending the flag to /tmp/flag_fifo!
hacker@processes~killing-misbehaving-processes:~$ cat /tmp/flag_fifo
pwn.college{YD4DPvh4uEbWeuN57ptrUFMpMFW.0FNzMDOxwSO4gjNzEzW}
```

## What I learned

I practiced killing processes

## References

NA
