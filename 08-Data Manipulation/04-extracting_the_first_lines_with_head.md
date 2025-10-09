# Extracting the First Lines with Head

### This challenge's /challenge/pwn outputs a bunch of data, and you'll need to pipe it through head to grab just the first 7 lines and then pipe them onwards to /challenge/college, which will give you the flag if you do this right! Your solution will be a long composite command with two pipes connecting three commands. Good luck!

**Flag:** `pwn.college{gVq1L0ZPtSp4G_STvnru3-XQFcj.0lNxEzNxwSO4gjNzEzW}`

```
#!/bin/bash

hacker@data~extracting-the-first-lines-with-head:~$ /challenge/pwn | head -n 7 | /challenge/college
Congratulations, you piped the right codes!
pwn.college{gVq1L0ZPtSp4G_STvnru3-XQFcj.0lNxEzNxwSO4gjNzEzW}
```

## What I learned

I learnt the head command to extract the first few lines of output

## References

NA
