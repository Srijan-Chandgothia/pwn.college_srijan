# Deleting Newlines

### In this challenge, we'll inject a bunch of newlines into the flag. Delete them with tr's -d flag and the escaped newline specification!

**Flag:** `pwn.college{wXvASuPiPtNpxROMV-5Jl_B2MAv.0VNxEzNxwSO4gjNzEzW}`

```
#!/bin/bash

hacker@data~deleting-newlines:~$ /challenge/run | tr -d "\n"
Your line-split flag: pwn.college{wXvASuPiPtNpxROMV-5Jl_B2MAv.0VNxEzNxwSO4gjNzEzW}
```

## What I learned

I practiced using -d flag in tr command

## References

NA
