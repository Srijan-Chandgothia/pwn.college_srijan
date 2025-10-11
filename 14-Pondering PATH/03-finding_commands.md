# Finding Commands

### In this challenge, we added a win command somewhere in your $PATH, but it won't give you the flag. Instead, it's in the same directory as a flag file that we made readable by you! You must find win (with the which command), and cat the flag out of that directory!

**Flag:** `pwn.college{AAn2snEQYsk4h37FZecPZyvAO9K.01NzEzNxwSO4gjNzEzW}`

```
#!/bin/bash

hacker@path~finding-commands:~$ which win
/challenge/paths/7805/win
hacker@path~finding-commands:~$ cat /challenge/paths/7805/flag
pwn.college{AAn2snEQYsk4h37FZecPZyvAO9K.01NzEzNxwSO4gjNzEzW}
```

## What I learned

I learnt to use which command

## References

NA
