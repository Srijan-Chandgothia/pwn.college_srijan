# Scripting with Conditionals

### For this challenge, write a script at /home/hacker/solve.sh that:

Takes one argument
If the argument is "pwn", output "college"
For any other input, output nothing

**Flag:** `pwn.college{0nP7Y97MrsE3-MpKgiytgWMqw7j.0lNzMDOxwSO4gjNzEzW}`

```
#!/bin/bash

hacker@chaining~scripting-with-conditionals:~$ cat > /home/hacker/solve.sh
#!/bin/bash
if [ "$1" == "pwn" ]
then
        echo "college"
fi
^C
hacker@chaining~scripting-with-conditionals:~$ /challenge/run
Correct! Your script properly handles all the conditions.
Here's your flag:
pwn.college{0nP7Y97MrsE3-MpKgiytgWMqw7j.0lNzMDOxwSO4gjNzEzW}
```

## What I learned

I learnt to write scripts with conditions

## References

NA
