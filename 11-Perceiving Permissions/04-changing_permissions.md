# Changing Permissions

### In this challenge, you must change the permissions of the /flag file to read it! Typically, you need to have write access to the file in order to change its permissions, but I have made the chmod command all-powerful for this level, and you can chmod anything you want even though you are the hacker user. This is an ultimate power. The /flag file is owned by root, and you can't change that, but you can make it readable. Go and solve this!

**Flag:** `pwn.college{A9bJ_C0M1LaqXPsWKBZYpmembZD.QXzcjM1wSO4gjNzEzW}`

```
#!/bin/bash

hacker@permissions~changing-permissions:~$ ls -l
total 36
-rw-r--r-- 1 hacker hacker   4 Sep 30 15:27 COLLEGE
drwxr-xr-x 1 hacker hacker   0 Sep 22 16:34 Desktop
-rw-r--r-- 1 hacker hacker   8 Sep 30 15:41 PWN
-rw-r--r-- 1 root   hacker  60 Sep 22 12:48 f
lrwxrwxrwx 1 hacker hacker  18 Sep 27 19:18 flag -> /challenge/catflag
-rw-r--r-- 1 hacker hacker 829 Sep 30 15:37 instructions
-rw-r--r-- 1 hacker hacker  95 Sep 30 15:37 myflag
lrwxrwxrwx 1 hacker hacker   5 Sep 27 19:29 not-the-flag -> /flag
-rw-r--r-- 1 root   hacker  77 Sep 30 16:00 pwn
-rw-r--r-- 1 hacker hacker 437 Sep 30 15:33 the-flag
hacker@permissions~changing-permissions:~$ chmod a+r
chmod: missing operand after ‘a+r’
Try 'chmod --help' for more information.
hacker@permissions~changing-permissions:~$ chmod a+r /flag
hacker@permissions~changing-permissions:~$ cat /flag
pwn.college{A9bJ_C0M1LaqXPsWKBZYpmembZD.QXzcjM1wSO4gjNzEzW}
```

## What I learned

I learnt about file permissions and changing them

## References

NA
