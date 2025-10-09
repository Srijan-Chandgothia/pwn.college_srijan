# Cracking Passwords

### This level simulates this story, giving you a leak of /etc/shadow (in /challenge/shadow-leak). Crack it (this could take a few minutes), su to zardus, and run /challenge/run to get the flag!

**Flag:** `pwn.college{YVqd06R5M0otVU3dq4GTYd-p5MC.QX3UDN1wSO4gjNzEzW}`

```
#!/bin/bash

hacker@users~cracking-passwords:~$ john /challenge/shadow-leak
Loaded 1 password hash (crypt, generic crypt(3) [?/64])
Press 'q' or Ctrl-C to abort, almost any other key for status
0g 0:00:00:04 54% 1/3 0g/s 284.4p/s 284.4c/s 284.4C/s zrdus..zardus9999994
0g 0:00:00:15 0% 2/3 0g/s 280.9p/s 280.9c/s 280.9C/s deedee..grizzly
aardvark         (zardus)
1g 0:00:00:20 100% 2/3 0.04885g/s 284.4p/s 284.4c/s 284.4C/s Johnson..buzz
Use the "--show" option to display all of the cracked passwords reliably
Session completed
hacker@users~cracking-passwords:~$ su zardus
Password:
zardus@users~cracking-passwords:/home/hacker$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{YVqd06R5M0otVU3dq4GTYd-p5MC.QX3UDN1wSO4gjNzEzW}
```

## What I learned

I learnt to crack passwords using john

## References

NA
