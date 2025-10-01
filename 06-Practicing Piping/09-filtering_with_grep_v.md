# Filtering With grep -v

### In this challenge, /challenge/run will output the flag to stdout, but it will also output over 1000 decoy flags (containing the word DECOY somewhere in the flag) mixed in with the real flag. You'll need to filter out the decoys while keeping the real flag!

**Flag:** `pwn.college{kT-Z7iala_GBNISJ-M-YodcbbEe.0FOxEzNxwSO4gjNzEzW}`

```
#!/bin/bash

hacker@piping~filtering-with-grep-v:~$ /challenge/run | grep -v DECOY
pwn.college{kT-Z7iala_GBNISJ-M-YodcbbEe.0FOxEzNxwSO4gjNzEzW}
```

## What I learned

I learnt about the -v option to invert and filter out grep results

## References

NA
