# Fun with Groups Names

### in this level, I'll allow you to use chgrp, but I have randomized the name of the group that your user is in. You will need to use the id command to figure that name out, then chgrp to victory!

**Flag:** `pwn.college{MP_ZJ3L8HBDWHTjdZk2cvb5fB6x.QXycjM1wSO4gjNzEzW}`

```
#!/bin/bash

hacker@permissions~fun-with-groups-names:~$ id
uid=1000(hacker) gid=1000(grp18510) groups=1000(grp18510)
hacker@permissions~fun-with-groups-names:~$ chgrp grp18510 /flag
hacker@permissions~fun-with-groups-names:~$ cat /flag
pwn.college{MP_ZJ3L8HBDWHTjdZk2cvb5fB6x.QXycjM1wSO4gjNzEzW}
```

## What I learned

I learnt to use the id command

## References

NA
