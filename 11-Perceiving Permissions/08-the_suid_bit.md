# The SUID Bit

### Now, we are going to let you add the SUID bit to the /challenge/getroot program in order to spawn a root shell for you to cat the flag yourself!

**Flag:** `pwn.college{UeUyrwzxHgXmoIiyVAR2hBPL9GG.QXzEjN0wSO4gjNzEzW}`

```
#!/bin/bash

hacker@permissions~the-suid-bit:~$ chmod u+s /challenge/getroot
hacker@permissions~the-suid-bit:~$ cat /flag
cat: /flag: Permission denied
hacker@permissions~the-suid-bit:~$ /challenge/getroot
SUCCESS! You have set the suid bit on this program, and it is running as root!
Here is your shell...
root@permissions~the-suid-bit:~# cat /flag
pwn.college{UeUyrwzxHgXmoIiyVAR2hBPL9GG.QXzEjN0wSO4gjNzEzW}
```

## What I learned

I learnt about SUID to give permission to run programs as the file owner

## References

NA
