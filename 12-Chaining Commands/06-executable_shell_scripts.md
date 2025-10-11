# Executable Shell Scripts

### Make a shellscript that will invoke /challenge/solve, make it executable, and run it without explicitly invoking bash!

**Flag:** `pwn.college{4uzIvakopfrqAN3ou0U2gdExs0n.QX0cjM1wSO4gjNzEzW}`

```
#!/bin/bash

hacker@chaining~executable-shell-scripts:~$ echo "/challenge/solve" > x.sh
hacker@chaining~executable-shell-scripts:~$ chmod a+x x.sh
hacker@chaining~executable-shell-scripts:~$ x.sh
bash: x.sh: command not found
hacker@chaining~executable-shell-scripts:~$ ./x.sh
Congratulations on your shell script execution! Your flag:
pwn.college{4uzIvakopfrqAN3ou0U2gdExs0n.QX0cjM1wSO4gjNzEzW}
```

## What I learned

I learnt to execute .sh scripts without mentioning bash

## References

NA
