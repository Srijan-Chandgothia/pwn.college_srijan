# Scripting With Arguments

### For this challenge, you need to write a script at /home/hacker/solve.sh that:

Takes two arguments
Outputs them in REVERSE order (second argument first, then the first argument)

**Flag:** `pwn.college{YRm6uuhM8bNQUiboGd5kgfsUkUn.0VNzMDOxwSO4gjNzEzW}`

```
#!/bin/bash

hacker@chaining~scripting-with-arguments:~$ cat > /home/hacker/solve.sh
#!/bin/bash
echo "$2 $1"
^C
hacker@chaining~scripting-with-arguments:~$ /challenge/run
Correct! Your script properly reversed the arguments.
Here's your flag:
pwn.college{YRm6uuhM8bNQUiboGd5kgfsUkUn.0VNzMDOxwSO4gjNzEzW}
```

## What I learned

I learnt to write scripts with arguments

## References

NA
