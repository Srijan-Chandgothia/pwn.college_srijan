# Touching Files

### In this level, please create two files: /tmp/pwn and /tmp/college, and run /challenge/run to get your flag!

**Flag:** `pwn.college{Y01RhT3GlK0I8OVuHWWawPsoWOF.QXwMDO0wSO4gjNzEzW}`

```
#!/bin/bash

example triple ticks for bash
hacker@commands~touching-files:~$ /challenge/run
Uh oh! /tmp/pwn does not exist. Please use the 'touch' command to create it!
hacker@commands~touching-files:~$ cd /tmp
hacker@commands~touching-files:/tmp$ ls
bin  hsperfdata_root  tmp.4mK6TfTSUV
hacker@commands~touching-files:/tmp$ touch pwn college
hacker@commands~touching-files:/tmp$ ls
bin  college  hsperfdata_root  pwn  tmp.4mK6TfTSUV
hacker@commands~touching-files:/tmp$ cd
hacker@commands~touching-files:~$ /challenge/run
Success! Here is your flag:
pwn.college{Y01RhT3GlK0I8OVuHWWawPsoWOF.QXwMDO0wSO4gjNzEzW}
```

## What I learned

I learnt to create files with touch command

## References

NA
