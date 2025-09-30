# Redirecting Errors

### In this challenge, you will need to redirect the output of /challenge/run, like before, to myflag, and the "errors" (in our case, the instructions) to instructions. You'll notice that nothing will be printed to the terminal, because you have redirected everything! You can find the instructions/feedback in instructions and the flag in myflag when you successfully pull this off!

**Flag:** `pwn.college{0hGaZle43avn46jZvliwBEOe88z.QX3YTN0wSO4gjNzEzW}`

```
#!/bin/bash

hacker@piping~redirecting-errors:~$ /challenge/run > myflag 2> instructions
hacker@piping~redirecting-errors:~$ cat myflag

[FLAG] Here is your flag:
[FLAG] pwn.college{0hGaZle43avn46jZvliwBEOe88z.QX3YTN0wSO4gjNzEzW}
```

## What I learned

I learnt to redirect errors to files

## References

NA
