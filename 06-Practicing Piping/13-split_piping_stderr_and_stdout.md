# Split-Piping stderr and stdout

### In this challenge, you have:

/challenge/hack: this produces data on stdout and stderr
/challenge/the: you must redirect hack's stderr to this program
/challenge/planet: you must redirect hack's stdout to this program

**Flag:** `pwn.college{8l9LXinZAi_kPG0hQuU4sAASoJa.QXxQDM2wSO4gjNzEzW}`

```
#!/bin/bash

hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack > >(/challenge/planet) 2> >(/challenge/the)
Congratulations, you have learned a redirection technique that even experts
struggle with! Here is your flag:
pwn.college{8l9LXinZAi_kPG0hQuU4sAASoJa.QXxQDM2wSO4gjNzEzW}
```

## What I learned

I practiced piping concepts

## References

NA
