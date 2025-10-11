# Scripting with Multiple Conditions

### For this challenge, write a script at /home/hacker/solve.sh that:

Takes one argument
If the argument is "hack", output "the planet"
If the argument is "pwn", output "college"
If the argument is "learn", output "linux"
For any other input, output "unknown"

**Flag:** `pwn.college{cK45D7W5ZFJnfL-1rYYZmvgEaNm.0FOzMDOxwSO4gjNzEzW}`

```
#!/bin/bash

hacker@chaining~scripting-with-multiple-conditions:~$ cat > /home/hacker/solve.sh
#!/bin/bash
if [ "$1" == "hack" ]
then
        echo "the planet"
elif [ "$1" == "pwn" ]
then
        echo "college"
elif [ "$1" == "learn" ]
then
        echo "linux"
else
        echo "unknown"
fi
^C
hacker@chaining~scripting-with-multiple-conditions:~$ /challenge/run
Correct! Your script properly handles all the conditions with elif.
Here's your flag:
pwn.college{cK45D7W5ZFJnfL-1rYYZmvgEaNm.0FOzMDOxwSO4gjNzEzW}
```

## What I learned

I learnt to write scripts with multiple conditions

## References

NA
