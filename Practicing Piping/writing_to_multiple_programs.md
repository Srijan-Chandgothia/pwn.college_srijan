# Writing to Multiple Programs

### In this challenge, we have /challenge/hack, /challenge/the, and /challenge/planet. Run the /challenge/hack command, and duplicate its output as input to both the /challenge/the and the /challenge/planet commands!

**Flag:** `pwn.college{E8g0ZIjFnQd2dl6JrHV96tas2-c.QXwgDN1wSO4gjNzEzW}`

```
#!/bin/bash

hacker@piping~writing-to-multiple-programs:~$ /challenge/hack | tee >(/challenge/the) > >(/challenge/planet)
Congratulations, you have duplicated data into the input of two programs! Here
is your flag:
pwn.college{E8g0ZIjFnQd2dl6JrHV96tas2-c.QXwgDN1wSO4gjNzEzW}
```

## What I learned

I learnt to duplicate output to multiple programs

## References

NA
