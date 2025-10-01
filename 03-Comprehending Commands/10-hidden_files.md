# Hidden Files

### Go find the flag, hidden as a dot-prepended file in /. To view them with ls, you need to invoke ls with the -a flag.

**Flag:** `pwn.college{sTERlW72FzjmYReAiMOf-ZPSBkV.QXwUDO0wSO4gjNzEzW}`

```
#!/bin/bash

hacker@commands~hidden-files:~$ ls -a
.  ..  .ICEauthority  .bash_history  .cache  .config  .dbus  .local  Desktop  f
hacker@commands~hidden-files:~$ ls /
bin   challenge  etc   lib    lib64   media  nix  proc  run   srv  tmp  var
boot  dev        home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~hidden-files:~$ ls / -a
.   .dockerenv             bin   challenge  etc   lib    lib64   media  nix  proc  run   srv  tmp  var
..  .flag-106683165717303  boot  dev        home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~hidden-files:~$ /.flag-106683165717303
bash: /.flag-106683165717303: Permission denied
hacker@commands~hidden-files:~$ cat /.flag-106683165717303
pwn.college{sTERlW72FzjmYReAiMOf-ZPSBkV.QXwUDO0wSO4gjNzEzW}
```

## What I learned

I learnt to list all files using -a flag

## References

NA
