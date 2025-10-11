# Scripting with Default Cases

### For this challenge, write a script at /home/hacker/solve.sh that:

Takes one argument
If the argument is "pwn", output "college"
For any other input, output "nope"

**Flag:** `pwn.college{0c5IkQbETEqvv3fdhcp8jL9N2yB.01NzMDOxwSO4gjNzEzW}`

```
#!/bin/bash

hacker@chaining~scripting-with-default-cases:~$ cat > /home/hacker/solve.sh
#!/bin/bash
if [ "$1" == "pwn" ]
then
        echo "college"
else
        echo "nope"
fi
^C
hacker@chaining~scripting-with-default-cases:~$ /challenge/run
Correct! Your script properly handles the if/else conditions.
Here's your flag:
pwn.college{0c5IkQbETEqvv3fdhcp8jL9N2yB.01NzMDOxwSO4gjNzEzW}
```

## What I learned

I learnt to write scripts with else condition

## References

NA
